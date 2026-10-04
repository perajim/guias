# Parte 10 — Integración — Preguntas tipo examen

19 preguntas de opción múltiple, sin respuestas marcadas, para autoevaluación.

**Pregunta 1.** Una aplicación de procesamiento de pedidos quiere desacoplar el servicio que recibe pedidos del servicio que los procesa, de forma que si el procesador está temporalmente saturado o caído, los pedidos no se pierdan y se procesen tan pronto como esté disponible de nuevo. ¿Qué servicio de AWS resuelve esto directamente?

- A) Amazon SNS
- B) Amazon SQS
- C) AWS Step Functions
- D) Amazon API Gateway

**Pregunta 2.** ¿Cuál es la diferencia fundamental entre Amazon SQS y Amazon SNS en cuanto al patrón de mensajería?

- A) Son el mismo servicio con nombres distintos
- B) SQS es un modelo de colas (un mensaje es consumido típicamente por un solo consumidor, punto a punto); SNS es un modelo de publicación/suscripción (un mensaje se entrega a MÚLTIPLES suscriptores simultáneamente)
- C) SNS solo funciona con Lambda; SQS solo funciona con EC2
- D) SQS es de pago; SNS es siempre gratuito

**Pregunta 3.** Una empresa necesita notificar simultáneamente a tres sistemas distintos (un correo al equipo de soporte, una función Lambda que actualiza un dashboard, y una cola SQS para procesamiento posterior) cada vez que ocurre un evento específico. ¿Qué servicio de AWS es el más adecuado para distribuir ese único evento a los tres destinos?

- A) Amazon SQS exclusivamente
- B) Amazon SNS, publicando el evento a un tópico con los tres suscriptores configurados
- C) AWS Step Functions exclusivamente
- D) Amazon Route 53

**Pregunta 4.** ¿Qué es Amazon EventBridge?

- A) Un servicio de colas de mensajes simple
- B) Un bus de eventos serverless que permite conectar aplicaciones usando datos de eventos desde fuentes de AWS, aplicaciones propias del cliente, y aplicaciones SaaS de terceros, con capacidad de enrutamiento basado en reglas
- C) Un servicio exclusivo de bases de datos
- D) Un tipo de instancia EC2

**Pregunta 5.** Una aplicación necesita orquestar un flujo de trabajo de varios pasos (validar pago, reservar inventario, notificar al almacén, enviar confirmación), donde cada paso depende del resultado del anterior y se necesita manejar reintentos y errores de forma visual y estructurada. ¿Qué servicio de AWS es el más adecuado?

- A) Amazon SQS
- B) AWS Step Functions
- C) Amazon SNS
- D) Amazon Route 53

**Pregunta 6.** ¿Qué es Amazon API Gateway?

- A) Un servicio de bases de datos NoSQL
- B) Un servicio totalmente administrado para crear, publicar, mantener, monitorear y proteger APIs REST, HTTP y WebSocket a cualquier escala
- C) Un tipo de Load Balancer exclusivo para tráfico interno
- D) Un servicio de almacenamiento de objetos

**Pregunta 7.** Una arquitectura serverless típica combina API Gateway con AWS Lambda. ¿Qué rol cumple API Gateway en esa combinación?

- A) Ejecuta el código de negocio de la aplicación
- B) Actúa como la puerta de entrada HTTP que recibe las peticiones de los clientes y las enruta hacia la función Lambda correspondiente, gestionando autenticación y límites de tasa
- C) Almacena los datos de la aplicación de forma persistente
- D) Reemplaza la necesidad de usar IAM

**Pregunta 8.** ¿Qué característica de Amazon SQS ayuda a evitar que un mensaje se pierda si el consumidor falla justo después de recibirlo pero antes de procesarlo completamente?

- A) El mensaje se elimina automáticamente e irrecuperablemente al ser recibido
- B) El periodo de visibilidad (visibility timeout): el mensaje se oculta temporalmente a otros consumidores tras ser recibido, pero vuelve a estar disponible en la cola si no se elimina explícitamente dentro de ese periodo
- C) SQS reenvía automáticamente el mensaje por correo electrónico como respaldo
- D) No existe ningún mecanismo de este tipo en SQS

**Pregunta 9.** ¿Qué es una Dead Letter Queue (DLQ) en el contexto de Amazon SQS?

- A) Una cola que elimina automáticamente todos los mensajes tras 1 hora
- B) Una cola secundaria hacia donde se envían automáticamente los mensajes que han fallado su procesamiento repetidamente, para su análisis posterior sin bloquear la cola principal
- C) Un tipo de instancia EC2
- D) Un sinónimo de Amazon SNS

**Pregunta 10.** Una empresa quiere reaccionar automáticamente cada vez que se crea una nueva instancia EC2 en su cuenta, sin importar si esa instancia fue creada manualmente, por un script, o por Auto Scaling, y enrutar ese evento según reglas de negocio hacia distintos destinos. ¿Qué servicio encaja mejor con este requisito de enrutamiento flexible basado en el contenido del evento?

- A) Amazon SQS exclusivamente
- B) Amazon EventBridge, usando una regla que capture eventos de EC2 y los enrute según su contenido
- C) AWS Step Functions exclusivamente
- D) Amazon Route 53

**Pregunta 11.** ¿Cuál de las siguientes NO es una fuente típica de eventos que puede recibir Amazon EventBridge?

- A) Servicios nativos de AWS (como EC2, S3)
- B) Aplicaciones propias del cliente, mediante eventos personalizados
- C) Aplicaciones SaaS de terceros integradas como fuentes de eventos
- D) Únicamente eventos generados manualmente por soporte de AWS

**Pregunta 12.** ¿Qué ventaja ofrece AWS Step Functions frente a coordinar manualmente una secuencia de invocaciones de Lambda escribiendo el código de orquestación dentro de una única función Lambda 'controladora'?

- A) Step Functions es siempre más económico en cualquier escenario, sin excepción
- B) Step Functions ofrece una representación visual del flujo, manejo nativo de reintentos y captura de errores por paso, y evita construir y mantener lógica de orquestación compleja dentro del código de una sola función
- C) Step Functions elimina la necesidad de usar Lambda por completo
- D) No existe ninguna ventaja real

**Pregunta 13.** Una aplicación pública necesita proteger su API contra un cliente que envía peticiones excesivamente rápido, degradando el servicio para otros usuarios. ¿Qué funcionalidad de Amazon API Gateway ayuda a mitigar esto?

- A) Versionado de API exclusivamente
- B) Throttling (limitación de tasa de peticiones), configurable a nivel de cuenta, API o cliente individual
- C) Amazon SNS integrado
- D) AWS Step Functions

**Pregunta 14.** ¿Qué tipo de arquitectura describe mejor una aplicación que usa SQS entre un servicio productor y un servicio consumidor, en vez de que el productor llame directamente al consumidor?

- A) Arquitectura fuertemente acoplada (tightly coupled)
- B) Arquitectura desacoplada (decoupled), donde los componentes no dependen de la disponibilidad inmediata del otro para funcionar
- C) Arquitectura monolítica
- D) Arquitectura sin estado exclusivamente para bases de datos

**Pregunta 15.** Una aplicación de e-commerce quiere enviar una notificación por SMS al cliente Y simultáneamente encolar el pedido para su procesamiento en backend, a partir de un único evento de 'pedido confirmado'. ¿Qué combinación de servicios de integración resolvería esto de forma nativa?

- A) Un tópico de Amazon SNS con dos suscriptores: un número de SMS y una cola SQS
- B) Solamente Amazon SQS, sin ningún otro servicio
- C) AWS Step Functions exclusivamente, sin SNS ni SQS
- D) Amazon Route 53 exclusivamente

**Pregunta 16.** ¿Qué sucede con un mensaje en una cola SQS estándar (no FIFO) en cuanto al orden de entrega y la posibilidad de duplicados?

- A) Garantiza orden estricto y entrega exactamente una vez, siempre
- B) No garantiza un orden estricto de entrega, y es posible (aunque poco frecuente) que un mensaje se entregue más de una vez (at-least-once delivery)
- C) Elimina automáticamente los mensajes duplicados sin configuración adicional
- D) Solo permite un mensaje en la cola a la vez

**Pregunta 17.** ¿Qué combinación de servicios describe una arquitectura serverless típica para exponer una API pública que ejecuta lógica de negocio sin servidores?

- A) Amazon API Gateway recibiendo peticiones HTTP y enrutándolas hacia funciones AWS Lambda
- B) Amazon EC2 exclusivamente, sin ningún otro servicio
- C) Amazon Redshift conectado directamente a internet
- D) AWS Direct Connect exclusivamente

**Pregunta 18.** Un proceso de aprobación de préstamos bancarios involucra varios pasos secuenciales con posibles ramificaciones (verificación de crédito, aprobación manual si el monto supera cierto umbral, notificación final), y el equipo quiere poder visualizar en qué paso exacto se encuentra cada solicitud en curso. ¿Qué servicio de AWS ofrece esa visualización nativa del estado del flujo?

- A) Amazon SQS
- B) AWS Step Functions, con su representación visual de la máquina de estados
- C) Amazon SNS
- D) Amazon CloudFront

**Pregunta 19.** ¿Cuál de las siguientes NO es una razón típica para elegir Amazon EventBridge sobre Amazon SNS en un escenario de integración de eventos?

- A) Se necesita filtrar y enrutar eventos según reglas complejas basadas en el contenido del evento
- B) Se necesita integrar eventos provenientes de aplicaciones SaaS de terceros de forma nativa
- C) Se necesita almacenar archivos de gran tamaño como parte del evento, sin ningún límite práctico de tamaño
- D) Se necesita un bus de eventos centralizado que conecte múltiples fuentes con múltiples destinos de forma desacoplada
