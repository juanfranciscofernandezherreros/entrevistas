Nivel Básico

Estas preguntas están orientadas a evaluar tus conocimientos básicos de programación y conceptos fundamentales.

1- ¿Qué es un API? 

Un API (Interfaz de Programación de Aplicaciones) es un conjunto de funciones y procedimientos que permiten la comunicación entre diferentes aplicaciones o servicios. Un API define cómo los programas pueden interactuar con otros sistemas mediante solicitudes y respuestas.

2- ¿Qué es un servidor web y cómo funciona?

Un servidor web es un sistema informático que entrega contenido web a los usuarios a través de internet. Funciona recibiendo solicitudes HTTP de los navegadores y enviando la respuesta, que generalmente es un archivo HTML, imágenes, o datos en formato JSON.

3- Explicame qué es HTTP y cómo funcionan los métodos GET, POST, PUT y DELETE.

HTTP (HyperText Transfer Protocol) es un protocolo de comunicación utilizado para la transferencia de datos en la web. 

GET: Solicita datos al servidor.

POST: Envia datos al servidor.

PUT: Actualiza datos existentes en el servidor.

DELETE: Elimina datos del servidor.

4- ¿Qué es un archivo JSON y para qué se utiliza?

JSON (JavaScript Object Notation) es un formato de intercambio de datos basado en texto, ligero y fácil de leer. Se utiliza comúnmente para enviar datos entre un servidor y un cliente, especialmente en APIs.

5- ¿Qué es una base de datos relacional? Da ejemplos de sistemas que la utilizan.

Una base de datos relacional almacena datos en tablas estructuradas con filas y columnas. Los sistemas de bases de datos como MySQL, PostgreSQL y SQLite son ejemplos de bases de datos relacionales.

6- ¿Qué es SQL?

SQL (Structured Query Language) es un lenguaje de programación utilizado para gestionar bases de datos relacionales. Permite realizar operaciones como la consulta, inserción, actualización y eliminación de datos.

7- Explicame qué es una consulta SQL simple (SELECT, WHERE).

SELECT se usa para recuperar datos de una base de datos. WHERE se usa para filtrar los registros según una condición. Ejemplo: SELECT * FROM usuarios WHERE edad > 18; recupera todos los usuarios cuya edad sea mayor a 18.

8- ¿Qué es un CRUD y por qué es importante en el backend?

CRUD es un acrónimo de Crear, Leer, Actualizar y Eliminar. Son las operaciones básicas que puedes realizar sobre los datos en una base de datos. Son fundamentales en el backend, ya que permiten manipular y gestionar la información de manera eficiente.

9- ¿Qué es el versionado de control? ¿Qué herramientas conocés para ello?

El versionado de control es el proceso de gestionar los cambios en el código fuente de un proyecto. Herramientas populares incluyen Git y plataformas como GitHub y GitLab.

10- ¿Qué es un framework y por qué se utiliza? Menciona algunos frameworks populares para backend.

Un framework es un conjunto de herramientas, bibliotecas y convenciones que facilita el desarrollo de aplicaciones. Se utiliza para agilizar el desarrollo y garantizar la coherencia en el código. Algunos ejemplos son Django (Python), Express (Node.js) y Spring (Java).

Nivel Intermedio

Las preguntas de este nivel se centran en tu capacidad para trabajar con tecnologías más complejas y aplicar conceptos de manera eficiente.

11- ¿Qué es una base de datos NoSQL y cuándo es más conveniente usarla?

Las bases de datos NoSQL son bases de datos no relacionales que permiten almacenar datos en estructuras más flexibles como documentos, clave-valor, columnas o grafos. Son útiles cuando se necesita escalar horizontalmente o manejar grandes volúmenes de datos no estructurados. Ejemplos: MongoDB y Cassandra.

12- ¿Qué es un middleware en una aplicación web?

Un middleware es un componente que se encuentra entre el servidor y el cliente y se encarga de procesar las solicitudes antes de que lleguen a la lógica de negocio o después de que se envíen de vuelta. Se utiliza para tareas como autenticación, manejo de errores o logging.

13- ¿Qué son las RESTful APIs y cómo las implementas?

Las RESTful APIs son APIs basadas en los principios de la arquitectura REST (Representational State Transfer), que utilizan los métodos HTTP para interactuar con recursos a través de URLs. Se implementan siguiendo convenciones como usar GET para obtener datos, POST para crear, PUT/PATCH para actualizar, y DELETE para eliminar.

14- ¿Qué son los códigos de estado HTTP y cómo los gestionás en tu aplicación?

Los códigos de estado HTTP son números que indican el resultado de una solicitud realizada por un cliente (como un navegador) al servidor. Estos códigos ayudan a identificar si la solicitud fue exitosa o si ocurrió algún error. Algunos ejemplos comunes son:

200 OK: La solicitud fue exitosa y el servidor ha devuelto la respuesta correcta.

404 Not Found: El recurso solicitado no se encuentra en el servidor.

500 Internal Server Error: Ocurrió un error inesperado en el servidor.

15- Explícame qué son los índices en bases de datos y por qué se usan.

Los índices en bases de datos son estructuras que mejoran la velocidad de las consultas. Permiten encontrar datos de manera más eficiente, pero pueden afectar el rendimiento en las operaciones de inserción y actualización.

16- ¿Qué es la autenticación y la autorización? Explicá la diferencia.

Autenticación: Proceso de verificar la identidad de un usuario (por ejemplo, a través de un nombre de usuario y contraseña). Autorización: Proceso de otorgar permisos al usuario para realizar ciertas acciones en el sistema (por ejemplo, acceso a ciertos recursos o acciones).

17- ¿Cómo gestionás el manejo de errores en una API?

El manejo de errores en una API se realiza mediante respuestas adecuadas y códigos de estado HTTP. Se pueden devolver mensajes de error claros con el código de estado correspondiente para ayudar al cliente a entender el problema.

18- Explícame qué son las transacciones en bases de datos y cómo las utilizás.

Una transacción es un conjunto de operaciones que se realizan como una unidad. Se utiliza para asegurar que los datos permanezcan consistentes, incluso si algo sale mal. Se utilizan comandos como BEGIN, COMMIT y ROLLBACK en SQL para controlar las transacciones.

19- ¿Qué es un patrón de diseño como el Singleton y cómo lo implementas?

El patrón Singleton asegura que una clase tenga solo una instancia durante la ejecución de una aplicación y proporciona un punto de acceso global a esa instancia. Se implementa restringiendo la creación de instancias adicionales y proporcionando un método estático para acceder a la instancia única.

20- ¿Cómo optimizarías una consulta SQL que está tardando demasiado?

Se pueden usar varias técnicas, como la creación de índices, optimización de las consultas JOIN, uso de subconsultas eficientes, y limitación de los resultados mediante paginación.

Nivel Avanzado

Este nivel evalúa tu comprensión de arquitecturas complejas, optimización de rendimiento y habilidades para resolver problemas de alto nivel.

21- ¿Cómo escalarías una aplicación de microservicios para soportar millones de usuarios?

Para escalar una aplicación de microservicios, se usarían técnicas como escala horizontal (añadir más instancias de los servicios), balanceo de carga, cachés distribuidos, y herramientas como Kubernetes para gestionar el ciclo de vida de los contenedores y asegurar la disponibilidad.

22- ¿Qué es la consistencia eventual y cuándo la usarías?

La consistencia eventual es un modelo de consistencia en el que las actualizaciones de los datos se propagan gradualmente, sin garantizar que todos los nodos estén actualizados inmediatamente. Se usa en sistemas distribuidos que requieren alta disponibilidad y tolerancia a fallos, como en Cassandra o Amazon DynamoDB.

23- ¿Cómo implementarías un sistema de caché para mejorar el rendimiento de una API?

Se podría implementar un caché en el back-end utilizando herramientas como Redis o Memcached para almacenar temporalmente respuestas frecuentes o datos pesados. Esto reduce la carga en las bases de datos y mejora la velocidad de respuesta.

24- ¿Qué son los WebSockets y en qué casos los utilizarías?

Los WebSockets permiten una comunicación bidireccional en tiempo real entre el cliente y el servidor. Se usan en aplicaciones donde se necesita una interacción continua y en tiempo real, como en chats en línea o juegos multiplayer.

25- Explicame la diferencia entre escalabilidad horizontal y vertical.

Escalabilidad vertical: Aumentar los recursos (CPU, RAM) de un único servidor. Escalabilidad horizontal: Añadir más servidores o instancias para distribuir la carga.

26- ¿Qué son las colas de mensajes y cómo las implementas en una arquitectura de microservicios?

Las colas de mensajes permiten la comunicación asíncrona entre servicios. Se utilizan para enviar mensajes entre componentes sin que estén directamente conectados. Herramientas como RabbitMQ y Kafka son comunes para implementarlas.

27- Explícame cómo manejarías el versionado de una API.

El versionado de una API se puede hacer mediante el uso de rutas específicas, como api/v1/resource. Se pueden utilizar headers o query parameters para indicar la versión de la API solicitada.

28- ¿Qué es un Deadlock y cómo lo evitarías?

Un Deadlock ocurre cuando dos o más procesos esperan indefinidamente por recursos que están siendo utilizados por otros. Se puede evitar mediante el uso de algoritmos de control de concurrencia o estableciendo reglas para adquirir los recursos en un orden específico.

29- ¿Qué técnicas de optimización utilizarías para mejorar el rendimiento de una base de datos de alto tráfico?

Se pueden usar técnicas como la desnormalización, indexación adecuada, caché de consultas frecuentes, particionado de bases de datos, y sharding para distribuir los datos en varios servidores.

30- ¿Cómo manejarías un sistema distribuido con múltiples bases de datos sincrónicas y asincrónicas?

Se utilizaría un enfoque de eventual consistency para las bases de datos asincrónicas y se garantizaría que la sincronización de los datos entre bases de datos sea manejada por eventos o colas de mensajes, asegurando que todas las bases de datos estén actualizadas sin afectar el rendimiento.
