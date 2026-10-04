# AWS Certified Cloud Practitioner (CLF-C02)

**Simulacro de Examen 1 de 5 — 65 preguntas**

Mismo nivel de dificultad y distribución de dominios que el examen oficial CLF-C02: Cloud Concepts, Security and Compliance, Cloud Technology and Services, y Billing and Pricing. Cada pregunta incluye la respuesta correcta, una explicación, y una referencia al capítulo de la guía donde puedes repasar el tema si fallaste.

> **Cómo usar este simulacro:** Resuélvelo primero completo, sin mirar las respuestas, cronometrando 90 minutos como en el examen real. Después revisa cada pregunta, prestando especial atención a las que fallaste, y repasa el capítulo referenciado antes de tu siguiente simulacro.

## Preguntas

**Pregunta 1.** Una empresa quiere convertir el gasto de capital (comprar servidores por adelantado) en gasto operativo (pagar por uso). ¿Qué beneficio del cloud computing describe esto?

A) Elasticidad

**B)** **Trade CAPEX for OPEX**

C) Alta disponibilidad

D) Tolerancia a fallos

**Respuesta correcta: B.** 

*Este es uno de los seis beneficios de negocio que AWS cita explícitamente: transformar inversión de capital por adelantado en gasto operativo variable según el uso real.*

Referencia: Parte 1

**Pregunta 2.** ¿Qué modelo de servicio en la nube entrega una aplicación completa lista para usar, sin que el cliente administre infraestructura ni código?

A) IaaS

B) PaaS

**C)** **SaaS**

D) FaaS

**Respuesta correcta: C.** 

*SaaS (Software as a Service) entrega software funcional y terminado; el cliente solo lo usa, como Gmail o Amazon Chime.*

Referencia: Parte 1

**Pregunta 3.** Una aplicación aumenta y disminuye automáticamente su capacidad de cómputo según la demanda real, sin intervención manual. ¿Qué concepto describe esto?

A) Escalabilidad únicamente

**B)** **Elasticidad**

C) Tolerancia a fallos

D) Recuperación ante desastres

**Respuesta correcta: B.** 

*Elasticidad es escalabilidad + automatismo + reversibilidad: el sistema crece y decrece solo según la demanda.*

Referencia: Parte 1

**Pregunta 4.** ¿Qué es una Availability Zone?

A) Un país donde AWS tiene oficinas

**B)** **Uno o más data centers discretos dentro de una Región, con energía y red independientes**

C) Un punto de presencia para CloudFront

D) Un tipo de instancia EC2

**Respuesta correcta: B.** 

*Una AZ es un conjunto de data centers físicamente aislados pero interconectados con baja latencia dentro de una misma Región.*

Referencia: Parte 2

**Pregunta 5.** ¿Qué elemento de una IAM Policy determina si una acción se permite o se deniega?

A) Resource

B) Action

**C)** **Effect**

D) Version

**Respuesta correcta: C.** 

*El elemento 'Effect' toma el valor 'Allow' o 'Deny' y determina el resultado de esa declaración de la policy.*

Referencia: Parte 3

**Pregunta 6.** Si una policy otorga acceso completo a S3 pero otra policy deniega explícitamente el acceso a un bucket específico, ¿qué prevalece?

A) El Allow, porque es más permisivo

**B)** **El Deny explícito siempre prevalece**

C) AWS pide confirmación manual

D) Depende del orden de creación de las policies

**Respuesta correcta: B.** 

*Un Deny explícito siempre prevalece sobre cualquier Allow, sin importar cuántas policies otorguen el permiso.*

Referencia: Parte 3

**Pregunta 7.** Una aplicación en EC2 necesita leer de un bucket S3 sin almacenar credenciales en el código. ¿Qué debería usarse?

A) Un IAM User con access keys embebidas en el código

**B)** **Un IAM Role asociado a la instancia (Instance Profile)**

C) Hacer el bucket público

D) Las credenciales del usuario root

**Respuesta correcta: B.** 

*Un IAM Role asociado a la instancia entrega credenciales temporales automáticamente, sin necesidad de almacenar ninguna credencial permanente en el código.*

Referencia: Parte 3

**Pregunta 8.** ¿Qué servicio de AWS permite ejecutar código en respuesta a eventos, sin administrar servidores?

A) Amazon EC2

**B)** **AWS Lambda**

C) Amazon Lightsail

D) AWS Batch

**Respuesta correcta: B.** 

*Lambda ejecuta funciones en respuesta a eventos (como un archivo subido a S3), cobrando solo por invocación y tiempo de ejecución.*

Referencia: Parte 4

**Pregunta 9.** ¿Qué componente distribuye el tráfico entrante entre múltiples instancias EC2 en distintas Availability Zones?

A) NAT Gateway

**B)** **Elastic Load Balancer**

C) Internet Gateway

D) AWS Direct Connect

**Respuesta correcta: B.** 

*El Elastic Load Balancer reparte el tráfico entre instancias saludables en una o más AZ, mejorando disponibilidad y capacidad.*

Referencia: Parte 4

**Pregunta 10.** ¿Qué diferencia principal existe entre un Security Group y una Network ACL?

A) Son idénticos

**B)** **El Security Group es stateful y solo permite Allow; la NACL es stateless y permite Allow y Deny**

C) La NACL es stateful; el Security Group es stateless

D) Ambos operan solo a nivel de subred

**Respuesta correcta: B.** 

*Security Group = instancia, stateful, solo Allow. NACL = subred, stateless, Allow y Deny.*

Referencia: Parte 4 y 7

**Pregunta 11.** ¿Qué clase de almacenamiento de S3 es la más económica, con tiempos de recuperación de hasta 12 horas?

A) S3 Standard

B) S3 Standard-IA

**C)** **S3 Glacier Deep Archive**

D) S3 Intelligent-Tiering

**Respuesta correcta: C.** 

*S3 Glacier Deep Archive ofrece el costo por GB más bajo de S3, a cambio de tiempos de recuperación de varias horas.*

Referencia: Parte 5

**Pregunta 12.** ¿Qué servicio de almacenamiento se comporta como un disco duro virtual, adjunto típicamente a una sola instancia EC2?

A) Amazon S3

**B)** **Amazon EBS**

C) Amazon EFS

D) AWS Storage Gateway

**Respuesta correcta: B.** 

*Amazon EBS entrega volúmenes en bloque persistentes que se adjuntan a una instancia EC2, viviendo dentro de una AZ específica.*

Referencia: Parte 5

**Pregunta 13.** ¿Qué servicio permite montar un mismo sistema de archivos simultáneamente desde múltiples instancias EC2 en distintas AZ?

A) Amazon EBS

**B)** **Amazon EFS**

C) AWS Snowball

D) Amazon Redshift

**Respuesta correcta: B.** 

*Amazon EFS es un sistema de archivos NFS compartido, montable simultáneamente por múltiples instancias en distintas AZ.*

Referencia: Parte 5

**Pregunta 14.** Una aplicación necesita latencia de un solo dígito de milisegundos a cualquier escala, con un modelo de datos clave-valor. ¿Qué base de datos es la más adecuada?

A) Amazon RDS

**B)** **Amazon DynamoDB**

C) Amazon Redshift

D) Amazon Neptune

**Respuesta correcta: B.** 

*DynamoDB está diseñado específicamente para latencia mínima y consistente a cualquier escala con un modelo clave-valor.*

Referencia: Parte 6

**Pregunta 15.** ¿Qué servicio de AWS está optimizado para consultas analíticas complejas (OLAP) sobre grandes volúmenes de datos históricos?

A) Amazon Aurora

**B)** **Amazon Redshift**

C) Amazon DynamoDB

D) Amazon ElastiCache

**Respuesta correcta: B.** 

*Redshift es el data warehouse de AWS, optimizado para analítica sobre grandes volúmenes históricos, no para transacciones.*

Referencia: Parte 6

**Pregunta 16.** ¿Qué función cumple RDS Multi-AZ?

A) Escalar el tráfico de lecturas

**B)** **Mantener una réplica standby sincronizada en otra AZ con failover automático**

C) Reducir el costo de almacenamiento

D) Convertir la base de datos en NoSQL

**Respuesta correcta: B.** 

*Multi-AZ mantiene una réplica standby en otra AZ para alta disponibilidad, con conmutación automática ante fallo de la primaria.*

Referencia: Parte 6

**Pregunta 17.** ¿Qué hace que una subred sea considerada 'pública' dentro de una VPC?

A) Tener asignada una IP elástica

**B)** **Su tabla de rutas tiene una ruta hacia un Internet Gateway**

C) Estar en la primera Availability Zone

D) Tener un Security Group vacío

**Respuesta correcta: B.** 

*Una subred es pública porque su tabla de rutas incluye una ruta 0.0.0.0/0 hacia un Internet Gateway, no por ningún otro atributo.*

Referencia: Parte 7

**Pregunta 18.** ¿Qué componente permite que instancias en subredes privadas inicien conexiones salientes hacia internet sin ser accesibles desde fuera?

A) Internet Gateway

**B)** **NAT Gateway**

C) Network ACL

D) Route 53

**Respuesta correcta: B.** 

*El NAT Gateway, ubicado en una subred pública, permite tráfico saliente desde subredes privadas sin exponerlas a conexiones entrantes.*

Referencia: Parte 7

**Pregunta 19.** ¿Qué servicio ofrece una conexión de red física y dedicada entre un data center on-premises y AWS, sin pasar por internet público?

A) Site-to-Site VPN

**B)** **AWS Direct Connect**

C) Amazon CloudFront

D) AWS Transit Gateway exclusivamente

**Respuesta correcta: B.** 

*Direct Connect establece una conexión física dedicada, con mayor consistencia de ancho de banda y menor latencia que una VPN sobre internet.*

Referencia: Parte 7

**Pregunta 20.** Según el Modelo de Responsabilidad Compartida, ¿quién es responsable de parchear el sistema operativo de una instancia EC2?

A) AWS

**B)** **El cliente**

C) Ambos al 50%

D) Ningún responsable definido

**Respuesta correcta: B.** 

*En EC2 (IaaS), el cliente administra el sistema operativo, incluyendo sus parches; AWS es responsable de la infraestructura física subyacente.*

Referencia: Parte 8

**Pregunta 21.** ¿Qué servicio detecta actividad maliciosa o anómala en una cuenta de AWS usando machine learning, sin requerir agentes?

A) Amazon Inspector

**B)** **Amazon GuardDuty**

C) Amazon Macie

D) AWS Config

**Respuesta correcta: B.** 

*GuardDuty analiza continuamente CloudTrail, VPC Flow Logs y DNS para detectar comportamiento anómalo, sin requerir ningún agente.*

Referencia: Parte 8

**Pregunta 22.** ¿Qué servicio descubre y clasifica automáticamente datos sensibles almacenados en buckets S3?

**A)** **Amazon Macie**

B) Amazon Inspector

C) AWS Shield

D) AWS WAF

**Respuesta correcta: A.** 

*Macie usa machine learning para identificar datos sensibles (como PII) mal protegidos en S3.*

Referencia: Parte 8

**Pregunta 23.** ¿Qué servicio registra un historial detallado de todas las llamadas a la API en una cuenta de AWS?

A) AWS Config

**B)** **AWS CloudTrail**

C) Amazon CloudWatch

D) AWS Trusted Advisor

**Respuesta correcta: B.** 

*CloudTrail registra quién hizo qué acción, cuándo y con qué parámetros, en toda la cuenta.*

Referencia: Parte 8

**Pregunta 24.** ¿Qué servicio permite rastrear el recorrido detallado de una solicitud individual a través de una arquitectura de microservicios distribuida?

A) Amazon CloudWatch

**B)** **AWS X-Ray**

C) AWS Trusted Advisor

D) AWS Health Dashboard

**Respuesta correcta: B.** 

*X-Ray genera trazas del recorrido de solicitudes individuales, mostrando en qué componente específico se origina la latencia.*

Referencia: Parte 9

**Pregunta 25.** ¿Qué herramienta ofrece recomendaciones en las categorías de costos, rendimiento, seguridad, tolerancia a fallos y límites de servicio?

**A)** **AWS Trusted Advisor**

B) AWS Health Dashboard

C) Amazon CloudWatch

D) AWS X-Ray

**Respuesta correcta: A.** 

*Trusted Advisor analiza la cuenta y ofrece recomendaciones en esas cinco categorías específicas.*

Referencia: Parte 9

**Pregunta 26.** ¿Qué servicio de AWS implementa el patrón de publicación/suscripción, entregando un mensaje a múltiples suscriptores simultáneamente?

A) Amazon SQS

**B)** **Amazon SNS**

C) AWS Step Functions

D) Amazon API Gateway

**Respuesta correcta: B.** 

*SNS distribuye un mensaje publicado a todos los suscriptores de un tópico de forma simultánea (fan-out).*

Referencia: Parte 10

**Pregunta 27.** ¿Qué servicio orquesta flujos de trabajo de múltiples pasos con manejo nativo de reintentos y errores?

A) Amazon SQS

**B)** **AWS Step Functions**

C) Amazon EventBridge

D) Amazon API Gateway

**Respuesta correcta: B.** 

*Step Functions coordina flujos de trabajo multi-paso como una máquina de estados visual, con reintentos y manejo de errores nativo.*

Referencia: Parte 10

**Pregunta 28.** ¿Qué herramienta permite analizar y visualizar el gasto histórico de una cuenta de AWS, filtrando por servicio o etiqueta?

A) AWS Budgets

**B)** **AWS Cost Explorer**

C) AWS Organizations

D) AWS Trusted Advisor

**Respuesta correcta: B.** 

*Cost Explorer es la herramienta de análisis retrospectivo de gasto, con filtros y pronósticos.*

Referencia: Parte 11

**Pregunta 29.** ¿Qué modelo de precios de EC2 ofrece hasta 90% de descuento frente a On-Demand, a cambio de que la instancia pueda ser interrumpida con poco aviso?

A) Reserved Instances

B) Savings Plans

**C)** **Spot Instances**

D) Dedicated Hosts

**Respuesta correcta: C.** 

*Las instancias Spot usan capacidad no utilizada de AWS con grandes descuentos, a cambio de posibles interrupciones con 2 minutos de aviso.*

Referencia: Parte 11

**Pregunta 30.** ¿Qué pilar del Well-Architected Framework se enfoca en recuperarse de fallos y satisfacer la demanda de forma consistente?

A) Excelencia Operacional

**B)** **Fiabilidad**

C) Sostenibilidad

D) Eficiencia del Rendimiento

**Respuesta correcta: B.** 

*El pilar de Fiabilidad abarca recuperación ante fallos, escalado dinámico y mitigación de errores de configuración o red.*

Referencia: Parte 12

**Pregunta 31.** ¿Qué servicio permite definir infraestructura de AWS de forma declarativa en archivos YAML o JSON?

A) AWS CDK exclusivamente

**B)** **AWS CloudFormation**

C) AWS Config

D) AWS Control Tower

**Respuesta correcta: B.** 

*CloudFormation aprovisiona infraestructura a partir de plantillas declarativas en JSON/YAML (Infrastructure as Code).*

Referencia: Parte 13

**Pregunta 32.** ¿Qué servicio se usaría para transferir 300 TB de datos hacia AWS cuando la conexión a internet disponible tardaría semanas?

A) AWS DataSync exclusivamente

**B)** **AWS Snowball**

C) AWS DMS

D) Amazon FSx

**Respuesta correcta: B.** 

*AWS Snowball es un dispositivo físico para transferencia masiva de datos, evitando el cuello de botella de una conexión lenta.*

Referencia: Parte 13

**Pregunta 33.** ¿Cuál de los siguientes es un ejemplo de nube híbrida?

A) Toda la infraestructura corriendo exclusivamente en AWS

**B)** **Una empresa que mantiene datos sensibles on-premises y usa AWS para picos de demanda**

C) Una infraestructura compartida entre varias empresas del mismo sector

D) Una infraestructura administrada exclusivamente por un tercero

**Respuesta correcta: B.** 

*La nube híbrida combina infraestructura on-premises con nube pública, comunicadas entre sí, como en el ejemplo de cloud bursting.*

Referencia: Parte 1

**Pregunta 34.** ¿Qué es una AMI?

A) Un tipo de Load Balancer

**B)** **Una plantilla que define el sistema operativo y software preinstalado de una instancia EC2**

C) Un servicio de monitoreo

D) Un tipo de base de datos

**Respuesta correcta: B.** 

*Una AMI (Amazon Machine Image) es la plantilla usada para lanzar instancias EC2 con una configuración específica.*

Referencia: Parte 4

**Pregunta 35.** ¿Qué es AWS Fargate?

A) Un orquestador de contenedores en sí mismo

**B)** **Un motor de cómputo serverless usado junto con ECS o EKS para no administrar servidores del clúster**

C) Un servicio de bases de datos

D) Un servicio de DNS

**Respuesta correcta: B.** 

*Fargate elimina la necesidad de administrar instancias EC2 subyacentes de un clúster ECS o EKS.*

Referencia: Parte 4

**Pregunta 36.** ¿Cuál es la diferencia principal entre Amazon ECS y Amazon EKS?

A) No hay diferencia

**B)** **ECS es el orquestador propio de AWS; EKS es Kubernetes administrado**

C) EKS solo funciona con Fargate

D) ECS es exclusivo para bases de datos

**Respuesta correcta: B.** 

*ECS es más simple y propietario de AWS; EKS ofrece compatibilidad total con el ecosistema estándar de Kubernetes.*

Referencia: Parte 4

**Pregunta 37.** ¿Qué beneficio ofrece principalmente S3 Versioning?

A) Reduce el costo de almacenamiento automáticamente

**B)** **Conserva versiones anteriores de un objeto, protegiendo contra sobrescritura o eliminación accidental**

C) Aumenta la velocidad de descarga

D) Cifra automáticamente todos los objetos

**Respuesta correcta: B.** 

*El versionado mantiene todas las versiones de un objeto, permitiendo restaurar cualquier versión anterior.*

Referencia: Parte 5

**Pregunta 38.** ¿Qué tipo de Storage Gateway presenta un sistema de archivos vía NFS o SMB hacia aplicaciones on-premises?

A) Volume Gateway

B) Tape Gateway

**C)** **File Gateway**

D) Snowball Gateway

**Respuesta correcta: C.** 

*File Gateway expone un sistema de archivos NFS/SMB, almacenando los datos como objetos en S3 de forma transparente.*

Referencia: Parte 5

**Pregunta 39.** ¿Qué servicio de AWS es un data warehouse totalmente administrado, usado para business intelligence?

A) Amazon RDS

**B)** **Amazon Redshift**

C) Amazon DynamoDB

D) Amazon Neptune

**Respuesta correcta: B.** 

*Redshift está optimizado para análisis de grandes volúmenes de datos históricos usando almacenamiento columnar.*

Referencia: Parte 6

**Pregunta 40.** ¿Qué servicio de base de datos es compatible con la API de MongoDB?

A) Amazon Aurora

**B)** **Amazon DocumentDB**

C) Amazon Neptune

D) Amazon ElastiCache

**Respuesta correcta: B.** 

*DocumentDB fue diseñado con compatibilidad con MongoDB para facilitar migraciones con cambios mínimos de código.*

Referencia: Parte 6

**Pregunta 41.** ¿Qué combinación de servicios describe la arquitectura serverless de referencia para exponer una API?

A) EC2 + RDS

**B)** **API Gateway + Lambda**

C) CloudFront + Route 53 exclusivamente

D) Redshift + QuickSight

**Respuesta correcta: B.** 

*API Gateway recibe las peticiones HTTP y las enruta hacia funciones Lambda que ejecutan la lógica de negocio.*

Referencia: Parte 10

**Pregunta 42.** ¿Qué es una Dead Letter Queue en SQS?

A) Una cola que elimina mensajes cada hora

**B)** **Una cola secundaria para mensajes que fallan su procesamiento repetidamente**

C) Un sinónimo de SNS

D) Un tipo de instancia EC2

**Respuesta correcta: B.** 

*Una DLQ recibe automáticamente mensajes que no pudieron procesarse tras varios intentos, evitando bloquear la cola principal.*

Referencia: Parte 10

**Pregunta 43.** ¿Qué diferencia a un Savings Plan de una Reserved Instance tradicional?

A) Son idénticos

**B)** **Savings Plan compromete un monto de gasto por hora, aplicado de forma más flexible al uso real**

C) Reserved Instance siempre es más barato en cualquier caso

D) Savings Plan no ofrece ningún descuento

**Respuesta correcta: B.** 

*Savings Plans comprometen gasto ($/hora) en vez de un tipo de instancia específico, aplicándose con más flexibilidad.*

Referencia: Parte 11

**Pregunta 44.** ¿Qué servicio de AWS centraliza la facturación de múltiples cuentas y permite aplicar Service Control Policies?

A) AWS Budgets

**B)** **AWS Organizations**

C) AWS Cost Explorer

D) AWS Backup

**Respuesta correcta: B.** 

*AWS Organizations ofrece facturación consolidada y gobernanza centralizada mediante SCPs sobre cuentas miembro.*

Referencia: Parte 11

**Pregunta 45.** ¿Qué pilar del Well-Architected Framework se añadió más recientemente a los cinco originales?

A) Seguridad

**B)** **Sostenibilidad**

C) Fiabilidad

D) Optimización de Costos

**Respuesta correcta: B.** 

*Sostenibilidad es el sexto pilar, enfocado en minimizar el impacto ambiental de las cargas de trabajo en la nube.*

Referencia: Parte 12

**Pregunta 46.** ¿Qué servicio replica continuamente servidores completos hacia AWS para recuperación ante desastres con RTO/RPO mínimos?

A) AWS Backup

**B)** **AWS Elastic Disaster Recovery**

C) AWS DataSync

D) AWS Migration Hub

**Respuesta correcta: B.** 

*AWS DRS replica servidores de forma continua, permitiendo lanzar instancias funcionales en AWS en minutos ante un desastre.*

Referencia: Parte 13

**Pregunta 47.** ¿Cuál de las siguientes NO es una característica esencial del cloud computing según la definición estándar?

A) Autoservicio bajo demanda

B) Elasticidad rápida

**C)** **Propiedad exclusiva del hardware por el cliente**

D) Servicio medido

**Respuesta correcta: C.** 

*La propiedad del hardware permanece en el proveedor de la nube; el cliente consume recursos, no es propietario del hardware físico.*

Referencia: Parte 1

**Pregunta 48.** ¿Qué son las Edge Locations de AWS?

A) Data centers completos para lanzar instancias EC2

**B)** **Puntos de presencia numerosos usados por CloudFront y Route 53 para reducir latencia**

C) Un sinónimo de Región

D) Oficinas comerciales de AWS

**Respuesta correcta: B.** 

*Las Edge Locations distribuyen contenido cacheado cerca del usuario final, no están pensadas para cómputo general.*

Referencia: Parte 2

**Pregunta 49.** ¿Qué es el principio de mínimo privilegio en IAM?

A) Otorgar acceso administrador a todos por defecto

**B)** **Otorgar solo los permisos estrictamente necesarios para cada tarea**

C) Usar siempre el usuario root

D) Nunca usar IAM Roles

**Respuesta correcta: B.** 

*El mínimo privilegio reduce la superficie de ataque otorgando solo los permisos necesarios, ni uno más.*

Referencia: Parte 3

**Pregunta 50.** ¿Qué servicio de AWS es ideal para desplegar un sitio WordPress simple con precios mensuales fijos y predecibles?

A) Amazon EKS

**B)** **Amazon Lightsail**

C) AWS Batch

D) Amazon Redshift

**Respuesta correcta: B.** 

*Lightsail simplifica el despliegue de aplicaciones sencillas con configuración de red simplificada y precio fijo.*

Referencia: Parte 4

**Pregunta 51.** ¿Qué servicio está diseñado para computación de alto rendimiento (HPC) y machine learning con integración directa a S3?

A) Amazon EFS

**B)** **Amazon FSx for Lustre**

C) AWS Storage Gateway

D) Amazon S3 Glacier

**Respuesta correcta: B.** 

*FSx for Lustre ofrece almacenamiento de altísimo rendimiento para cargas HPC y ML, con integración nativa a S3.*

Referencia: Parte 5

**Pregunta 52.** ¿Qué servicio de AWS proporciona una capa de caché en memoria compatible con Redis o Memcached?

**A)** **Amazon ElastiCache**

B) Amazon DynamoDB Accelerator exclusivamente

C) Amazon Redshift

D) AWS Batch

**Respuesta correcta: A.** 

*ElastiCache ofrece caché en memoria totalmente administrada, reduciendo la carga y latencia de la base de datos principal.*

Referencia: Parte 6

**Pregunta 53.** ¿Qué tipo de cola SQS garantiza orden estricto y entrega exactamente una vez dentro de un grupo de mensajes?

A) SQS Standard

**B)** **SQS FIFO**

C) SNS Standard

D) SNS FIFO exclusivamente para email

**Respuesta correcta: B.** 

*Las colas SQS FIFO garantizan orden y entrega exactamente una vez, a cambio de menor throughput que las Standard.*

Referencia: Parte 10

**Pregunta 54.** ¿Qué recurso de AWS es completamente gratuito de crear en cualquier cantidad, aunque sus acciones puedan generar costo en otros servicios?

A) Instancias EC2

**B)** **Usuarios, roles y policies de IAM**

C) Volúmenes EBS

D) Bases de datos RDS

**Respuesta correcta: B.** 

*IAM en sí mismo no tiene costo; el costo proviene de los recursos que esas identidades usan o crean.*

Referencia: Parte 11

**Pregunta 55.** ¿Qué combinación de AWS Backup y Elastic Disaster Recovery describe mejor su diferencia?

A) Son el mismo servicio

**B)** **Backup = copias periódicas de recursos individuales; DRS = replicación continua de servidores completos**

C) DRS es más barato que Backup en todos los casos

D) Backup no puede usarse con RDS

**Respuesta correcta: B.** 

*Backup resuelve '¿perdí este dato?'; DRS resuelve '¿mi entorno completo cayó, puedo seguir operando desde AWS?'.*

Referencia: Parte 13

**Pregunta 56.** ¿Qué elemento hace que un IAM Role sea más seguro que un IAM User con access keys permanentes, en el contexto de una aplicación en EC2?

A) El Role nunca expira y no requiere ninguna gestión

**B)** **Las credenciales del Role son temporales y se rotan automáticamente**

C) El Role tiene automáticamente permisos de administrador

D) No hay ninguna diferencia de seguridad real

**Respuesta correcta: B.** 

*Las credenciales de un Role son temporales (minutos a horas), reduciendo drásticamente la ventana de exposición ante una fuga.*

Referencia: Parte 3

**Pregunta 57.** ¿Qué es el 'undifferentiated heavy lifting' que AWS busca eliminar para sus clientes?

A) El trabajo creativo único de cada empresa

**B)** **Tareas operativas necesarias pero que no aportan ventaja competitiva, como mantener hardware**

C) El proceso de facturación mensual

D) El soporte técnico de AWS

**Respuesta correcta: B.** 

*AWS libera a los clientes de tareas operativas repetitivas y sin valor diferencial, como mantenimiento de hardware físico.*

Referencia: Parte 1

**Pregunta 58.** ¿Qué tipo de instancia EC2 está optimizada para alto rendimiento de CPU, ideal para procesamiento por lotes o modelado científico?

A) Memory optimized (r, x)

**B)** **Compute optimized (c)**

C) Storage optimized (i, d)

D) General purpose (t, m)

**Respuesta correcta: B.** 

*La familia 'compute optimized' (c) prioriza alto rendimiento de CPU sobre memoria o almacenamiento.*

Referencia: Parte 4

**Pregunta 59.** ¿Qué servicio ayudaría a auditar si un bucket S3 tuvo cifrado activado de forma continua durante los últimos 6 meses?

A) AWS CloudTrail exclusivamente

**B)** **AWS Config, revisando el historial de configuración del recurso**

C) Amazon GuardDuty

D) AWS Shield

**Respuesta correcta: B.** 

*AWS Config mantiene el historial de configuración de un recurso en el tiempo, permitiendo auditar cumplimiento continuo.*

Referencia: Parte 8

**Pregunta 60.** ¿Qué servicio de AWS convierte el esquema y código de una base de datos de origen a la sintaxis de un motor de destino distinto, como parte de una migración heterogénea?

A) AWS DMS

**B)** **AWS Schema Conversion Tool (SCT)**

C) AWS DataSync

D) AWS Migration Hub

**Respuesta correcta: B.** 

*SCT convierte esquema/código; DMS migra los datos en sí. Se usan juntos en migraciones entre motores distintos.*

Referencia: Parte 13

**Pregunta 61.** ¿Qué describe mejor el patrón de 'defensa en profundidad' en el contexto de seguridad de red de AWS?

A) Usar solo Security Groups, sin NACL

**B)** **Combinar Security Groups a nivel de instancia con Network ACL a nivel de subred como capas complementarias**

C) Usar solo NACL, eliminando los Security Groups

D) Confiar únicamente en IAM sin controles de red

**Respuesta correcta: B.** 

*La defensa en profundidad combina múltiples capas de seguridad de red, de forma que el fallo de una capa no deja el sistema completamente expuesto.*

Referencia: Parte 7

**Pregunta 62.** ¿Qué es AWS Control Tower?

A) Un servicio de bases de datos

**B)** **Un servicio construido sobre AWS Organizations que automatiza una zona de aterrizaje multi-cuenta con gobernanza preconfigurada**

C) Un tipo de instancia EC2

D) Un servicio de CDN

**Respuesta correcta: B.** 

*Control Tower simplifica la creación de cuentas nuevas con barreras de gobernanza (guardrails) ya aplicadas, construido sobre Organizations.*

Referencia: Parte 13

**Pregunta 63.** Una empresa necesita un balanceador de carga optimizado para tráfico TCP/UDP de altísimo rendimiento y baja latencia. ¿Cuál debería elegir?

A) Application Load Balancer

**B)** **Network Load Balancer**

C) Gateway Load Balancer

D) Classic Load Balancer exclusivamente

**Respuesta correcta: B.** 

*El Network Load Balancer está optimizado para tráfico TCP/UDP de alto rendimiento y latencia ultra baja, a diferencia del ALB (HTTP/HTTPS).*

Referencia: Parte 4

**Pregunta 64.** ¿Qué describe mejor el rol de Amazon Route 53 frente a Amazon CloudFront?

A) Son el mismo servicio

**B)** **Route 53 resuelve DNS hacia recursos de AWS; CloudFront entrega y cachea contenido desde Edge Locations cercanas al usuario**

C) CloudFront resuelve DNS; Route 53 cachea contenido

D) Ambos son exclusivos para bases de datos

**Respuesta correcta: B.** 

*Route 53 traduce nombres de dominio a direcciones/recursos; CloudFront distribuye contenido cacheado — se combinan frecuentemente.*

Referencia: Parte 7

**Pregunta 65.** ¿Qué elemento de AWS Budgets permite recibir una alerta ANTES de que el gasto real supere un umbral, basándose en la tendencia actual?

**A)** **Alertas basadas en gasto proyectado (forecasted)**

B) Solo alertas basadas en gasto ya ocurrido

C) AWS Budgets no ofrece ningún tipo de alerta proactiva

D) Alertas basadas exclusivamente en el uso de CPU

**Respuesta correcta: A.** 

*AWS Budgets permite configurar alertas basadas en el gasto proyectado, no solo en el gasto real ya ocurrido, permitiendo actuar preventivamente.*

Referencia: Parte 11

## Hoja de respuestas rápida

| # | # | # | # | # |
| --- | --- | --- | --- | --- |
| 1: B | 2: C | 3: B | 4: B | 5: C |
| 6: B | 7: B | 8: B | 9: B | 10: B |
| 11: C | 12: B | 13: B | 14: B | 15: B |
| 16: B | 17: B | 18: B | 19: B | 20: B |
| 21: B | 22: A | 23: B | 24: B | 25: A |
| 26: B | 27: B | 28: B | 29: C | 30: B |
| 31: B | 32: B | 33: B | 34: B | 35: B |
| 36: B | 37: B | 38: C | 39: B | 40: B |
| 41: B | 42: B | 43: B | 44: B | 45: B |
| 46: B | 47: C | 48: B | 49: B | 50: B |
| 51: B | 52: A | 53: B | 54: B | 55: B |
| 56: B | 57: B | 58: B | 59: B | 60: B |
| 61: B | 62: B | 63: B | 64: B | 65: A |
