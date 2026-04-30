kafka:
            producer:
              properties:
                linger.ms: 20
                batch.size: 900000
                buffer.memory: 13430000217728
                request.timeout.ms: 30000
                delivery.timeout.ms: 120000
                max.block.ms: 90000
