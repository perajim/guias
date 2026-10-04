# AWS Certified Cloud Practitioner (CLF-C02)

**Simulacro de Examen 2 de 5 — 65 preguntas**

Mismo nivel de dificultad y distribución de dominios que el examen oficial CLF-C02: Cloud Concepts, Security and Compliance, Cloud Technology and Services, y Billing and Pricing. Cada pregunta incluye la respuesta correcta, una explicación, y una referencia al capítulo de la guía donde puedes repasar el tema si fallaste.

> **Cómo usar este simulacro:** Resuélvelo primero completo, sin mirar las respuestas, cronometrando 90 minutos como en el examen real. Después revisa cada pregunta, prestando especial atención a las que fallaste, y repasa el capítulo referenciado antes de tu siguiente simulacro.

## Preguntas

**Pregunta 1.** Una empresa reduce el tiempo de aprovisionamiento de nuevos servidores de semanas a minutos al migrar a AWS. ¿Qué beneficio del cloud computing ilustra esto?

A) Economías de escala

**B)** **Agilidad**

C) Tolerancia a fallos

D) Nube comunitaria

**Respuesta correcta: B.** 

*La agilidad se refiere a la rapidez con la que se pueden aprovisionar nuevos recursos de TI en la nube frente a semanas o meses on-premises.*

Referencia: Parte 1

**Pregunta 2.** Un desarrollador sube su código a Elastic Beanstalk sin preocuparse por el sistema operativo subyacente. ¿Qué modelo de servicio describe esto?

A) IaaS

**B)** **PaaS**

C) SaaS

D) On-premises

**Respuesta correcta: B.** 

*PaaS entrega la plataforma de ejecución (SO, runtime); el cliente solo administra el código de la aplicación.*

Referencia: Parte 1

**Pregunta 3.** ¿Qué diferencia a la tolerancia a fallos de la alta disponibilidad?

A) No hay diferencia

**B)** **Tolerancia a fallos = cero downtime perceptible; Alta disponibilidad = downtime mínimo pero puede existir una breve interrupción**

C) Alta disponibilidad requiere múltiples Regiones obligatoriamente

D) Tolerancia a fallos solo aplica a redes

**Respuesta correcta: B.** 

*La tolerancia a fallos es un nivel más estricto que la alta disponibilidad: el sistema no debe mostrar ninguna interrupción perceptible ante el fallo de un componente.*

Referencia: Parte 1

**Pregunta 4.** ¿Cuál de los siguientes criterios NO es mencionado por AWS como relevante para elegir una Región?

A) Cumplimiento normativo

B) Latencia hacia los usuarios

C) Disponibilidad de servicios

**D)** **Cantidad de empleados de AWS en esa ciudad**

**Respuesta correcta: D.** 

*AWS menciona cumplimiento, latencia, disponibilidad de servicios y costo como criterios; la cantidad de empleados locales no es un criterio real.*

Referencia: Parte 2

**Pregunta 5.** ¿Qué herramienta de AWS es la más adecuada para automatizar el lanzamiento de 100 instancias idénticas dentro de un pipeline de CI/CD?

A) AWS Management Console exclusivamente

**B)** **AWS CLI o SDK dentro de un script**

C) Llamar a soporte de AWS

D) AWS Artifact

**Respuesta correcta: B.** 

*Para automatización sin intervención manual, el CLI o los SDK son la elección correcta, ya que pueden ejecutarse de forma programática.*

Referencia: Parte 2

**Pregunta 6.** ¿Qué tipo de policy de IAM está embebida directamente en un único User, Group o Role, sin poder reutilizarse en otra identidad?

A) AWS managed policy

B) Customer managed policy

**C)** **Inline policy**

D) Resource-based policy

**Respuesta correcta: C.** 

*Las inline policies se adjuntan directamente a una sola identidad y se eliminan junto con ella; no son reutilizables como las managed policies.*

Referencia: Parte 3

**Pregunta 7.** ¿Qué componente de un IAM Role determina QUIÉN puede asumirlo?

A) La permissions policy

**B)** **La trust policy**

C) El Access Key ID

D) El Security Group asociado

**Respuesta correcta: B.** 

*La trust policy de un Role especifica qué identidades (usuarios, servicios, cuentas) tienen permitido asumir ese rol.*

Referencia: Parte 3

**Pregunta 8.** Una empresa con Active Directory corporativo quiere que sus empleados accedan a AWS con sus credenciales existentes, sin crear un IAM User por persona. ¿Qué solución es la más adecuada?

A) Crear cientos de IAM Users manualmente

**B)** **Federación de identidades vía AWS IAM Identity Center**

C) Compartir las credenciales del usuario root

D) Deshabilitar IAM completamente

**Respuesta correcta: B.** 

*La federación permite autenticarse contra un directorio existente y obtener acceso temporal a AWS sin crear un IAM User por persona.*

Referencia: Parte 3

**Pregunta 9.** ¿Qué tipo de instancia EC2 se recomienda para bases de datos NoSQL de alta transacción que requieren alto I/O de disco local?

A) General purpose (t, m)

B) Compute optimized (c)

**C)** **Storage optimized (i, d)**

D) Memory optimized (r, x) exclusivamente

**Respuesta correcta: C.** 

*La familia 'storage optimized' (i, d) prioriza alto rendimiento de I/O de disco local, ideal para bases NoSQL de alta transacción.*

Referencia: Parte 4

**Pregunta 10.** ¿Qué servicio permite ejecutar contenedores sin administrar los servidores EC2 subyacentes del clúster?

A) Amazon ECS con tipo de lanzamiento EC2

**B)** **AWS Fargate**

C) AWS Batch exclusivamente

D) Amazon Lightsail

**Respuesta correcta: B.** 

*AWS Fargate es el motor de cómputo serverless para contenedores, usado junto con ECS o EKS, eliminando la administración de servidores del clúster.*

Referencia: Parte 4

**Pregunta 11.** ¿Qué caracteriza a un Security Group en cuanto al tráfico de respuesta?

A) Es stateless, requiere reglas explícitas de salida

**B)** **Es stateful: el tráfico de respuesta se permite automáticamente**

C) No permite ningún tráfico saliente

D) Solo permite tráfico desde 0.0.0.0/0

**Respuesta correcta: B.** 

*Un Security Group es stateful: si se permite tráfico entrante, la respuesta saliente se permite automáticamente sin regla adicional.*

Referencia: Parte 4

**Pregunta 12.** ¿Qué clase de almacenamiento de S3 mueve automáticamente los objetos entre niveles de acceso según el patrón de uso real, sin cargos de recuperación?

A) S3 Standard-IA

B) S3 One Zone-IA

**C)** **S3 Intelligent-Tiering**

D) S3 Glacier Deep Archive

**Respuesta correcta: C.** 

*S3 Intelligent-Tiering monitorea el acceso real y mueve los objetos entre niveles automáticamente, sin cargos por recuperación ni gestión manual.*

Referencia: Parte 5

**Pregunta 13.** ¿Qué combinación de servicios de AWS soporta la restricción WORM (Write Once Read Many) para cumplimiento regulatorio?

**A)** **S3 con Object Lock en modo de cumplimiento**

B) EBS con snapshots automáticos

C) EFS con versionado

D) DynamoDB con TTL

**Respuesta correcta: A.** 

*S3 Object Lock impide la eliminación o sobrescritura de objetos durante un periodo definido, cumpliendo requisitos WORM regulatorios.*

Referencia: Parte 5

**Pregunta 14.** ¿Qué servicio administrado replica datos en bloque hacia AWS desde servidores on-premises usando iSCSI?

A) File Gateway

**B)** **Volume Gateway**

C) Tape Gateway

D) AWS DataSync

**Respuesta correcta: B.** 

*Volume Gateway presenta volúmenes en bloque vía iSCSI hacia servidores on-premises, con modos cached o stored.*

Referencia: Parte 5

**Pregunta 15.** ¿Qué tipo de Read Replica de RDS puede ubicarse en una Región distinta a la de la base de datos primaria?

A) Ninguna, siempre deben estar en la misma Región

**B)** **Read Replicas entre Regiones (cross-Region), disponibles en varios motores de RDS**

C) Solo Multi-AZ soporta múltiples Regiones

D) Read Replicas nunca pueden usarse para lecturas activas

**Respuesta correcta: B.** 

*RDS soporta Read Replicas entre Regiones distintas en varios motores, útiles para escalar lecturas geográficamente distribuidas o como base para DR.*

Referencia: Parte 6

**Pregunta 16.** ¿Qué servicio de base de datos sería el más adecuado para modelar y consultar relaciones de recomendación entre usuarios de una red social?

A) Amazon Redshift

**B)** **Amazon Neptune**

C) Amazon ElastiCache

D) AWS Batch

**Respuesta correcta: B.** 

*Neptune está optimizado para almacenar y navegar relaciones altamente conectadas, ideal para grafos de recomendación social.*

Referencia: Parte 6

**Pregunta 17.** ¿Qué modo de capacidad de DynamoDB es el más adecuado para una carga de trabajo nueva con patrón de tráfico impredecible?

A) Provisioned sin Auto Scaling

**B)** **On-Demand**

C) Reserved Capacity exclusivamente

D) DynamoDB no ofrece modos de capacidad distintos

**Respuesta correcta: B.** 

*El modo On-Demand cobra por solicitud real sin necesidad de estimar capacidad de antemano, ideal para cargas impredecibles.*

Referencia: Parte 6

**Pregunta 18.** ¿Qué elemento de una VPC define hacia dónde se dirige el tráfico según la IP de destino?

A) Security Group

**B)** **Route Table**

C) AMI

D) IAM Role

**Respuesta correcta: B.** 

*La tabla de rutas de una subred determina el destino del tráfico según la IP, definiendo si la subred es pública o privada.*

Referencia: Parte 7

**Pregunta 19.** ¿Qué combinación de servicios protegería una aplicación web contra tráfico DDoS masivo Y contra inyección SQL en las peticiones HTTP?

A) Solo AWS Shield

B) Solo AWS WAF

**C)** **AWS Shield (DDoS) combinado con AWS WAF (capa de aplicación)**

D) Solo Security Groups

**Respuesta correcta: C.** 

*Shield protege contra DDoS a nivel de red/transporte; WAF filtra patrones maliciosos específicos en el tráfico HTTP como inyección SQL — se complementan.*

Referencia: Parte 7 y 8

**Pregunta 20.** ¿Qué servicio de AWS resolvería nombres de dominio hacia un Application Load Balancer usando un alias record?

A) Amazon CloudFront

**B)** **Amazon Route 53**

C) AWS Direct Connect

D) Amazon VPC

**Respuesta correcta: B.** 

*Route 53 resuelve DNS hacia recursos de AWS mediante alias records, incluyendo Load Balancers.*

Referencia: Parte 7

**Pregunta 21.** ¿Qué es responsabilidad EXCLUSIVA del cliente según el Modelo de Responsabilidad Compartida, sin importar el servicio de AWS usado?

A) El hipervisor

**B)** **La clasificación y configuración de sus propios datos**

C) La infraestructura física de los data centers

D) La red troncal global de AWS

**Respuesta correcta: B.** 

*La clasificación y configuración de los datos del cliente es siempre responsabilidad del cliente, independientemente de cuán administrado sea el servicio.*

Referencia: Parte 8

**Pregunta 22.** ¿Qué servicio evaluaría vulnerabilidades conocidas (CVEs) en una imagen de contenedor almacenada en Amazon ECR?

A) Amazon GuardDuty

**B)** **Amazon Inspector**

C) Amazon Macie

D) AWS Shield

**Respuesta correcta: B.** 

*Amazon Inspector escanea EC2, imágenes de contenedores en ECR y funciones Lambda en busca de vulnerabilidades conocidas.*

Referencia: Parte 8

**Pregunta 23.** ¿Qué servicio permite rotar automáticamente la contraseña de una base de datos RDS según un calendario definido?

A) AWS KMS

**B)** **AWS Secrets Manager**

C) Amazon Macie

D) AWS Certificate Manager

**Respuesta correcta: B.** 

*Secrets Manager centraliza secretos y puede rotarlos automáticamente, integrándose de forma nativa con RDS.*

Referencia: Parte 8

**Pregunta 24.** ¿Qué diferencia a CloudWatch de X-Ray?

A) Son el mismo servicio

**B)** **CloudWatch ofrece métricas/logs agregados; X-Ray rastrea el recorrido detallado de solicitudes individuales**

C) X-Ray reemplaza completamente a CloudWatch

D) CloudWatch solo funciona con Lambda

**Respuesta correcta: B.** 

*CloudWatch da una vista agregada de infraestructura y aplicación; X-Ray traza solicitudes individuales a través de servicios distribuidos.*

Referencia: Parte 9

**Pregunta 25.** ¿Qué vista del AWS Health Dashboard está disponible públicamente sin necesidad de iniciar sesión?

A) Personal Health únicamente

**B)** **Service Health**

C) Ninguna vista es pública

D) Solo para clientes Enterprise Support

**Respuesta correcta: B.** 

*La vista 'Service Health' muestra el estado operativo general de AWS y es pública, sin requerir sesión iniciada.*

Referencia: Parte 9

**Pregunta 26.** ¿Qué acción puede disparar automáticamente una CloudWatch Alarm al cruzar un umbral definido?

A) Aprobar solicitudes de acceso de usuarios IAM

**B)** **Enviar una notificación vía SNS o disparar una acción de Auto Scaling**

C) Cambiar automáticamente el plan de soporte de la cuenta

D) Renovar automáticamente un certificado ACM

**Respuesta correcta: B.** 

*Las CloudWatch Alarms pueden disparar notificaciones SNS, acciones de Auto Scaling, o acciones directas sobre instancias EC2.*

Referencia: Parte 9

**Pregunta 27.** ¿Qué servicio de AWS permite enrutar eventos según reglas basadas en el contenido del evento, integrando además fuentes SaaS de terceros?

A) Amazon SQS

B) Amazon SNS

**C)** **Amazon EventBridge**

D) AWS Step Functions

**Respuesta correcta: C.** 

*EventBridge ofrece enrutamiento flexible basado en reglas y soporta fuentes de AWS, propias, y SaaS de terceros.*

Referencia: Parte 10

**Pregunta 28.** ¿Qué mecanismo de Amazon SQS oculta temporalmente un mensaje a otros consumidores tras ser recibido, sin eliminarlo de la cola?

A) Dead Letter Queue

**B)** **Visibility timeout**

C) FIFO ordering

D) Long polling

**Respuesta correcta: B.** 

*El visibility timeout oculta el mensaje temporalmente; si no se elimina explícitamente dentro de ese periodo, vuelve a estar disponible.*

Referencia: Parte 10

**Pregunta 29.** ¿Qué modelo de precios de EC2 es ideal para una carga de trabajo constante y predecible durante los próximos 3 años, maximizando el descuento?

A) On-Demand

**B)** **Reserved Instances o Savings Plans a 3 años con pago por adelantado**

C) Spot Instances exclusivamente

D) AWS Free Tier

**Respuesta correcta: B.** 

*Un compromiso a 3 años con pago anticipado maximiza el descuento frente a On-Demand para cargas constantes y predecibles.*

Referencia: Parte 11

**Pregunta 30.** ¿Qué transferencia de datos en AWS generalmente NO tiene costo?

A) Transferencia saliente hacia internet

**B)** **Transferencia entrante hacia AWS**

C) Transferencia entre Regiones distintas siempre

D) Ninguna transferencia es gratuita

**Respuesta correcta: B.** 

*La transferencia de datos entrante hacia AWS es gratuita en la gran mayoría de los casos; la saliente hacia internet sí tiene costo.*

Referencia: Parte 11

**Pregunta 31.** ¿Qué pilar del Well-Architected Framework se enfoca en usar los recursos de cómputo de forma eficiente ante demanda y tecnología cambiantes?

A) Seguridad

**B)** **Eficiencia del Rendimiento**

C) Optimización de Costos exclusivamente

D) Excelencia Operacional exclusivamente

**Respuesta correcta: B.** 

*Eficiencia del Rendimiento se enfoca en seleccionar y mantener el uso más eficiente de los recursos conforme cambia la demanda y la tecnología.*

Referencia: Parte 12

**Pregunta 32.** ¿Qué herramienta gratuita permite evaluar formalmente una carga de trabajo contra los seis pilares del framework, generando un reporte de riesgos?

A) AWS Trusted Advisor

**B)** **AWS Well-Architected Tool**

C) AWS Config

D) Amazon Inspector

**Respuesta correcta: B.** 

*El AWS Well-Architected Tool guía un cuestionario estructurado por pilar y genera un reporte de riesgos con recomendaciones.*

Referencia: Parte 12

**Pregunta 33.** ¿Qué framework permite definir infraestructura de AWS usando lenguajes de programación de propósito general, sintetizando hacia CloudFormation?

A) AWS Control Tower

**B)** **AWS Cloud Development Kit (CDK)**

C) AWS Config

D) AWS Backup

**Respuesta correcta: B.** 

*CDK permite escribir infraestructura en TypeScript, Python, Java, etc., generando internamente plantillas de CloudFormation.*

Referencia: Parte 13

**Pregunta 34.** ¿Qué servicio ofrece un panel centralizado para rastrear el progreso de una migración de aplicaciones que usa múltiples herramientas distintas?

**A)** **AWS Migration Hub**

B) AWS DataSync

C) AWS Snowmobile

D) Amazon FSx

**Respuesta correcta: A.** 

*Migration Hub consolida el estado de avance de migraciones complejas provenientes de distintas herramientas en un panel único.*

Referencia: Parte 13

**Pregunta 35.** Una empresa mantiene su ERP crítico en su propio data center por requisitos regulatorios, pero usa AWS para análisis de datos no sensibles. ¿Qué modelo de despliegue es este?

A) Nube pública pura

B) Nube privada pura

**C)** **Nube híbrida**

D) Nube comunitaria

**Respuesta correcta: C.** 

*Combinar infraestructura on-premises con nube pública para distintas cargas de trabajo es un ejemplo directo de nube híbrida.*

Referencia: Parte 1

**Pregunta 36.** ¿Qué diferencia a la virtualización de la contenedorización en cuanto a lo que se comparte con el host?

A) Son exactamente lo mismo

**B)** **La virtualización usa un hipervisor con SO completo por VM; los contenedores comparten el kernel del sistema operativo anfitrión**

C) Los contenedores requieren siempre más recursos que una VM completa

D) La virtualización no existe en AWS

**Respuesta correcta: B.** 

*Las VMs tienen su propio SO completo mediante un hipervisor; los contenedores comparten el kernel del host, siendo más ligeros.*

Referencia: Parte 1 y 4

**Pregunta 37.** ¿Qué recomienda AWS respecto al uso del usuario root en el día a día operativo?

A) Usarlo siempre para mayor comodidad

**B)** **Protegerlo con MFA y reservarlo solo para tareas que estrictamente lo requieran**

C) Compartirlo entre todo el equipo

D) Eliminarlo completamente de la cuenta

**Respuesta correcta: B.** 

*El root tiene control total e irrestricto; AWS recomienda protegerlo con MFA y usarlo solo para tareas excepcionales, no el trabajo diario.*

Referencia: Parte 3

**Pregunta 38.** ¿Qué ocurre si una instancia dentro de un Auto Scaling Group falla sus verificaciones de salud?

**A)** **El ASG la reemplaza automáticamente por una nueva instancia saludable**

B) El ASG apaga todo el grupo

C) No ocurre ninguna acción automática

D) El tráfico se redirige a la instancia fallida de todas formas

**Respuesta correcta: A.** 

*El ASG reemplaza automáticamente instancias que fallan las verificaciones de salud, aportando resiliencia además de elasticidad.*

Referencia: Parte 4

**Pregunta 39.** ¿Qué característica NO corresponde a Amazon Lightsail?

A) Precios mensuales fijos y predecibles

B) Configuración de red simplificada sin gestionar una VPC completa manualmente

**C)** **Control granular completo de tipos de instancia como en EC2 puro**

D) Ideal para principiantes o proyectos pequeños

**Respuesta correcta: C.** 

*Lightsail prioriza simplicidad sobre control granular; para ese nivel de control se recomienda EC2 con VPC completa.*

Referencia: Parte 4

**Pregunta 40.** ¿Qué sucede con los objetos de un bucket S3 al eliminarlos cuando el versionado está activo?

A) Se eliminan permanentemente de inmediato

**B)** **Se añade un marcador de eliminación (delete marker); las versiones anteriores siguen existiendo**

C) El bucket completo se elimina automáticamente

D) S3 rechaza la operación de eliminación

**Respuesta correcta: B.** 

*Con versionado activo, 'eliminar' un objeto solo añade un delete marker; las versiones previas persisten hasta eliminarse explícitamente.*

Referencia: Parte 5

**Pregunta 41.** ¿Qué servicio sería el más adecuado para un sistema de archivos compartido compatible con SMB e integración a Active Directory?

A) Amazon EFS

**B)** **Amazon FSx for Windows File Server**

C) Amazon S3

D) AWS Storage Gateway Volume Gateway

**Respuesta correcta: B.** 

*FSx for Windows File Server ofrece compatibilidad SMB e integración nativa con Active Directory, algo que EFS (basado en NFS) no cubre.*

Referencia: Parte 5

**Pregunta 42.** ¿Qué servicio de AWS sería el más adecuado para reportes de business intelligence sobre años de datos históricos de ventas?

A) Amazon DynamoDB

**B)** **Amazon Redshift**

C) Amazon ElastiCache

D) AWS Batch

**Respuesta correcta: B.** 

*Redshift está optimizado para consultas analíticas complejas (OLAP) sobre grandes volúmenes históricos, ideal para BI.*

Referencia: Parte 6

**Pregunta 43.** ¿Qué característica del NAT Gateway es correcta?

A) Se ubica en una subred privada

**B)** **Se ubica en una subred pública y permite tráfico saliente desde subredes privadas**

C) Permite conexiones entrantes no solicitadas hacia instancias privadas

D) Reemplaza la necesidad de un Internet Gateway en toda la VPC

**Respuesta correcta: B.** 

*El NAT Gateway vive en una subred pública (para poder alcanzar el IGW) y sirve de intermediario de salida para las subredes privadas.*

Referencia: Parte 7

**Pregunta 44.** ¿Qué recomienda AWS al conectar un data center on-premises con alta necesidad de ancho de banda consistente y baja latencia de forma sostenida?

A) Usar exclusivamente Site-to-Site VPN

**B)** **AWS Direct Connect, posiblemente con VPN como respaldo**

C) No es posible conectar on-premises con AWS de forma privada

D) Usar únicamente Amazon CloudFront

**Respuesta correcta: B.** 

*Direct Connect ofrece la conectividad dedicada más consistente; VPN puede usarse como respaldo (failover) de Direct Connect.*

Referencia: Parte 7

**Pregunta 45.** ¿Cuál de las siguientes prácticas de seguridad viola directamente el principio de mínimo privilegio?

A) Crear policies granulares por función de trabajo

**B)** **Otorgar 'AdministratorAccess' a todos los usuarios para simplificar la gestión**

C) Revisar periódicamente permisos no utilizados

D) Usar IAM Access Analyzer para auditar accesos

**Respuesta correcta: B.** 

*Otorgar acceso administrador completo a todos viola el mínimo privilegio, que exige otorgar solo lo estrictamente necesario.*

Referencia: Parte 3 y 8

**Pregunta 46.** ¿Qué tipo de hallazgo generaría típicamente Amazon GuardDuty?

A) Un bucket S3 sin cifrado detectado por análisis de configuración estática

**B)** **Una instancia EC2 comunicándose con una IP conocida de distribución de malware**

C) Un certificado SSL a punto de expirar

D) Una vulnerabilidad de software desactualizado en una AMI

**Respuesta correcta: B.** 

*GuardDuty analiza comportamiento y tráfico de red en busca de patrones maliciosos, como comunicación con infraestructura de malware conocida.*

Referencia: Parte 8

**Pregunta 47.** ¿Qué combinación de servicios de integración usarías para que un evento se procese por un SOLO consumidor de forma controlada, con reintentos si falla?

A) Amazon SNS exclusivamente

**B)** **Amazon SQS**

C) Amazon Route 53

D) AWS Certificate Manager

**Respuesta correcta: B.** 

*SQS es el patrón adecuado cuando se necesita un consumidor procesando mensajes de forma controlada, con reintentos vía visibility timeout.*

Referencia: Parte 10

**Pregunta 48.** ¿Qué estrategia de optimización de costos consiste en ajustar el tipo/tamaño de un recurso a la demanda real observada?

**A)** **Rightsizing**

B) Federación de identidades

C) Object Lock

D) Chaos engineering

**Respuesta correcta: A.** 

*Rightsizing ajusta instancias u otros recursos al uso real, evitando tanto sobreaprovisionamiento como subaprovisionamiento.*

Referencia: Parte 11

**Pregunta 49.** ¿Qué describe mejor un trade-off típico entre pilares del Well-Architected Framework?

A) Los pilares nunca generan tensión entre sí

**B)** **Mayor redundancia multi-Región mejora Fiabilidad pero incrementa el costo (tensión con Optimización de Costos)**

C) Todos los pilares siempre se maximizan simultáneamente sin costo adicional

D) Solo existe un pilar relevante por carga de trabajo

**Respuesta correcta: B.** 

*Aumentar la redundancia para mejorar Fiabilidad normalmente incrementa el costo, ilustrando un trade-off consciente entre pilares.*

Referencia: Parte 12

**Pregunta 50.** ¿Qué distingue a AWS Snowball Edge de un Snowball estándar?

A) No hay diferencia

**B)** **Snowball Edge añade capacidad de cómputo local (puede correr EC2/Lambda en el dispositivo)**

C) Snowball Edge es exclusivamente para bases de datos

D) Snowball Edge no puede transferir datos, solo procesarlos

**Respuesta correcta: B.** 

*Snowball Edge añade cómputo local al dispositivo, útil para procesar datos en el borde en ubicaciones con conectividad limitada.*

Referencia: Parte 13

**Pregunta 51.** ¿Qué garantiza que los datos de un cliente no salgan de una Región específica de AWS, salvo acción explícita del cliente?

A) Un Security Group restrictivo

**B)** **El diseño de aislamiento geográfico de las Regiones de AWS**

C) Un NACL con reglas Deny

D) AWS Shield Advanced

**Respuesta correcta: B.** 

*Cada Región de AWS es un clúster aislado; los datos permanecen ahí a menos que el cliente configure explícitamente replicación entre Regiones.*

Referencia: Parte 2

**Pregunta 52.** ¿Qué diferencia a un IAM Group de un IAM Role?

A) Son sinónimos exactos

**B)** **Un Group es una colección de Users sin credenciales propias; un Role sí se asume y genera credenciales temporales**

C) Un Role es una colección de Groups

D) Un Group puede iniciar sesión directamente en la consola

**Respuesta correcta: B.** 

*El Group organiza Users para asignar policies en bloque, sin ser una identidad asumible; el Role sí se asume y genera credenciales temporales.*

Referencia: Parte 3

**Pregunta 53.** ¿Qué combinación describe correctamente Reserved Instances vs Spot Instances en cuanto a certeza del compromiso?

A) Ambas requieren el mismo nivel de compromiso

**B)** **Reserved Instances = compromiso fijo con descuento garantizado; Spot = sin compromiso pero con riesgo de interrupción**

C) Spot Instances requieren compromiso de 3 años obligatorio

D) Reserved Instances pueden interrumpirse con 2 minutos de aviso

**Respuesta correcta: B.** 

*RI comprometen uso a cambio de descuento garantizado y sin riesgo de interrupción; Spot no requiere compromiso pero sí acepta el riesgo de interrupción.*

Referencia: Parte 11

**Pregunta 54.** ¿Qué elemento de gobernanza permite a una organización con múltiples cuentas prohibir el uso de ciertas Regiones en todas las cuentas miembro?

A) IAM Policies individuales por cuenta

**B)** **Service Control Policies (SCPs) de AWS Organizations**

C) AWS Budgets

D) Amazon CloudWatch Alarms

**Respuesta correcta: B.** 

*Las SCPs definen los permisos máximos permitidos en cuentas miembro de una organización, aplicando restricciones centralizadas como prohibir Regiones.*

Referencia: Parte 11

**Pregunta 55.** ¿Qué servicio es más adecuado para un caso de uso de detección de fraude que analiza relaciones entre cuentas, dispositivos y transacciones?

A) Amazon Redshift

**B)** **Amazon Neptune**

C) AWS Batch

D) Amazon Lightsail

**Respuesta correcta: B.** 

*Neptune está optimizado para consultas sobre relaciones altamente conectadas, un patrón común en detección de fraude.*

Referencia: Parte 6

**Pregunta 56.** ¿Qué es cierto respecto a las Local Zones de AWS?

A) Son idénticas a las Availability Zones en todos los aspectos

**B)** **Extienden un subconjunto de servicios de AWS más cerca de grandes áreas metropolitanas para latencia ultra baja**

C) Solo existen dentro de Estados Unidos

D) No pueden ejecutar instancias EC2 bajo ninguna circunstancia

**Respuesta correcta: B.** 

*Las Local Zones acercan cómputo y almacenamiento a grandes ciudades sin Región completa cercana, para casos de latencia ultra baja.*

Referencia: Parte 2

**Pregunta 57.** ¿Qué describe mejor la relación entre AWS Organizations y AWS Control Tower?

A) Son servicios completamente independientes

**B)** **Control Tower se construye sobre Organizations, añadiendo automatización de gobernanza multi-cuenta**

C) Organizations se construye sobre Control Tower

D) Ambos son el mismo servicio con nombres distintos

**Respuesta correcta: B.** 

*Control Tower usa Organizations como base y añade automatización de guardrails y estructura de cuentas preconfigurada.*

Referencia: Parte 13

**Pregunta 58.** ¿Qué beneficio de negocio del cloud computing describe la capacidad de desplegar una aplicación en múltiples continentes en cuestión de minutos?

**A)** **Ir global en minutos**

B) Tolerancia a fallos

C) Nube comunitaria

D) Federación de identidades

**Respuesta correcta: A.** 

*AWS cita 'Go Global in Minutes' como uno de sus seis beneficios: desplegar cerca de usuarios de cualquier continente sin construir data centers propios ahí.*

Referencia: Parte 1

**Pregunta 59.** ¿Qué es un IAM Access Analyzer usado para?

A) Cifrar datos en tránsito

**B)** **Identificar permisos no utilizados o accesos no deseados hacia recursos externos**

C) Balancear tráfico entre instancias

D) Migrar bases de datos entre motores

**Respuesta correcta: B.** 

*IAM Access Analyzer ayuda a aplicar el principio de mínimo privilegio detectando permisos excesivos o accesos hacia fuera de la cuenta no intencionados.*

Referencia: Parte 3

**Pregunta 60.** ¿Qué servicio permite ejecutar trabajos de procesamiento por lotes a escala, gestionando automáticamente la cola y el aprovisionamiento de cómputo (incluyendo Spot)?

**A)** **AWS Batch**

B) Amazon Lightsail

C) AWS Direct Connect

D) Amazon Route 53

**Respuesta correcta: A.** 

*AWS Batch planifica y ejecuta trabajos por lotes, aprovisionando dinámicamente los recursos óptimos, incluyendo instancias Spot para reducir costos.*

Referencia: Parte 4

**Pregunta 61.** ¿Qué describe mejor el propósito de un EBS Snapshot?

**A)** **Un respaldo puntual incremental de un volumen EBS, almacenado en S3 de forma interna**

B) Una réplica activa y legible de una base de datos

C) Un tipo de instancia EC2

D) Una regla de firewall

**Respuesta correcta: A.** 

*Los EBS Snapshots son copias de respaldo incrementales de un volumen, útiles para backups y para crear nuevos volúmenes idénticos.*

Referencia: Parte 5

**Pregunta 62.** ¿Qué servicio de AWS ofrecería lecturas de solo lectura escalables para descargar tráfico de una base de datos RDS muy consultada?

A) RDS Multi-AZ exclusivamente

**B)** **RDS Read Replicas**

C) Amazon Redshift exclusivamente

D) AWS Batch

**Respuesta correcta: B.** 

*Las Read Replicas de RDS escalan el tráfico de lectura dirigiendo consultas hacia copias activas de solo lectura, distinto del propósito de Multi-AZ.*

Referencia: Parte 6

**Pregunta 63.** ¿Qué elemento de AWS WAF permite limitar cuántas peticiones por minuto puede hacer una misma IP hacia una aplicación?

**A)** **Rate-based rules (reglas basadas en tasa)**

B) Un Security Group

C) Una Network ACL

D) AWS Shield Standard exclusivamente

**Respuesta correcta: A.** 

*AWS WAF admite reglas basadas en tasa (rate-based rules) que bloquean automáticamente IPs que exceden un número de peticiones definido en una ventana de tiempo.*

Referencia: Parte 8

**Pregunta 64.** ¿Qué panel consolidaría el estado de avance de una migración compleja que usa DMS, DataSync y Snowball simultáneamente?

**A)** **AWS Migration Hub**

B) Amazon CloudWatch

C) AWS Config

D) AWS Trusted Advisor

**Respuesta correcta: A.** 

*Migration Hub centraliza y consolida el estado de múltiples herramientas de migración en un único panel de seguimiento.*

Referencia: Parte 13

**Pregunta 65.** ¿Qué recomienda el pilar de Sostenibilidad respecto a servicios administrados frente a instancias EC2 dedicadas subutilizadas?

A) Evitar siempre los servicios administrados

**B)** **Preferir servicios administrados cuando sea razonable, ya que a menudo comparten infraestructura de forma más eficiente entre clientes**

C) No existe relación entre este tema y sostenibilidad

D) Usar exclusivamente Dedicated Hosts para reducir el impacto ambiental

**Respuesta correcta: B.** 

*El pilar de Sostenibilidad sugiere que los servicios administrados, al compartir infraestructura eficientemente entre múltiples clientes, suelen reducir el desperdicio de capacidad frente a instancias dedicadas subutilizadas.*

Referencia: Parte 12

## Hoja de respuestas rápida

| # | # | # | # | # |
| --- | --- | --- | --- | --- |
| 1: B | 2: B | 3: B | 4: D | 5: B |
| 6: C | 7: B | 8: B | 9: C | 10: B |
| 11: B | 12: C | 13: A | 14: B | 15: B |
| 16: B | 17: B | 18: B | 19: C | 20: B |
| 21: B | 22: B | 23: B | 24: B | 25: B |
| 26: B | 27: C | 28: B | 29: B | 30: B |
| 31: B | 32: B | 33: B | 34: A | 35: C |
| 36: B | 37: B | 38: A | 39: C | 40: B |
| 41: B | 42: B | 43: B | 44: B | 45: B |
| 46: B | 47: B | 48: A | 49: B | 50: B |
| 51: B | 52: B | 53: B | 54: B | 55: B |
| 56: B | 57: B | 58: A | 59: B | 60: A |
| 61: A | 62: B | 63: A | 64: A | 65: B |
