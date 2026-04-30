"Para explicarlo simple: @Bean es un método que sirve como fábrica. Yo escribo el código para crear e inicializar un objeto complejo, y al ponerle @Bean, Spring lo guarda en su contenedor. Así, cualquier otra parte de mi app puede usar ese objeto ya configurado simplemente pidiéndolo con @Autowired".

1. Nivel Básico: Concepto y Diferenciación
Estas preguntas sirven para filtrar si conoces la herramienta.

¿Cuál es la diferencia fundamental entre @Component y @Bean?

Lo que buscan: Que digas que @Component es para tus clases (automático) y @Bean es para clases externas o configuraciones manuales (método).

¿Dónde se suelen declarar los métodos anotados con @Bean?

Lo que buscan: Que menciones las clases anotadas con @Configuration.

2. Nivel Intermedio: Escenarios y Práctica
Aquí es donde demuestras que sabes aplicar la teoría.

Si tengo una librería externa de seguridad que no usa Spring, ¿cómo la integrarías en tu proyecto para poder usarla con @Autowired?

Lo que buscan: Que respondas: "Crearía un método con @Bean en una clase de configuración que instancie la clase de esa librería".

Imagina que un @Bean necesita otro objeto para funcionar. ¿Cómo se lo pasas?

Lo que buscan: Que sepas que puedes pasar ese objeto como parámetro del método y Spring lo inyectará automáticamente.

3. Nivel Avanzado: Comportamiento Interno
Aquí es donde separas a un principiante de un experto.

¿Qué sucede si llamo dos veces a un método @Bean desde otra parte de mi clase @Configuration? ¿Se crean dos objetos?

Lo que buscan: Que sepas que, gracias a CGLIB (si usas @Configuration), Spring intercepta la llamada y devuelve siempre la misma instancia (Singleton).

¿Para qué sirve el atributo name en la anotación @Bean?

Lo que buscan: Que expliques que sirve para identificar el bean si tienes varios del mismo tipo, evitando conflictos de ambigüedad.

1. El Ejemplo de Código
Aquí creamos un "Cliente de Almacenamiento" que requiere una clave y una ruta específica:

Java
// 1. La clase de configuración (El taller)
@Configuration
public class AlmacenamientoConfig {

    // 2. El método @Bean (La receta de fabricación)
    @Bean
    public ClienteAlmacenamiento clienteDeFotos() {
        // Aquí personalizamos el objeto antes de que Spring lo guarde
        ClienteAlmacenamiento cliente = new ClienteAlmacenamiento();
        cliente.setRuta("/usuarios/fotos");
        cliente.setApiKey("SECURE_123");
        return cliente; 
    }
}
Ahora, en cualquier otra parte de tu app (un Controller o un Service), simplemente lo pides:

Java
@Service
public class PerfilService {
    @Autowired
    private ClienteAlmacenamiento clienteDeFotos; // Spring te entrega el que configuraste arriba
}
2. ¿Por qué usar @Configuration? (La razón técnica)
Esta es la parte que te hará destacar en la entrevista. Podrías poner un @Bean en cualquier clase (como un @Component), pero DEBES usar @Configuration por una razón clave: La garantía del Singleton.
