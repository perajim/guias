# Parte 4 — Servicios de Cómputo — Preguntas tipo examen

20 preguntas de opción múltiple, sin respuestas marcadas, para autoevaluación.

**Pregunta 1.** Una empresa necesita ejecutar una aplicación con control total sobre el sistema operativo, incluyendo software legado que requiere configuraciones muy específicas. ¿Qué servicio de cómputo de AWS es el más adecuado?

- A) AWS Lambda
- B) Amazon EC2
- C) AWS Fargate
- D) Amazon Lightsail exclusivamente

**Pregunta 2.** ¿Qué es una AMI (Amazon Machine Image)?

- A) Un tipo de instancia EC2 de alto rendimiento
- B) Una plantilla que contiene la configuración necesaria para lanzar una instancia EC2 (sistema operativo, software preinstalado, configuraciones)
- C) Un servicio de monitoreo de instancias EC2
- D) El nombre del hipervisor de AWS

**Pregunta 3.** ¿Qué función cumple un Security Group en AWS?

- A) Es un firewall a nivel de subred que opera con reglas allow y deny
- B) Es un firewall virtual a nivel de instancia que controla el tráfico entrante y saliente, y solo permite reglas de tipo 'Allow'
- C) Es un servicio de balanceo de carga
- D) Es un tipo de rol de IAM

**Pregunta 4.** Una aplicación web experimenta picos de tráfico impredecibles durante el día. La empresa quiere que el número de instancias EC2 aumente y disminuya automáticamente según la demanda real. ¿Qué servicio resuelve esto?

- A) AWS Lambda exclusivamente
- B) Amazon EC2 Auto Scaling
- C) Amazon Lightsail
- D) AWS Batch

**Pregunta 5.** ¿Qué componente de AWS distribuye el tráfico entrante entre múltiples instancias EC2 en diferentes Availability Zones para mejorar la disponibilidad?

- A) Amazon Route 53 exclusivamente
- B) Elastic Load Balancer (ELB)
- C) AWS Direct Connect
- D) Amazon CloudFront exclusivamente

**Pregunta 6.** Una empresa necesita ejecutar código solo cuando ocurre un evento específico (por ejemplo, un archivo subido a S3), sin mantener ningún servidor corriendo el resto del tiempo. ¿Qué servicio es el más adecuado?

- A) Amazon EC2
- B) AWS Lambda
- C) Amazon Lightsail
- D) AWS Batch

**Pregunta 7.** ¿Cuál es la diferencia principal entre Amazon ECS y Amazon EKS?

- A) No hay diferencia, son el mismo servicio con distinto nombre
- B) ECS es el orquestador de contenedores propio de AWS; EKS es un servicio administrado de Kubernetes, el estándar open source de orquestación
- C) ECS solo funciona con Fargate; EKS solo funciona con EC2
- D) EKS es exclusivamente para bases de datos

**Pregunta 8.** ¿Qué es AWS Fargate?

- A) Un tipo de instancia EC2 optimizada para cómputo
- B) Un motor de cómputo serverless para contenedores, usado con ECS o EKS, que elimina la necesidad de administrar servidores o clústeres de EC2 subyacentes
- C) Un servicio de almacenamiento de imágenes de contenedores
- D) Un servicio de bases de datos NoSQL

**Pregunta 9.** Una pequeña empresa quiere desplegar un sitio web WordPress de forma simple, sin tener que configurar VPC, subnets, ni Security Groups manualmente, con precios predecibles mensuales. ¿Qué servicio de AWS es el más adecuado?

- A) Amazon EKS
- B) AWS Batch
- C) Amazon Lightsail
- D) AWS Outposts

**Pregunta 10.** Un laboratorio de investigación necesita procesar miles de trabajos de cómputo por lotes (batch) de forma eficiente, sin gestionar manualmente la cola de trabajos ni la asignación de recursos de cómputo. ¿Qué servicio es el más adecuado?

- A) AWS Batch
- B) Amazon Lightsail
- C) AWS Lambda exclusivamente para todos los trabajos sin importar duración
- D) Amazon Route 53

**Pregunta 11.** ¿Cuál de las siguientes opciones describe mejor cuándo usar EC2 en lugar de Lambda?

- A) Cuando la carga de trabajo es esporádica y de corta duración
- B) Cuando se necesita control total del sistema operativo, o cargas de trabajo de larga duración y predecibles que no encajan en el límite de tiempo de ejecución de Lambda
- C) Lambda siempre es mejor opción que EC2 en cualquier escenario
- D) EC2 no puede ejecutar aplicaciones web

**Pregunta 12.** ¿Qué son los 'tipos de instancia' de EC2 (como t3.micro, m5.large, c5.xlarge)?

- A) Nombres de las Availability Zones donde se puede lanzar la instancia
- B) Combinaciones predefinidas de capacidad de CPU, memoria, almacenamiento y red, optimizadas para distintos casos de uso (general purpose, compute optimized, memory optimized, etc.)
- C) El nombre del sistema operativo instalado
- D) El nivel de soporte técnico contratado

**Pregunta 13.** Una aplicación en contenedores necesita ejecutarse en AWS, y el equipo NO quiere administrar ningún servidor EC2 subyacente ni preocuparse por parchear el sistema operativo del clúster. ¿Qué combinación de servicios es la más adecuada?

- A) ECS o EKS ejecutándose sobre EC2 tradicional
- B) ECS o EKS ejecutándose sobre AWS Fargate
- C) Solamente Lambda, sin usar contenedores
- D) AWS Batch exclusivamente

**Pregunta 14.** ¿Qué diferencia a un Security Group de una Network ACL (NACL) en cuanto al tipo de reglas que admite?

- A) Ambos solo admiten reglas Allow
- B) El Security Group solo admite reglas Allow (stateful); la NACL admite reglas Allow y Deny (stateless), y opera a nivel de subred
- C) La NACL solo admite reglas Allow; el Security Group admite Allow y Deny
- D) No hay diferencia entre ambos

**Pregunta 15.** Una startup quiere reducir el costo de sus cargas de trabajo de procesamiento por lotes que pueden interrumpirse y reanudarse sin problema. ¿Qué tipo de instancia EC2 le conviene combinar con AWS Batch para maximizar el ahorro?

- A) Instancias On-Demand exclusivamente
- B) Instancias Reservadas a 3 años
- C) Instancias Spot
- D) Instancias dedicadas (Dedicated Hosts)

**Pregunta 16.** ¿Qué es un Auto Scaling Group (ASG)?

- A) Un tipo de balanceador de carga
- B) Una colección lógica de instancias EC2 que se gestionan de forma conjunta, con reglas de escalado automático definidas (mínimo, máximo, deseado)
- C) Un servicio de almacenamiento elástico
- D) Un tipo de Security Group especial

**Pregunta 17.** Un ELB detecta que una de las tres instancias EC2 detrás de él está fallando las verificaciones de salud (health checks). ¿Qué hace el ELB en ese caso?

- A) Detiene el envío de tráfico a esa instancia específica hasta que vuelva a pasar las verificaciones de salud, y sigue distribuyendo el tráfico entre las instancias saludables restantes
- B) Apaga automáticamente toda la aplicación
- C) Envía más tráfico a esa instancia para forzar su recuperación
- D) Elimina permanentemente esa instancia sin posibilidad de recuperación

**Pregunta 18.** ¿Cuál de los siguientes servicios de cómputo de AWS tiene un modelo de precios basado principalmente en 'pago por invocación y tiempo de ejecución', sin cobrar nada mientras el código no se ejecuta?

- A) Amazon EC2 On-Demand
- B) Amazon Lightsail
- C) AWS Lambda
- D) Amazon EKS con nodos EC2

**Pregunta 19.** Un equipo de DevOps con amplia experiencia previa en Kubernetes on-premises está migrando sus cargas de trabajo en contenedores a AWS y quiere mantener la mayor compatibilidad posible con sus manifiestos y herramientas de Kubernetes existentes. ¿Qué servicio de AWS es el más adecuado?

- A) Amazon ECS
- B) Amazon EKS
- C) AWS Lambda
- D) Amazon Lightsail Containers exclusivamente

**Pregunta 20.** Una empresa de comercio electrónico despliega su aplicación web en instancias EC2 dentro de un Auto Scaling Group repartido en tres Availability Zones, detrás de un Application Load Balancer. ¿Qué combinación de conceptos de arquitectura está aplicando principalmente?

- A) Solo elasticidad, sin alta disponibilidad
- B) Elasticidad (Auto Scaling) y alta disponibilidad (múltiples AZ + Load Balancer)
- C) Solo tolerancia a fallos, sin elasticidad
- D) Ninguno de estos conceptos aplica a esta arquitectura
