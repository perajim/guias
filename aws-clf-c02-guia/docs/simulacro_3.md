# AWS Certified Cloud Practitioner (CLF-C02)

**Simulacro de Examen 3 de 5 — 65 preguntas**

Mismo nivel de dificultad y distribución de dominios que el examen oficial CLF-C02: Cloud Concepts, Security and Compliance, Cloud Technology and Services, y Billing and Pricing. Cada pregunta incluye la respuesta correcta, una explicación, y una referencia al capítulo de la guía donde puedes repasar el tema si fallaste.

> **Cómo usar este simulacro:** Resuélvelo primero completo, sin mirar las respuestas, cronometrando 90 minutos como en el examen real. Después revisa cada pregunta, prestando especial atención a las que fallaste, y repasa el capítulo referenciado antes de tu siguiente simulacro.

## Preguntas

**Pregunta 1.** Una empresa migra sus servidores a la nube y deja de tener que reemplazar hardware físico cada pocos años. ¿Qué beneficio del cloud computing describe esto?

A) Elasticidad

**B)** **Dejar de gastar dinero en mantener data centers**

C) Nube comunitaria

D) Recuperación ante desastres

**Respuesta correcta: B.** 

*Uno de los seis beneficios citados por AWS es dejar de invertir en mantener infraestructura física propia, enfocándose en lo que diferencia al negocio.*

Referencia: Parte 1

**Pregunta 2.** ¿Qué modelo de despliegue de nube está dedicado exclusivamente a una sola organización, ya sea gestionado internamente o por un tercero?

A) Nube pública

**B)** **Nube privada**

C) Nube híbrida

D) Multi-cloud

**Respuesta correcta: B.** 

*La nube privada está dedicada a una sola organización, a diferencia de la pública, que es compartida (multi-tenant) entre múltiples clientes.*

Referencia: Parte 1

**Pregunta 3.** ¿Qué tecnología permite dividir un servidor físico en múltiples máquinas virtuales aisladas entre sí?

A) Contenedorización

**B)** **Virtualización**

C) Elasticidad

D) Federación

**Respuesta correcta: B.** 

*La virtualización usa un hipervisor para dividir un servidor físico en VMs aisladas, siendo la base tecnológica del cloud computing moderno.*

Referencia: Parte 1

**Pregunta 4.** ¿Qué es AWS Local Zones?

A) Un sinónimo de Región

**B)** **Una extensión de infraestructura de AWS más cercana a grandes áreas metropolitanas, para latencia de un solo dígito de milisegundos**

C) El nombre técnico del usuario root

D) Una herramienta de facturación

**Respuesta correcta: B.** 

*Local Zones acercan cómputo y almacenamiento a ciudades específicas que no tienen una Región completa cerca, para casos de latencia ultra baja.*

Referencia: Parte 2

**Pregunta 5.** ¿Qué comando de AWS CLI listaría los buckets de S3 en tu cuenta?

A) aws ec2 describe-instances

**B)** **aws s3 ls**

C) aws iam list-users

D) aws lambda list-functions

**Respuesta correcta: B.** 

*'aws s3 ls' es el comando estándar del CLI para listar los buckets de Amazon S3 asociados a las credenciales configuradas.*

Referencia: Parte 2

**Pregunta 6.** ¿Qué tipo de policy de IAM viene predefinida y mantenida por AWS, lista para adjuntar directamente?

A) Customer managed policy

B) Inline policy

**C)** **AWS managed policy**

D) Resource-based policy

**Respuesta correcta: C.** 

*Las AWS managed policies son predefinidas y mantenidas por AWS para casos de uso comunes, actualizándose automáticamente cuando es necesario.*

Referencia: Parte 3

**Pregunta 7.** ¿Qué elemento de IAM identifica de forma única un recurso específico de AWS dentro de una policy?

A) El Access Key ID

**B)** **El ARN (Amazon Resource Name)**

C) El Account ID únicamente

D) El nombre de la Región

**Respuesta correcta: B.** 

*El ARN es el identificador único y estandarizado de cualquier recurso en AWS, usado en el elemento 'Resource' de una policy.*

Referencia: Parte 3

**Pregunta 8.** ¿Qué credenciales genera AWS STS cuando un usuario o servicio asume un IAM Role?

A) Credenciales permanentes idénticas al usuario root

**B)** **Credenciales temporales con expiración configurable**

C) Una nueva contraseña de consola

D) Ninguna credencial, el acceso es directo

**Respuesta correcta: B.** 

*AWS Security Token Service genera credenciales temporales con duración configurable al asumir un Role, reduciendo el riesgo de exposición prolongada.*

Referencia: Parte 3

**Pregunta 9.** ¿Qué servicio de AWS entrega máquinas virtuales con control total sobre el sistema operativo?

A) AWS Lambda

**B)** **Amazon EC2**

C) AWS Fargate

D) Amazon Lightsail exclusivamente

**Respuesta correcta: B.** 

*EC2 es el servicio IaaS de AWS, entregando control completo del sistema operativo y todo el software instalado encima.*

Referencia: Parte 4

**Pregunta 10.** ¿Qué es un Auto Scaling Group?

A) Un tipo de balanceador de carga

**B)** **Una colección de instancias EC2 gestionadas conjuntamente con reglas de escalado automático (mínimo, máximo, deseado)**

C) Un servicio de almacenamiento elástico

D) Un tipo de Security Group especial

**Respuesta correcta: B.** 

*Un ASG mantiene un rango de instancias EC2 definido, ajustando la capacidad automáticamente según políticas de escalado basadas en métricas.*

Referencia: Parte 4

**Pregunta 11.** ¿Qué tipo de Elastic Load Balancer está optimizado para tráfico HTTP/HTTPS con enrutamiento avanzado basado en contenido?

A) Network Load Balancer

**B)** **Application Load Balancer**

C) Gateway Load Balancer

D) Classic Load Balancer exclusivamente

**Respuesta correcta: B.** 

*El Application Load Balancer opera en capa 7 y permite enrutamiento avanzado basado en el contenido de la petición HTTP/HTTPS.*

Referencia: Parte 4

**Pregunta 12.** ¿Qué característica define a S3 Standard-Infrequent Access frente a S3 Glacier?

**A)** **S3 Standard-IA tiene acceso instantáneo (milisegundos); Glacier tiene tiempos de recuperación de minutos a horas**

B) Ambos tienen exactamente el mismo tiempo de recuperación

C) Glacier es más caro que S3 Standard-IA

D) S3 Standard-IA no permite acceso a los datos bajo ninguna circunstancia

**Respuesta correcta: A.** 

*S3 Standard-IA ofrece menor costo con acceso instantáneo; las clases Glacier reducen aún más el costo a cambio de mayores tiempos de recuperación.*

Referencia: Parte 5

**Pregunta 13.** ¿Qué tipo de volumen EBS se recomienda para cargas de trabajo con requisitos de rendimiento de I/O muy exigentes, como bases de datos transaccionales?

A) gp2/gp3 de propósito general

**B)** **io1/io2 de IOPS provisionadas**

C) st1/sc1 tipo HDD

D) Ninguno, EBS no soporta alto rendimiento

**Respuesta correcta: B.** 

*Los volúmenes io1/io2 ofrecen IOPS provisionadas para cargas con requisitos de rendimiento muy exigentes, como bases de datos transaccionales críticas.*

Referencia: Parte 5

**Pregunta 14.** ¿Qué protocolo de red usa Amazon EFS para ser montado por múltiples instancias?

A) SMB exclusivamente

**B)** **NFS**

C) iSCSI

D) FTP

**Respuesta correcta: B.** 

*Amazon EFS es compatible con el protocolo NFS (Network File System), estándar en entornos Linux/Unix.*

Referencia: Parte 5

**Pregunta 15.** ¿Qué servicio de base de datos relacional fue diseñado por AWS con arquitectura de almacenamiento distribuido propia, compatible con MySQL y PostgreSQL?

A) Amazon RDS estándar

**B)** **Amazon Aurora**

C) Amazon DynamoDB

D) Amazon Redshift

**Respuesta correcta: B.** 

*Aurora ofrece mayor rendimiento y disponibilidad que RDS estándar gracias a su arquitectura de almacenamiento distribuido diseñada por AWS.*

Referencia: Parte 6

**Pregunta 16.** ¿Qué servicio de AWS es compatible con Redis o Memcached para reducir la carga de lecturas frecuentes sobre una base de datos?

**A)** **Amazon ElastiCache**

B) Amazon Redshift

C) AWS Batch

D) Amazon FSx

**Respuesta correcta: A.** 

*ElastiCache ofrece caché en memoria totalmente administrada, compatible con Redis o Memcached, complementando la base de datos principal.*

Referencia: Parte 6

**Pregunta 17.** ¿Qué es una Availability Zone en relación con una Región?

**A)** **Una Región contiene múltiples Availability Zones**

B) Una Availability Zone contiene múltiples Regiones

C) Son sinónimos

D) Las AZ solo existen fuera de Estados Unidos

**Respuesta correcta: A.** 

*Cada Región de AWS está compuesta por varias Availability Zones (normalmente 3 o más), físicamente aisladas pero interconectadas.*

Referencia: Parte 2

**Pregunta 18.** ¿Qué elemento de una VPC permite tráfico bidireccional completo hacia y desde subredes públicas?

A) NAT Gateway

**B)** **Internet Gateway**

C) Network ACL

D) Route 53

**Respuesta correcta: B.** 

*El Internet Gateway permite comunicación bidireccional entre internet y recursos con IP pública en subredes públicas.*

Referencia: Parte 7

**Pregunta 19.** ¿Qué diferencia principal existe entre Site-to-Site VPN y AWS Direct Connect?

A) Son exactamente lo mismo

**B)** **VPN usa internet público (cifrado, rápida de configurar); Direct Connect es una conexión física dedicada (más consistente, más lenta de aprovisionar)**

C) Direct Connect siempre es más barato que VPN

D) VPN no puede cifrar el tráfico

**Respuesta correcta: B.** 

*VPN es más rápida de implementar pero depende de internet; Direct Connect ofrece conectividad dedicada más consistente a cambio de mayor tiempo de aprovisionamiento.*

Referencia: Parte 7

**Pregunta 20.** ¿A qué nivel de la arquitectura de red opera una Network ACL?

A) Instancia individual

**B)** **Subred**

C) Región completa

D) Cuenta completa

**Respuesta correcta: B.** 

*La NACL opera a nivel de subred, aplicando sus reglas a todo el tráfico que entra o sale de esa subred.*

Referencia: Parte 7

**Pregunta 21.** Según el Modelo de Responsabilidad Compartida, ¿de quién es la responsabilidad del hipervisor y la infraestructura física?

A) Del cliente

**B)** **De AWS**

C) Compartida al 50%

D) De un proveedor externo

**Respuesta correcta: B.** 

*AWS es responsable de la 'seguridad DE la nube': infraestructura física, hipervisor y red global subyacente.*

Referencia: Parte 8

**Pregunta 22.** ¿Qué servicio permite aprovisionar certificados SSL/TLS gratuitos para usar con CloudFront o un Load Balancer?

A) AWS KMS

**B)** **AWS Certificate Manager (ACM)**

C) AWS Secrets Manager

D) Amazon Macie

**Respuesta correcta: B.** 

*ACM aprovisiona y renueva automáticamente certificados SSL/TLS públicos sin costo adicional para servicios integrados de AWS.*

Referencia: Parte 8

**Pregunta 23.** ¿Qué servicio protege contra ataques de Denegación de Servicio Distribuido (DDoS)?

A) AWS WAF

**B)** **AWS Shield**

C) Amazon GuardDuty

D) AWS Config

**Respuesta correcta: B.** 

*AWS Shield está diseñado específicamente para mitigar ataques DDoS; Shield Standard es automático y gratuito para todos los clientes.*

Referencia: Parte 8

**Pregunta 24.** ¿Qué servicio evalúa continuamente si la configuración de tus recursos cumple con reglas definidas, manteniendo un historial de cambios?

A) AWS CloudTrail

**B)** **AWS Config**

C) AWS Trusted Advisor

D) Amazon Inspector

**Respuesta correcta: B.** 

*AWS Config registra y evalúa continuamente el estado de configuración de los recursos, comparándolo contra reglas de cumplimiento definidas.*

Referencia: Parte 8

**Pregunta 25.** ¿Qué herramienta de AWS permite crear paneles visuales personalizados combinando múltiples métricas de distintos servicios?

A) CloudWatch Logs Insights

**B)** **CloudWatch Dashboards**

C) CloudWatch Alarms

D) AWS X-Ray

**Respuesta correcta: B.** 

*CloudWatch Dashboards permite combinar gráficas de múltiples métricas en un panel visual consolidado.*

Referencia: Parte 9

**Pregunta 26.** ¿Qué vista del AWS Health Dashboard muestra eventos que afectan específicamente a los recursos de tu propia cuenta?

A) Service Health

**B)** **Personal Health**

C) Trusted Advisor

D) CloudTrail Event History

**Respuesta correcta: B.** 

*La vista de 'Your account health' (Personal Health) filtra eventos operativos relevantes específicamente para los recursos de tu cuenta.*

Referencia: Parte 9

**Pregunta 27.** ¿Qué servicio permite escribir consultas interactivas similares a SQL sobre grandes volúmenes de logs almacenados en CloudWatch?

A) CloudWatch Alarms

**B)** **CloudWatch Logs Insights**

C) AWS X-Ray

D) AWS Trusted Advisor

**Respuesta correcta: B.** 

*CloudWatch Logs Insights permite filtrar, agregar y analizar grandes volúmenes de logs sin descargarlos manualmente.*

Referencia: Parte 9

**Pregunta 28.** ¿Qué servicio de AWS actúa como la puerta de entrada HTTP para exponer una API hacia clientes externos, gestionando throttling y autenticación?

A) AWS Step Functions

**B)** **Amazon API Gateway**

C) Amazon SQS

D) Amazon EventBridge

**Respuesta correcta: B.** 

*API Gateway gestiona la capa HTTP de una API (autenticación, throttling, enrutamiento), frecuentemente combinado con Lambda.*

Referencia: Parte 10

**Pregunta 29.** ¿Qué patrón de mensajería implementa Amazon SNS?

A) Colas punto a punto

**B)** **Publicación/suscripción (fan-out a múltiples destinos)**

C) Orquestación de flujos de trabajo

D) Bus de eventos con reglas de contenido

**Respuesta correcta: B.** 

*SNS distribuye un mensaje publicado a todos los suscriptores de un tópico simultáneamente (fan-out).*

Referencia: Parte 10

**Pregunta 30.** ¿Cuál es el modelo de precios de AWS Lambda?

A) Precio fijo mensual sin importar el uso

**B)** **Pago por invocación y por tiempo de ejecución multiplicado por la memoria asignada**

C) Pago único de por vida

D) Gratuito en cualquier volumen de uso

**Respuesta correcta: B.** 

*Lambda cobra por el número de invocaciones y la duración/memoria consumida durante cada ejecución, sin costo si no se invoca.*

Referencia: Parte 4 y 11

**Pregunta 31.** ¿Qué herramienta de AWS te permite definir un umbral de gasto y recibir alertas automáticas cuando el gasto real o proyectado se acerca a ese umbral?

A) AWS Cost Explorer

**B)** **AWS Budgets**

C) AWS Organizations

D) Reserved Instances

**Respuesta correcta: B.** 

*AWS Budgets permite crear presupuestos y configurar alertas automáticas basadas en gasto real o proyectado.*

Referencia: Parte 11

**Pregunta 32.** ¿Qué pilar del Well-Architected Framework se enfoca en ejecutar y monitorear sistemas para entregar valor de negocio, mejorando procesos continuamente?

A) Seguridad

**B)** **Excelencia Operacional**

C) Sostenibilidad

D) Eficiencia del Rendimiento

**Respuesta correcta: B.** 

*Excelencia Operacional abarca automatización de cambios, respuesta a eventos, y mejora continua de procesos operativos.*

Referencia: Parte 12

**Pregunta 33.** ¿Qué servicio permite definir infraestructura usando lenguajes de programación de propósito general, sintetizando hacia CloudFormation?

A) AWS Config

**B)** **AWS Cloud Development Kit (CDK)**

C) AWS Control Tower

D) AWS Backup

**Respuesta correcta: B.** 

*CDK permite escribir infraestructura en TypeScript, Python, Java, etc., generando plantillas de CloudFormation internamente.*

Referencia: Parte 13

**Pregunta 34.** ¿Qué servicio replica continuamente servidores on-premises hacia AWS para recuperación ante desastres con RTO/RPO mínimos?

A) AWS Backup

**B)** **AWS Elastic Disaster Recovery**

C) AWS Migration Hub

D) AWS DataSync

**Respuesta correcta: B.** 

*AWS DRS replica servidores de forma continua, permitiendo un failover rápido hacia AWS en caso de desastre del entorno de origen.*

Referencia: Parte 13

**Pregunta 35.** ¿Cuál de los siguientes es un ejemplo de FaaS (Function as a Service)?

A) Una instancia EC2 corriendo 24/7

**B)** **AWS Lambda ejecutando código solo cuando se dispara un evento**

C) Una base de datos RDS con Multi-AZ

D) Un bucket S3 con versionado

**Respuesta correcta: B.** 

*FaaS ejecuta funciones solo en respuesta a eventos, sin servidor visible ni siquiera de forma indirecta para el cliente.*

Referencia: Parte 1 y 4

**Pregunta 36.** ¿Qué diferencia a la escalabilidad vertical de la escalabilidad horizontal?

A) Son sinónimos exactos

**B)** **Vertical = más recursos a UNA misma instancia; Horizontal = añadir MÁS instancias en paralelo**

C) Horizontal siempre requiere downtime; vertical nunca lo requiere

D) La escalabilidad vertical no existe en AWS

**Respuesta correcta: B.** 

*Escalar verticalmente aumenta recursos de un solo servidor (con límite físico); escalar horizontalmente añade más servidores en paralelo.*

Referencia: Parte 1

**Pregunta 37.** ¿Qué servicio de AWS simplifica el despliegue de aplicaciones sencillas con precios mensuales fijos y configuración de red simplificada?

A) Amazon EKS

**B)** **Amazon Lightsail**

C) AWS Batch

D) Amazon Redshift

**Respuesta correcta: B.** 

*Lightsail está diseñado para simplicidad y precios predecibles, ideal para proyectos pequeños o principiantes.*

Referencia: Parte 4

**Pregunta 38.** ¿Qué recurso de almacenamiento vive dentro de una única Availability Zone específica y no puede adjuntarse directamente a instancias en otra AZ?

A) Amazon S3

**B)** **Amazon EBS**

C) Amazon EFS

D) AWS Storage Gateway

**Respuesta correcta: B.** 

*Un volumen EBS vive en una AZ específica y solo puede adjuntarse a instancias EC2 de esa misma AZ.*

Referencia: Parte 5

**Pregunta 39.** ¿Qué servicio de AWS convierte el esquema y código de una base de datos Oracle hacia la sintaxis de Aurora PostgreSQL en una migración heterogénea?

A) AWS DMS

**B)** **AWS Schema Conversion Tool (SCT)**

C) AWS DataSync

D) Amazon Migration Hub

**Respuesta correcta: B.** 

*SCT convierte esquema y código (procedimientos, vistas) de la base de datos de origen al motor de destino; DMS migra los datos.*

Referencia: Parte 13

**Pregunta 40.** ¿Qué describe mejor el propósito de AWS Backup?

A) Replicar servidores completos de forma continua para DR

**B)** **Centralizar y automatizar copias de seguridad de múltiples servicios de AWS desde un único lugar**

C) Migrar bases de datos entre motores distintos

D) Transferir datos físicamente mediante dispositivos

**Respuesta correcta: B.** 

*AWS Backup centraliza la gestión de copias de seguridad de EBS, RDS, DynamoDB, EFS, entre otros, con políticas definidas centralmente.*

Referencia: Parte 13

**Pregunta 41.** ¿Qué es la elasticidad, en contraste con la simple escalabilidad?

**A)** **Escalabilidad + automatismo + reversibilidad (crece y decrece solo)**

B) Un sinónimo exacto de tolerancia a fallos

C) La capacidad de un sistema de nunca fallar

D) Un servicio específico de AWS

**Respuesta correcta: A.** 

*La elasticidad añade automatismo y reversibilidad a la escalabilidad: el sistema ajusta capacidad solo, tanto hacia arriba como hacia abajo.*

Referencia: Parte 1

**Pregunta 42.** ¿Qué es responsabilidad del cliente en un servicio totalmente administrado como AWS Lambda, según el Modelo de Responsabilidad Compartida?

A) Parchear el sistema operativo subyacente

**B)** **El código de la función y la configuración de IAM/datos asociados**

C) La infraestructura física de los data centers

D) El hipervisor

**Respuesta correcta: B.** 

*Incluso en servicios muy administrados como Lambda, el cliente sigue siendo responsable de su código, sus datos y la configuración de IAM.*

Referencia: Parte 8

**Pregunta 43.** ¿Qué servicio ayuda a identificar instancias EC2 subutilizadas que podrían redimensionarse para ahorrar costos?

**A)** **AWS Trusted Advisor, categoría de optimización de costos**

B) AWS Shield

C) Amazon Macie

D) AWS Certificate Manager

**Respuesta correcta: A.** 

*Trusted Advisor analiza el uso real de recursos y recomienda redimensionar o detener instancias subutilizadas.*

Referencia: Parte 9 y 11

**Pregunta 44.** ¿Qué combinación de servicios formaría una arquitectura de tres capas estándar en AWS?

**A)** **ALB en subred pública, servidores de aplicación en subred privada, base de datos en subred privada más restringida**

B) Todo en una sola subred pública sin separación

C) Todo en subredes privadas sin ningún Load Balancer

D) Solo Lambda sin ninguna VPC

**Respuesta correcta: A.** 

*La arquitectura de tres capas estándar separa el Load Balancer (público), la aplicación (privada) y la base de datos (privada, más restringida).*

Referencia: Parte 7

**Pregunta 45.** ¿Qué describe mejor el propósito de un Dead Letter Queue en SQS?

A) Eliminar mensajes automáticamente cada hora

**B)** **Recibir mensajes que fallan su procesamiento repetidamente, evitando bloquear la cola principal**

C) Duplicar mensajes automáticamente

D) Cifrar mensajes en tránsito

**Respuesta correcta: B.** 

*Una DLQ aísla mensajes problemáticos tras varios intentos fallidos, permitiendo su análisis sin bloquear el flujo normal.*

Referencia: Parte 10

**Pregunta 46.** ¿Qué modelo de precios de EC2 comprometes un monto de gasto constante por hora, aplicándose de forma flexible sobre el uso real?

A) Reserved Instances

**B)** **Savings Plans**

C) On-Demand

D) Instancias Dedicadas

**Respuesta correcta: B.** 

*Savings Plans comprometen un gasto ($/hora) en vez de un tipo de instancia específico, ofreciendo más flexibilidad que Reserved Instances.*

Referencia: Parte 11

**Pregunta 47.** ¿Qué beneficio ofrece la facturación consolidada de AWS Organizations?

A) Elimina la necesidad de pagar por cualquier servicio

**B)** **Combina el uso de todas las cuentas miembro para calcular descuentos por volumen de forma agregada**

C) Solo funciona con instancias Spot

D) Requiere que todas las cuentas usen los mismos servicios

**Respuesta correcta: B.** 

*La facturación consolidada agrega el uso de todas las cuentas para alcanzar más rápido los umbrales de descuento por volumen.*

Referencia: Parte 11

**Pregunta 48.** ¿Qué recomienda el pilar de Fiabilidad respecto a probar los procedimientos de recuperación?

A) Esperar a un fallo real para descubrir si el plan funciona

**B)** **Probar automáticamente los procedimientos de recuperación mediante simulacros controlados**

C) Nunca automatizar la recuperación

D) Evitar cualquier tipo de backup

**Respuesta correcta: B.** 

*El pilar de Fiabilidad recomienda probar proactivamente la recuperación mediante fallos simulados, en vez de descubrir fallas durante un incidente real.*

Referencia: Parte 12

**Pregunta 49.** ¿Qué diferencia a AWS Snowball de AWS Snowmobile?

A) Son el mismo servicio

**B)** **Snowball transfiere decenas de TB por dispositivo; Snowmobile transporta volúmenes de hasta exabytes en un contenedor completo**

C) Snowmobile es un servicio de bases de datos

D) Snowball requiere conexión a internet obligatoria

**Respuesta correcta: B.** 

*Snowball es un dispositivo físico estándar; Snowmobile es para migraciones verdaderamente masivas, transportado en camión.*

Referencia: Parte 13

**Pregunta 50.** ¿Qué es cierto sobre la transferencia de datos entrante hacia AWS desde internet?

A) Siempre tiene un costo significativo

**B)** **Es gratuita en la gran mayoría de los casos**

C) Solo es gratuita los fines de semana

D) Depende exclusivamente del tipo de instancia EC2

**Respuesta correcta: B.** 

*La transferencia de datos entrante hacia AWS es gratuita en la gran mayoría de los servicios, a diferencia de la saliente hacia internet.*

Referencia: Parte 11

**Pregunta 51.** ¿Qué servicio de AWS es un bus de eventos serverless que integra fuentes de AWS, aplicaciones propias, y SaaS de terceros?

A) Amazon SQS

**B)** **Amazon EventBridge**

C) AWS Step Functions

D) Amazon API Gateway

**Respuesta correcta: B.** 

*EventBridge recibe eventos de múltiples fuentes (incluyendo SaaS de terceros) y los enruta según reglas basadas en contenido.*

Referencia: Parte 10

**Pregunta 52.** ¿Qué es cierto sobre el usuario root de una cuenta de AWS?

A) Debería usarse para las tareas diarias del equipo

**B)** **Tiene control total e irrestricto y debería protegerse con MFA, usándose solo para tareas excepcionales**

C) No puede eliminarse ni tiene permisos especiales

D) Es lo mismo que un IAM Role

**Respuesta correcta: B.** 

*El usuario root tiene acceso completo e irrestricto; AWS recomienda protegerlo con MFA y reservarlo para tareas que estrictamente lo requieran.*

Referencia: Parte 3

**Pregunta 53.** ¿Qué diferencia a un IAM User de un IAM Role en cuanto a sus credenciales?

A) Ambos tienen credenciales idénticas

**B)** **User = credenciales permanentes; Role = credenciales temporales generadas al asumirse**

C) Role = credenciales permanentes; User = credenciales temporales

D) Ninguno de los dos tiene credenciales

**Respuesta correcta: B.** 

*Un User tiene credenciales de larga duración; un Role no tiene credenciales propias, se asume generando credenciales temporales vía STS.*

Referencia: Parte 3

**Pregunta 54.** ¿Qué servicio ofrecería visibilidad de qué porcentaje de un límite de servicio (como número de VPCs) está usando una cuenta?

**A)** **AWS Trusted Advisor, categoría de límites de servicio**

B) AWS X-Ray

C) Amazon CloudWatch Logs Insights

D) AWS Certificate Manager

**Respuesta correcta: A.** 

*Trusted Advisor incluye una categoría de Service Limits que compara el uso actual contra las cuotas establecidas por AWS.*

Referencia: Parte 9

**Pregunta 55.** ¿Qué servicio sería el más adecuado para procesar imágenes subidas a un bucket S3 de forma automática, sin mantener servidores encendidos permanentemente?

A) Amazon EC2 con una instancia siempre encendida

**B)** **AWS Lambda disparado por un evento de S3**

C) Amazon Redshift

D) AWS Direct Connect

**Respuesta correcta: B.** 

*Lambda disparado por eventos de S3 procesa cada archivo subido sin necesidad de mantener ningún servidor corriendo permanentemente.*

Referencia: Parte 4 y 10

**Pregunta 56.** ¿Qué recomienda AWS respecto a elegir Región cuando la latencia lo permite, dentro del pilar de Sostenibilidad?

A) Elegir siempre la Región más cara

**B)** **Considerar Regiones con mayor proporción de energía renovable, cuando cumplimiento y latencia lo permitan**

C) La elección de Región no tiene relación con sostenibilidad

D) Elegir siempre la Región con más AZ sin importar otros factores

**Respuesta correcta: B.** 

*El pilar de Sostenibilidad sugiere considerar la matriz energética de la Región, siempre que otros requisitos como cumplimiento y latencia lo permitan.*

Referencia: Parte 12

**Pregunta 57.** ¿Qué servicio administrado de AWS soporta tanto migraciones homogéneas como heterogéneas de bases de datos, manteniendo la fuente operativa durante el proceso?

A) AWS DataSync

**B)** **AWS Database Migration Service (DMS)**

C) Amazon Migration Hub

D) AWS Snowball

**Respuesta correcta: B.** 

*DMS migra bases de datos manteniendo la fuente operativa, soportando migraciones tanto entre el mismo motor como entre motores distintos (con SCT).*

Referencia: Parte 13

**Pregunta 58.** ¿Qué elemento de diseño ilustra mejor el principio de 'defensa en profundidad'?

A) Confiar únicamente en un Security Group sin ninguna otra capa

**B)** **Combinar IAM de mínimo privilegio, Security Groups, NACL y cifrado de datos como capas complementarias**

C) Usar solo cifrado, sin controles de acceso

D) Deshabilitar todos los logs para simplificar

**Respuesta correcta: B.** 

*La defensa en profundidad combina múltiples capas de seguridad independientes, de forma que el fallo de una no deje el sistema completamente expuesto.*

Referencia: Parte 3, 7 y 8

**Pregunta 59.** ¿Qué servicio sería el más adecuado para una empresa que quiere estructurar la creación de nuevas cuentas de AWS con gobernanza preconfigurada desde el inicio?

**A)** **AWS Control Tower**

B) Amazon CloudWatch

C) AWS Certificate Manager

D) Amazon Route 53

**Respuesta correcta: A.** 

*Control Tower automatiza una zona de aterrizaje multi-cuenta con barreras de gobernanza (guardrails) ya aplicadas desde la creación de cada cuenta.*

Referencia: Parte 13

**Pregunta 60.** ¿Qué modelo de servicio en la nube deja al cliente administrar el sistema operativo y todo el software encima, mientras AWS administra la virtualización y el hardware?

A) SaaS

B) PaaS

**C)** **IaaS**

D) FaaS

**Respuesta correcta: C.** 

*IaaS (como EC2) entrega infraestructura básica; el cliente administra SO, runtime y aplicación, mientras AWS administra la capa física y de virtualización.*

Referencia: Parte 1

**Pregunta 61.** ¿Qué diferencia a S3 One Zone-IA de S3 Standard-IA?

A) Son idénticas en todo

**B)** **One Zone-IA almacena datos en una sola AZ (menor costo, menor resiliencia); Standard-IA replica entre múltiples AZ**

C) Standard-IA es más cara pero menos duradera

D) One Zone-IA no permite ningún acceso a los datos

**Respuesta correcta: B.** 

*S3 One Zone-IA reduce el costo al almacenar en una sola AZ, apto para datos recreables; Standard-IA mantiene redundancia entre múltiples AZ.*

Referencia: Parte 5

**Pregunta 62.** ¿Qué servicio de AWS ofrece backups automáticos y Multi-AZ de forma nativa para bases de datos relacionales administradas?

**A)** **Amazon RDS**

B) Amazon Neptune exclusivamente

C) AWS Batch

D) Amazon Lightsail

**Respuesta correcta: A.** 

*RDS ofrece backups automáticos configurables y la opción de Multi-AZ para alta disponibilidad de forma nativa administrada.*

Referencia: Parte 6

**Pregunta 63.** ¿Qué elemento de seguridad de red permite tanto reglas Allow como Deny explícitas, evaluadas en orden numérico?

A) Security Group

**B)** **Network ACL**

C) IAM Policy

D) AWS Shield

**Respuesta correcta: B.** 

*La Network ACL admite reglas Allow y Deny, evaluadas en orden numérico ascendente hasta la primera coincidencia.*

Referencia: Parte 7

**Pregunta 64.** ¿Qué servicio permite a un desarrollador consultar programáticamente el estado operativo de los servicios de AWS que usa su aplicación?

**A)** **AWS Health Dashboard / Health API**

B) AWS Certificate Manager

C) Amazon Route 53

D) AWS Direct Connect

**Respuesta correcta: A.** 

*El AWS Health Dashboard (y su API asociada) permite consultar el estado operativo de los servicios de AWS relevantes para la cuenta.*

Referencia: Parte 9

**Pregunta 65.** ¿Qué describe mejor el propósito de AWS Schema Conversion Tool (SCT) en una migración de base de datos?

A) Migrar los datos en sí desde el origen hacia el destino

**B)** **Convertir el esquema y código (procedimientos almacenados, vistas) de la base de datos de origen a la sintaxis del motor de destino**

C) Transferir archivos físicamente mediante un dispositivo

D) Centralizar copias de seguridad de múltiples servicios

**Respuesta correcta: B.** 

*SCT convierte esquema y código entre motores distintos; AWS DMS es quien migra los datos en sí durante el proceso de migración.*

Referencia: Parte 13

## Hoja de respuestas rápida

| # | # | # | # | # |
| --- | --- | --- | --- | --- |
| 1: B | 2: B | 3: B | 4: B | 5: B |
| 6: C | 7: B | 8: B | 9: B | 10: B |
| 11: B | 12: A | 13: B | 14: B | 15: B |
| 16: A | 17: A | 18: B | 19: B | 20: B |
| 21: B | 22: B | 23: B | 24: B | 25: B |
| 26: B | 27: B | 28: B | 29: B | 30: B |
| 31: B | 32: B | 33: B | 34: B | 35: B |
| 36: B | 37: B | 38: B | 39: B | 40: B |
| 41: A | 42: B | 43: A | 44: A | 45: B |
| 46: B | 47: B | 48: B | 49: B | 50: B |
| 51: B | 52: B | 53: B | 54: A | 55: B |
| 56: B | 57: B | 58: B | 59: A | 60: C |
| 61: B | 62: A | 63: B | 64: A | 65: B |
