# AWS Certified Cloud Practitioner (CLF-C02)

**Simulacro de Examen 5 de 5 — 65 preguntas**

Mismo nivel de dificultad y distribución de dominios que el examen oficial CLF-C02: Cloud Concepts, Security and Compliance, Cloud Technology and Services, y Billing and Pricing. Cada pregunta incluye la respuesta correcta, una explicación, y una referencia al capítulo de la guía donde puedes repasar el tema si fallaste.

> **Cómo usar este simulacro:** Resuélvelo primero completo, sin mirar las respuestas, cronometrando 90 minutos como en el examen real. Después revisa cada pregunta, prestando especial atención a las que fallaste, y repasa el capítulo referenciado antes de tu siguiente simulacro.

## Preguntas

**Pregunta 1.** ¿Qué característica esencial del cloud computing permite que múltiples clientes compartan de forma segura el mismo hardware físico subyacente?

A) Servicio medido

**B)** **Pool de recursos compartidos (resource pooling)**

C) Autoservicio bajo demanda

D) Acceso amplio a la red

**Respuesta correcta: B.** 

*El pool de recursos compartidos, habilitado por la virtualización, permite que múltiples clientes (multi-tenant) usen el mismo hardware físico de forma aislada y segura.*

Referencia: Parte 1

**Pregunta 2.** ¿Qué beneficio de negocio describe mejor el hecho de que AWS traslade parte de sus economías de escala a los clientes mediante reducciones de precio recurrentes?

A) Ir global en minutos

**B)** **Beneficiarse de economías de escala masivas**

C) Alta disponibilidad

D) Recuperación ante desastres

**Respuesta correcta: B.** 

*AWS agrega el uso de miles de clientes para obtener mejores precios de proveedores, trasladando parte de ese ahorro mediante reducciones de precio.*

Referencia: Parte 1

**Pregunta 3.** ¿Qué elemento de la infraestructura global de AWS es el más numeroso, usado principalmente por CloudFront y Route 53?

A) Regiones

B) Availability Zones

**C)** **Edge Locations**

D) Local Zones

**Respuesta correcta: C.** 

*Las Edge Locations son mucho más numerosas que Regiones o AZ, distribuidas globalmente para reducir la latencia de entrega de contenido.*

Referencia: Parte 2

**Pregunta 4.** ¿Qué herramienta de AWS sería la más adecuada para que un desarrollador explore por primera vez, de forma visual, cómo se relacionan los recursos de una VPC recién creada?

A) AWS CLI

**B)** **AWS Management Console**

C) Un AWS SDK

D) Llamadas directas a la API

**Respuesta correcta: B.** 

*La consola es ideal para exploración visual inicial y aprendizaje, mostrando claramente la relación entre recursos.*

Referencia: Parte 2

**Pregunta 5.** ¿Qué elemento de una IAM Policy especifica sobre qué recurso exacto aplican los permisos, usando su ARN?

A) Effect

B) Action

**C)** **Resource**

D) Version

**Respuesta correcta: C.** 

*El elemento 'Resource' de una policy especifica, mediante el ARN, sobre qué recurso(s) exacto(s) aplican las acciones permitidas o denegadas.*

Referencia: Parte 3

**Pregunta 6.** ¿Qué herramienta de IAM muestra qué servicios ha usado realmente una identidad en los últimos meses, ayudando a aplicar mínimo privilegio?

A) CloudTrail exclusivamente

**B)** **IAM Access Advisor (último acceso)**

C) AWS Shield

D) Amazon Route 53

**Respuesta correcta: B.** 

*El reporte de 'último acceso' (Access Advisor) de IAM muestra qué servicios ha usado realmente una identidad, ayudando a identificar permisos no utilizados.*

Referencia: Parte 3

**Pregunta 7.** ¿Qué servicio de cómputo tiene un límite máximo de tiempo de ejecución por invocación, actualmente de 15 minutos?

A) Amazon EC2

**B)** **AWS Lambda**

C) Amazon Lightsail

D) AWS Batch

**Respuesta correcta: B.** 

*Lambda tiene un límite máximo de tiempo de ejecución por invocación, por lo que no es adecuado para procesos de muy larga duración.*

Referencia: Parte 4

**Pregunta 8.** ¿Qué combinación de servicios de cómputo sería la más adecuada para un equipo con amplia experiencia en Kubernetes que migra sus cargas de contenedores a AWS sin administrar servidores?

A) ECS con tipo de lanzamiento EC2

**B)** **EKS con Fargate**

C) AWS Batch exclusivamente

D) Amazon Lightsail Containers

**Respuesta correcta: B.** 

*EKS ofrece compatibilidad total con Kubernetes, y combinado con Fargate elimina la necesidad de administrar servidores del clúster.*

Referencia: Parte 4

**Pregunta 9.** ¿Qué característica define a las instancias Spot en cuanto a la certeza de disponibilidad continua?

A) Garantizan disponibilidad continua sin ninguna interrupción posible

**B)** **Pueden ser interrumpidas por AWS con aproximadamente 2 minutos de aviso cuando se necesita la capacidad de vuelta**

C) Requieren un compromiso mínimo de 6 meses

D) Solo están disponibles para bases de datos

**Respuesta correcta: B.** 

*Las instancias Spot pueden interrumpirse con poco aviso (2 minutos) cuando AWS necesita recuperar esa capacidad, a cambio de grandes descuentos.*

Referencia: Parte 4 y 11

**Pregunta 10.** ¿Qué clase de almacenamiento S3 almacena datos en una sola Availability Zone, reduciendo el costo a cambio de menor resiliencia?

A) S3 Standard

**B)** **S3 One Zone-IA**

C) S3 Glacier Flexible Retrieval

D) S3 Intelligent-Tiering

**Respuesta correcta: B.** 

*S3 One Zone-IA reduce costos al no replicar entre múltiples AZ, apto para datos de acceso infrecuente que pueden recrearse si se pierden.*

Referencia: Parte 5

**Pregunta 11.** ¿Qué tipo de volumen EBS es más adecuado para cargas de trabajo secuenciales de gran volumen y bajo costo, como procesamiento de big data?

A) gp3 de propósito general

B) io2 de IOPS provisionadas

**C)** **st1 tipo HDD optimizado para throughput**

D) Ninguno, EBS no soporta HDD

**Respuesta correcta: C.** 

*Los volúmenes st1 (HDD) están optimizados para cargas secuenciales de alto throughput y menor costo, como big data o logs.*

Referencia: Parte 5

**Pregunta 12.** ¿Qué servicio de AWS permitiría a una aplicación en EC2 leer y escribir en un sistema de archivos compartido montado simultáneamente por 30 instancias en 3 AZ distintas?

A) Amazon EBS con Multi-Attach en un solo volumen

**B)** **Amazon EFS**

C) AWS Snowball

D) Amazon Redshift

**Respuesta correcta: B.** 

*EFS está diseñado exactamente para este escenario: sistema de archivos NFS compartido, montable simultáneamente por múltiples instancias en distintas AZ.*

Referencia: Parte 5

**Pregunta 13.** ¿Qué modo de capacidad de DynamoDB requiere que el cliente defina de antemano las unidades de lectura/escritura necesarias, con opción de Auto Scaling?

A) On-Demand

**B)** **Provisioned**

C) Reserved Capacity exclusivamente

D) DynamoDB no ofrece modos de capacidad

**Respuesta correcta: B.** 

*El modo Provisioned requiere definir de antemano la capacidad de lectura/escritura, pudiendo combinarse con Auto Scaling para ajustarla automáticamente.*

Referencia: Parte 6

**Pregunta 14.** ¿Qué servicio sería el más adecuado para almacenar y consultar el estado de sesión de millones de jugadores simultáneos en un videojuego online, con latencia mínima?

A) Amazon Redshift

**B)** **Amazon DynamoDB**

C) Amazon Neptune

D) AWS Batch

**Respuesta correcta: B.** 

*DynamoDB ofrece latencia de un solo dígito de milisegundo a cualquier escala con un modelo clave-valor, ideal para estado de sesión de alta concurrencia.*

Referencia: Parte 6

**Pregunta 15.** ¿Qué combinación de RDS Multi-AZ y Read Replicas describiría correctamente el uso de ambas simultáneamente?

A) No pueden usarse juntas en la misma base de datos

**B)** **Multi-AZ para alta disponibilidad y Read Replicas para escalar lecturas, ambas pueden coexistir en la misma arquitectura**

C) Read Replicas reemplazan completamente la necesidad de Multi-AZ

D) Multi-AZ y Read Replicas son exactamente lo mismo

**Respuesta correcta: B.** 

*Multi-AZ (alta disponibilidad) y Read Replicas (escalado de lecturas) resuelven necesidades distintas y complementarias, pudiendo coexistir en la misma arquitectura.*

Referencia: Parte 6

**Pregunta 16.** ¿Qué componente de una VPC se adjunta una sola vez por VPC y permite tráfico bidireccional hacia subredes públicas?

A) NAT Gateway (puede haber varios)

**B)** **Internet Gateway (uno por VPC)**

C) Network ACL

D) Route Table

**Respuesta correcta: B.** 

*El Internet Gateway se adjunta una vez a nivel de VPC completa, habilitando tráfico bidireccional para las subredes públicas que enruten hacia él.*

Referencia: Parte 7

**Pregunta 17.** ¿Qué servicio combinaría con Direct Connect como respaldo (failover) en caso de que la conexión dedicada falle?

A) Amazon CloudFront

**B)** **AWS Site-to-Site VPN**

C) Amazon Route 53 exclusivamente

D) AWS Certificate Manager

**Respuesta correcta: B.** 

*Es común usar Site-to-Site VPN como respaldo (failover) de una conexión Direct Connect primaria, manteniendo conectividad si la línea dedicada falla.*

Referencia: Parte 7

**Pregunta 18.** ¿Qué es cierto sobre las reglas de una Network ACL en cuanto a su evaluación?

A) Se evalúan todas simultáneamente de forma aditiva, como los Security Groups

**B)** **Se evalúan en orden numérico ascendente, aplicándose la primera regla que coincida**

C) Solo se evalúa la última regla de la lista

D) El orden de las reglas no tiene ningún efecto

**Respuesta correcta: B.** 

*Las reglas de una NACL se evalúan en orden numérico, y se aplica la primera coincidencia, a diferencia de los Security Groups que son aditivos.*

Referencia: Parte 7

**Pregunta 19.** ¿Qué es responsabilidad de AWS, y NO del cliente, en cualquier servicio de AWS sin excepción?

A) La configuración de IAM del cliente

**B)** **La infraestructura física global (data centers, hardware, energía)**

C) El cifrado de los datos del cliente

D) El código de la aplicación del cliente

**Respuesta correcta: B.** 

*La infraestructura física global es responsabilidad exclusiva de AWS ('seguridad DE la nube'), sin importar el servicio usado.*

Referencia: Parte 8

**Pregunta 20.** ¿Qué servicio permitiría bloquear automáticamente una IP que excede 100 peticiones por minuto hacia una API pública?

A) AWS Shield Standard exclusivamente

**B)** **AWS WAF con una regla basada en tasa (rate-based rule)**

C) Amazon GuardDuty

D) AWS Config

**Respuesta correcta: B.** 

*AWS WAF admite reglas basadas en tasa que bloquean automáticamente IPs que excedan un número de peticiones definido en una ventana de tiempo.*

Referencia: Parte 8

**Pregunta 21.** ¿Qué servicio ayudaría a demostrar en una auditoría exactamente qué usuario de IAM modificó una Security Group específica y en qué momento?

A) Amazon GuardDuty

**B)** **AWS CloudTrail**

C) Amazon Macie

D) AWS Certificate Manager

**Respuesta correcta: B.** 

*CloudTrail registra el historial detallado de llamadas a la API, incluyendo qué usuario realizó una acción específica y cuándo.*

Referencia: Parte 8

**Pregunta 22.** ¿Qué servicio evaluaría si un volumen EBS cumple continuamente con la regla 'todo volumen debe estar cifrado', alertando si deja de cumplirla?

A) AWS CloudTrail

**B)** **AWS Config**

C) Amazon Inspector

D) AWS Shield

**Respuesta correcta: B.** 

*AWS Config evalúa continuamente la configuración de los recursos contra reglas definidas, alertando sobre desviaciones del cumplimiento esperado.*

Referencia: Parte 8

**Pregunta 23.** ¿Qué servicio de observabilidad sería el más adecuado para escribir una consulta similar a SQL sobre millones de líneas de logs de una función Lambda?

A) CloudWatch Alarms

**B)** **CloudWatch Logs Insights**

C) AWS X-Ray exclusivamente

D) AWS Trusted Advisor

**Respuesta correcta: B.** 

*CloudWatch Logs Insights permite consultas interactivas sobre grandes volúmenes de logs sin descargarlos manualmente.*

Referencia: Parte 9

**Pregunta 24.** ¿Qué diferencia a la resolución 'estándar' de una métrica de CloudWatch (1 minuto) de la resolución 'de alta frecuencia' (hasta 1 segundo)?

A) No existe tal diferencia

**B)** **La alta resolución permite detectar cambios más rápidos, a cambio de mayor costo por más puntos de datos almacenados**

C) La alta resolución solo aplica a S3

D) La resolución no afecta el costo de CloudWatch

**Respuesta correcta: B.** 

*CloudWatch permite publicar métricas con resolución estándar o de alta frecuencia (hasta 1 segundo), esta última con mayor costo por más puntos de datos.*

Referencia: Parte 9

**Pregunta 25.** ¿Qué nivel de soporte de AWS es necesario para acceder al conjunto COMPLETO de verificaciones de Trusted Advisor?

A) Basic Support (gratuito) da acceso completo

**B)** **Business o Enterprise Support (de pago)**

C) Ningún plan da acceso a Trusted Advisor

D) Solo mediante un ticket manual de soporte

**Respuesta correcta: B.** 

*El plan Basic Support solo da acceso a un subconjunto limitado de verificaciones; el conjunto completo requiere Business o Enterprise Support.*

Referencia: Parte 9

**Pregunta 26.** ¿Qué servicio de integración sería el más adecuado para notificar simultáneamente por email, SMS y a una cola SQS cuando se confirma un pedido?

A) Amazon SQS exclusivamente

**B)** **Amazon SNS, con los tres tipos de suscriptores configurados en el mismo tópico**

C) AWS Step Functions exclusivamente

D) Amazon Route 53

**Respuesta correcta: B.** 

*SNS permite múltiples tipos de suscriptores simultáneos (email, SMS, SQS, Lambda) en el mismo tópico, logrando el patrón fan-out desde un único evento.*

Referencia: Parte 10

**Pregunta 27.** ¿Qué tipo de cola SQS ofrece el mayor throughput, a cambio de no garantizar un orden estricto de entrega?

A) SQS FIFO

**B)** **SQS Standard**

C) SNS FIFO

D) SNS Standard

**Respuesta correcta: B.** 

*Las colas SQS Standard priorizan el máximo throughput, sin garantía estricta de orden, a diferencia de las colas FIFO.*

Referencia: Parte 10

**Pregunta 28.** ¿Qué describe mejor el rol de AWS Step Functions frente a construir la lógica de orquestación manualmente dentro de una función Lambda controladora?

A) Step Functions elimina la necesidad de Lambda por completo

**B)** **Step Functions externaliza la lógica de orquestación con visualización nativa, reintentos y manejo de errores por paso**

C) No existe ninguna diferencia práctica entre ambos enfoques

D) Step Functions solo funciona sin Lambda

**Respuesta correcta: B.** 

*Step Functions saca la lógica de orquestación del código, ofreciendo visualización, reintentos y manejo de errores nativo por cada paso del flujo.*

Referencia: Parte 10

**Pregunta 29.** ¿Qué modelo de precios de EC2 requiere el mayor compromiso pero ofrece el mayor descuento garantizado para uso constante a largo plazo?

A) On-Demand

B) Spot Instances

**C)** **Reserved Instances o Savings Plans a 3 años con pago total por adelantado**

D) AWS Free Tier

**Respuesta correcta: C.** 

*Un compromiso de 3 años con pago total por adelantado maximiza el descuento frente a On-Demand para cargas de trabajo constantes y predecibles.*

Referencia: Parte 11

**Pregunta 30.** ¿Qué herramienta de AWS ayudaría a responder '¿cuánto gastamos en RDS el trimestre pasado, desglosado por equipo usando etiquetas?'

A) AWS Organizations exclusivamente

**B)** **AWS Cost Explorer, filtrando por servicio y agrupando por cost allocation tag**

C) AWS Shield

D) Amazon GuardDuty

**Respuesta correcta: B.** 

*Cost Explorer permite filtrar por servicio y periodo, y agrupar por etiquetas de asignación de costos previamente configuradas.*

Referencia: Parte 11

**Pregunta 31.** ¿Qué pilar del Well-Architected Framework abarca la automatización de despliegues y la práctica de simulacros de respuesta a incidentes ('game days')?

A) Seguridad

**B)** **Excelencia Operacional**

C) Sostenibilidad

D) Eficiencia del Rendimiento

**Respuesta correcta: B.** 

*Excelencia Operacional incluye automatizar cambios y practicar la respuesta a fallos mediante simulacros controlados como 'game days'.*

Referencia: Parte 12

**Pregunta 32.** ¿Qué pilar del Well-Architected Framework recomienda maximizar la utilización de recursos aprovisionados para minimizar el impacto ambiental?

A) Optimización de Costos exclusivamente, sin relación con sostenibilidad

**B)** **Sostenibilidad**

C) Seguridad

D) Fiabilidad

**Respuesta correcta: B.** 

*El pilar de Sostenibilidad recomienda maximizar la utilización de recursos, evitando capacidad ociosa que consume energía sin generar valor.*

Referencia: Parte 12

**Pregunta 33.** ¿Qué servicio de AWS permitiría desplegar de forma reproducible la misma arquitectura de red en un entorno de desarrollo y en uno de producción, evitando diferencias por configuración manual?

**A)** **AWS CloudFormation**

B) AWS Trusted Advisor

C) Amazon CloudWatch

D) AWS Certificate Manager

**Respuesta correcta: A.** 

*CloudFormation permite reutilizar la misma plantilla declarativa para desplegar entornos idénticos, evitando inconsistencias por configuración manual.*

Referencia: Parte 13

**Pregunta 34.** ¿Qué servicio se usaría para migrar un servidor SQL Server on-premises hacia Amazon RDS for SQL Server, manteniendo la fuente operativa durante la migración?

A) AWS DataSync

**B)** **AWS Database Migration Service (DMS)**

C) AWS Snowmobile

D) Amazon FSx

**Respuesta correcta: B.** 

*DMS migra bases de datos manteniendo la fuente operativa; al ser una migración homogénea (mismo motor), no requiere AWS SCT para convertir esquema.*

Referencia: Parte 13

**Pregunta 35.** ¿Qué modelo de despliegue de nube prioriza el control total y la exclusividad de uso, a cambio de mayor costo de mantenimiento frente a la nube pública?

A) Nube pública

**B)** **Nube privada**

C) Nube híbrida

D) Nube comunitaria

**Respuesta correcta: B.** 

*La nube privada ofrece control y exclusividad dedicados a una organización, perdiendo parte de la eficiencia de costos del modelo compartido de la nube pública.*

Referencia: Parte 1

**Pregunta 36.** ¿Qué es cierto sobre la disponibilidad de servicios de AWS entre distintas Regiones?

A) Todos los servicios están disponibles en todas las Regiones simultáneamente desde su lanzamiento

**B)** **No todos los servicios están disponibles en todas las Regiones; los más nuevos suelen lanzarse primero en unas pocas Regiones**

C) Solo us-east-1 tiene servicios disponibles

D) La disponibilidad de servicios no varía nunca entre Regiones

**Respuesta correcta: B.** 

*Los servicios nuevos suelen lanzarse primero en Regiones limitadas (frecuentemente us-east-1) y expandirse gradualmente; siempre debe verificarse la Region Table.*

Referencia: Parte 2

**Pregunta 37.** ¿Qué es cierto sobre un IAM Role usado por una función Lambda?

A) La función Lambda necesita access keys embebidas además del Role

**B)** **El Role otorga a la función únicamente los permisos necesarios para su tarea, sin credenciales permanentes almacenadas**

C) Un Role nunca puede usarse con Lambda, solo con EC2

D) El Role de Lambda siempre otorga acceso administrador completo

**Respuesta correcta: B.** 

*Un Role asociado a una función Lambda le otorga credenciales temporales con exactamente los permisos necesarios, sin requerir access keys embebidas.*

Referencia: Parte 3

**Pregunta 38.** ¿Qué servicio de cómputo sería el más adecuado para un servidor de desarrollo personal con presupuesto muy limitado y sin necesidad de alta disponibilidad?

A) Amazon Redshift

**B)** **Una instancia EC2 t2.micro/t3.micro Free Tier eligible, o Amazon Lightsail**

C) AWS Direct Connect

D) Amazon Neptune

**Respuesta correcta: B.** 

*Para un servidor de desarrollo personal de bajo presupuesto, una instancia EC2 Free Tier o Lightsail son las opciones más económicas y simples.*

Referencia: Parte 4

**Pregunta 39.** ¿Qué característica de EFS permite que su capacidad se ajuste automáticamente sin necesidad de aprovisionar un tamaño fijo por adelantado?

A) EFS requiere definir un tamaño fijo obligatorio, igual que EBS

**B)** **EFS escala automáticamente su capacidad según los datos almacenados, sin aprovisionamiento previo de tamaño**

C) EFS solo funciona con tamaños menores a 10 GB

D) EFS no permite ningún tipo de escalado

**Respuesta correcta: B.** 

*A diferencia de EBS (que requiere definir un tamaño fijo), EFS escala automáticamente según el volumen de datos real almacenado.*

Referencia: Parte 5

**Pregunta 40.** ¿Qué combinación describe correctamente el uso de S3 Lifecycle Policies junto con S3 Versioning?

A) No pueden usarse juntas en el mismo bucket

**B)** **Las reglas de lifecycle pueden aplicarse tanto a las versiones actuales como a las versiones anteriores (noncurrent) de un objeto**

C) Lifecycle elimina automáticamente el versionado al activarse

D) Versioning desactiva automáticamente cualquier regla de lifecycle

**Respuesta correcta: B.** 

*Las reglas de lifecycle en un bucket con versionado pueden gestionar tanto la versión actual como las versiones anteriores (noncurrent versions) de forma independiente.*

Referencia: Parte 5

**Pregunta 41.** ¿Qué servicio de AWS sería el más adecuado para almacenar el histórico de eventos de sensores IoT de una fábrica, con consultas analíticas complejas posteriores sobre años de datos?

A) Amazon DynamoDB exclusivamente para el histórico completo

**B)** **Amazon Redshift para el análisis histórico, posiblemente con DynamoDB para el estado en tiempo real**

C) AWS Batch exclusivamente

D) Amazon Lightsail

**Respuesta correcta: B.** 

*Redshift es adecuado para análisis histórico de grandes volúmenes; DynamoDB podría complementar para el estado en tiempo real de baja latencia.*

Referencia: Parte 6

**Pregunta 42.** ¿Qué elemento de diseño de VPC sería incorrecto para una base de datos de producción crítica según las mejores prácticas de AWS?

A) Ubicarla en una subred privada

**B)** **Ubicarla en una subred pública con acceso directo desde internet**

C) Protegerla con un Security Group restrictivo

D) Activar backups automáticos

**Respuesta correcta: B.** 

*Ubicar una base de datos de producción en una subred pública con acceso directo desde internet viola las mejores prácticas de seguridad de red.*

Referencia: Parte 7

**Pregunta 43.** ¿Qué servicio de AWS sería el más adecuado para dar servicio DNS con políticas de enrutamiento por latencia hacia distintos endpoints según la ubicación del usuario?

A) Amazon CloudFront exclusivamente

**B)** **Amazon Route 53**

C) AWS Direct Connect

D) Amazon VPC

**Respuesta correcta: B.** 

*Route 53 ofrece políticas de enrutamiento avanzadas, incluyendo enrutamiento por latencia, dirigiendo a cada usuario hacia el endpoint más rápido.*

Referencia: Parte 7

**Pregunta 44.** ¿Qué describe mejor el motivo por el que AWS recomienda usar IAM Roles en vez de access keys embebidas para aplicaciones en EC2?

A) Los Roles son más rápidos de configurar únicamente

**B)** **Los Roles eliminan la necesidad de almacenar credenciales permanentes, reduciendo el riesgo de exposición si el código se filtra**

C) Las access keys embebidas son más seguras que los Roles

D) No existe ninguna diferencia de seguridad real

**Respuesta correcta: B.** 

*Los Roles evitan almacenar credenciales permanentes en el código, que podrían filtrarse (por ejemplo, en un repositorio público), reduciendo significativamente el riesgo.*

Referencia: Parte 3

**Pregunta 45.** ¿Qué servicio ayudaría a demostrar que una aplicación cumple con el requisito de que 'ningún bucket S3 debe ser públicamente accesible' de forma continua?

**A)** **AWS Config con una regla de cumplimiento correspondiente**

B) AWS CloudTrail exclusivamente

C) Amazon GuardDuty exclusivamente

D) AWS Certificate Manager

**Respuesta correcta: A.** 

*AWS Config puede evaluar continuamente si los buckets S3 cumplen la regla de no ser públicamente accesibles, alertando ante desviaciones.*

Referencia: Parte 8

**Pregunta 46.** ¿Qué es cierto sobre AWS Shield Advanced en comparación con Shield Standard?

A) Shield Advanced es gratuito para todos; Shield Standard tiene costo

**B)** **Shield Advanced tiene costo adicional y ofrece protección más avanzada, visibilidad detallada, y acceso al equipo de respuesta DDoS de AWS**

C) Ambos ofrecen exactamente las mismas funcionalidades

D) Shield Advanced solo protege bases de datos

**Respuesta correcta: B.** 

*Shield Advanced añade protección más sofisticada, visibilidad en tiempo real, y acceso al AWS DDoS Response Team, con costo adicional sobre Shield Standard.*

Referencia: Parte 8

**Pregunta 47.** ¿Qué servicio permitiría rastrear que una solicitud lenta de un usuario pasó por API Gateway, luego una Lambda, y finalmente una consulta lenta a DynamoDB?

A) Amazon CloudWatch exclusivamente

**B)** **AWS X-Ray**

C) AWS Trusted Advisor

D) Amazon Route 53

**Respuesta correcta: B.** 

*X-Ray traza el recorrido completo de una solicitud a través de múltiples servicios, identificando en qué segmento específico se genera la lentitud.*

Referencia: Parte 9

**Pregunta 48.** ¿Qué recomienda AWS respecto a la frecuencia de revisión de Trusted Advisor y Cost Explorer para una gestión de costos efectiva?

A) Revisarlos una sola vez al crear la cuenta y nunca más

**B)** **Revisarlos de forma recurrente, no solo una vez, como parte de un proceso continuo de optimización**

C) Solo revisarlos si AWS lo solicita explícitamente

D) Revisarlos exclusivamente al final del año fiscal

**Respuesta correcta: B.** 

*La optimización de costos es un proceso continuo; revisar herramientas como Trusted Advisor y Cost Explorer de forma recurrente es la práctica recomendada.*

Referencia: Parte 9 y 11

**Pregunta 49.** ¿Qué servicio de integración sería el más adecuado para conectar eventos de una aplicación SaaS de terceros (como un CRM) con una función Lambda propia, filtrando solo cierto tipo de eventos?

A) Amazon SQS exclusivamente

**B)** **Amazon EventBridge, con una regla de filtrado configurada**

C) AWS Certificate Manager

D) Amazon Route 53

**Respuesta correcta: B.** 

*EventBridge soporta integraciones nativas con aplicaciones SaaS de terceros y permite filtrar eventos según reglas antes de enrutarlos a Lambda.*

Referencia: Parte 10

**Pregunta 50.** ¿Qué es cierto sobre el patrón de mensajería usado cuando un pedido confirmado debe notificar simultáneamente a facturación, inventario y al cliente?

A) Es un patrón de colas puro (SQS exclusivamente)

**B)** **Es un patrón de publicación/suscripción tipo fan-out, típicamente resuelto con SNS o EventBridge**

C) No existe ningún patrón estándar para este caso

D) Requiere obligatoriamente Step Functions

**Respuesta correcta: B.** 

*Notificar a múltiples sistemas simultáneamente desde un único evento es el patrón fan-out, resuelto naturalmente con SNS o EventBridge.*

Referencia: Parte 10

**Pregunta 51.** ¿Qué es cierto sobre el costo de AWS Organizations en cuanto a su uso básico de facturación consolidada?

A) Tiene un costo mensual fijo por cuenta miembro

**B)** **AWS Organizations es gratuito de usar; los costos provienen de los recursos usados en cada cuenta**

C) Solo las empresas Enterprise pueden usar Organizations

D) Requiere un mínimo de 50 cuentas para activarse

**Respuesta correcta: B.** 

*AWS Organizations en sí es gratuito; el costo proviene únicamente de los recursos que las cuentas miembro consumen.*

Referencia: Parte 11

**Pregunta 52.** ¿Qué pilar del Well-Architected Framework se pondría a prueba directamente mediante un ejercicio de 'game day' que simula la caída de una Availability Zone completa?

A) Optimización de Costos

**B)** **Fiabilidad**

C) Sostenibilidad

D) Ninguno de los pilares se relaciona con este ejercicio

**Respuesta correcta: B.** 

*Simular la caída de una AZ para probar la respuesta del sistema evalúa directamente el pilar de Fiabilidad y su capacidad de recuperación real.*

Referencia: Parte 12

**Pregunta 53.** ¿Qué describe mejor la diferencia entre AWS Backup y hacer snapshots manuales de forma independiente en cada servicio?

A) Son exactamente equivalentes en todos los aspectos

**B)** **AWS Backup centraliza políticas consistentes a través de múltiples tipos de recursos desde una única consola, evitando configuración dispersa**

C) Los snapshots manuales son siempre más baratos que AWS Backup

D) AWS Backup solo puede usarse una vez por cuenta

**Respuesta correcta: B.** 

*AWS Backup evita la dispersión de configurar backups de forma independiente por servicio, centralizando políticas consistentes de frecuencia y retención.*

Referencia: Parte 13

**Pregunta 54.** ¿Qué elemento de diseño ilustra correctamente la aplicación combinada de los pilares de Seguridad y Fiabilidad en una arquitectura real?

**A)** **Cifrar los datos en reposo (Seguridad) y desplegar en múltiples AZ con backups probados (Fiabilidad) simultáneamente**

B) Solo es posible aplicar un pilar a la vez en cualquier arquitectura

C) Seguridad y Fiabilidad son mutuamente excluyentes

D) Ninguna arquitectura real combina múltiples pilares

**Respuesta correcta: A.** 

*Una arquitectura bien diseñada aplica múltiples pilares simultáneamente: cifrado de datos (Seguridad) junto con redundancia multi-AZ y backups probados (Fiabilidad).*

Referencia: Parte 12

**Pregunta 55.** ¿Qué es cierto sobre la elección entre AWS DataSync y AWS Snowball para una transferencia de 5 TB de archivos con una conexión a internet razonablemente buena?

A) Snowball sería la única opción viable en cualquier caso

**B)** **AWS DataSync sería más adecuado, ya que la conexión existente puede manejar ese volumen en un tiempo razonable sin necesitar un dispositivo físico**

C) Ambos servicios son exactamente intercambiables sin ninguna consideración de volumen

D) Ninguno de los dos puede transferir archivos, solo bases de datos

**Respuesta correcta: B.** 

*Para volúmenes moderados con una conexión razonable, DataSync es más simple y rápido de implementar que solicitar y esperar un dispositivo físico Snowball.*

Referencia: Parte 13

**Pregunta 56.** ¿Qué es cierto sobre el uso del usuario root en combinación con MFA, según las mejores prácticas de AWS?

A) MFA en el root es opcional y de baja prioridad

**B)** **MFA debe activarse en el usuario root desde el primer momento de creación de la cuenta, antes de cualquier otra configuración**

C) El usuario root no puede tener MFA activado

D) MFA solo aplica a IAM Users, nunca al root

**Respuesta correcta: B.** 

*AWS recomienda activar MFA en el usuario root como la primera acción de seguridad al crear una cuenta, dado el control total e irrestricto que ese usuario posee.*

Referencia: Parte 1 y 3

**Pregunta 57.** ¿Qué es cierto sobre la relación entre Amazon EKS/ECS y AWS Fargate en cuanto a su rol respectivo?

A) Fargate es un orquestador de contenedores que compite con ECS y EKS

**B)** **Fargate es el motor de cómputo serverless que se usa JUNTO con ECS o EKS, no un orquestador en sí mismo**

C) ECS y EKS no pueden usarse con Fargate bajo ninguna circunstancia

D) Fargate reemplaza completamente la necesidad de contenedores

**Respuesta correcta: B.** 

*Fargate no orquesta contenedores por sí mismo; es el motor de cómputo serverless que ECS o EKS usan como tipo de lanzamiento para no administrar servidores.*

Referencia: Parte 4

**Pregunta 58.** ¿Qué es cierto sobre el patrón de 'rightsizing' aplicado a una base de datos RDS sobredimensionada con bajo uso de CPU sostenido?

A) Rightsizing solo aplica a instancias EC2, nunca a RDS

**B)** **Rightsizing recomendaría reducir el tipo de instancia de RDS al tamaño que coincida con el uso real observado**

C) Rightsizing siempre recomienda aumentar el tamaño de cualquier recurso

D) Rightsizing es sinónimo exacto de Reserved Instances

**Respuesta correcta: B.** 

*El principio de rightsizing aplica a cualquier recurso, incluyendo instancias de RDS, ajustando su tamaño a la demanda real observada para optimizar costos.*

Referencia: Parte 11

**Pregunta 59.** ¿Qué es cierto sobre la combinación de AWS Migration Hub con AWS Application Discovery Service en un proyecto de migración?

A) Application Discovery Service migra los datos; Migration Hub descubre servidores

**B)** **Application Discovery Service ayuda a descubrir servidores y sus dependencias on-premises; Migration Hub consolida y rastrea el progreso de la migración de esos servidores descubiertos**

C) Ambos servicios son exactamente el mismo

D) Ninguno de los dos tiene relación con migraciones reales

**Respuesta correcta: B.** 

*Application Discovery Service identifica servidores y dependencias on-premises como paso previo; Migration Hub consolida y rastrea el progreso de migrar esos recursos descubiertos.*

Referencia: Parte 13

**Pregunta 60.** ¿Qué es cierto sobre el nivel de esfuerzo requerido para lanzar un nuevo servidor en la nube frente a on-premises, según el beneficio de 'agilidad'?

A) Es exactamente el mismo esfuerzo en ambos casos

**B)** **En la nube, un nuevo servidor puede aprovisionarse en minutos; on-premises, comprar e instalar hardware puede tomar semanas**

C) On-premises siempre es más rápido que la nube

D) La agilidad no es un beneficio real del cloud computing

**Respuesta correcta: B.** 

*La agilidad de la nube permite aprovisionar recursos en minutos, frente a semanas o meses para adquirir e instalar hardware físico on-premises.*

Referencia: Parte 1

**Pregunta 61.** ¿Qué es cierto sobre el uso de un IAM Group para 50 desarrolladores con los mismos permisos de acceso a S3 y EC2?

A) Se debe crear una policy individual para cada uno de los 50 desarrolladores

**B)** **Se puede crear un IAM Group con la policy necesaria una sola vez, y añadir los 50 usuarios a ese grupo**

C) Los Groups no pueden tener más de 10 usuarios

D) Cada desarrollador necesita su propio IAM Role, no un Group

**Respuesta correcta: B.** 

*Un IAM Group permite asignar permisos una sola vez a nivel de grupo, aplicándose automáticamente a todos sus miembros, escalando eficientemente con el número de usuarios.*

Referencia: Parte 3

**Pregunta 62.** ¿Qué es cierto sobre el uso de AWS Config junto con AWS CloudTrail en una investigación de un incidente de seguridad?

A) Solo uno de los dos servicios es útil en cualquier investigación

**B)** **CloudTrail respondería 'quién hizo qué acción', y Config respondería 'cómo estaba configurado el recurso en ese momento', siendo complementarios**

C) Ambos servicios ofrecen exactamente la misma información

D) Ninguno de los dos es relevante para investigaciones de seguridad

**Respuesta correcta: B.** 

*En una investigación completa, CloudTrail aporta el historial de acciones, y Config aporta el historial de configuración — juntos dan una imagen completa del incidente.*

Referencia: Parte 8

**Pregunta 63.** ¿Qué es cierto sobre el uso de Amazon ElastiCache delante de una base de datos Aurora con alta carga de lecturas repetidas?

A) ElastiCache reemplaza completamente la necesidad de Aurora

**B)** **ElastiCache complementa a Aurora, sirviendo lecturas frecuentes desde memoria y reduciendo la carga sobre la base de datos principal**

C) ElastiCache y Aurora no pueden usarse juntos

D) ElastiCache solo funciona con DynamoDB, no con Aurora

**Respuesta correcta: B.** 

*ElastiCache actúa como capa de caché complementaria, no como reemplazo, reduciendo la carga de lecturas repetidas sobre la base de datos principal.*

Referencia: Parte 6

**Pregunta 64.** ¿Qué es cierto sobre la relación entre el pilar de Optimización de Costos y el pilar de Sostenibilidad al aplicar rightsizing a una flota de instancias EC2?

A) No existe ninguna relación entre ambos pilares en este caso

**B)** **Rightsizing beneficia simultáneamente a ambos pilares: reduce el gasto y reduce el consumo energético de capacidad ociosa**

C) Rightsizing solo beneficia a Optimización de Costos, nunca a Sostenibilidad

D) Rightsizing perjudica al pilar de Sostenibilidad

**Respuesta correcta: B.** 

*Ajustar instancias a la demanda real reduce tanto el gasto (Optimización de Costos) como el desperdicio energético de capacidad ociosa (Sostenibilidad), ilustrando una sinergia entre pilares.*

Referencia: Parte 12

**Pregunta 65.** Al completar los cinco simulacros de esta guía con una puntuación consistente por encima del 85-90%, ¿qué recomienda hacer esta guía antes de presentarte al examen real?

A) Repasar exclusivamente las preguntas que acertaste

**B)** **Repasar el capítulo de Estrategias para Aprobar el Examen y las tablas comparativas de servicios que más se confunden**

C) Memorizar las 325 preguntas de los simulacros palabra por palabra

D) No es necesario ningún repaso adicional

**Respuesta correcta: B.** 

*El capítulo de estrategias y las tablas comparativas (GuardDuty vs Inspector, CloudTrail vs Config, SQS vs SNS, etc.) son el mejor repaso final antes del examen real.*

Referencia: Capítulo de Estrategias

## Hoja de respuestas rápida

| # | # | # | # | # |
| --- | --- | --- | --- | --- |
| 1: B | 2: B | 3: C | 4: B | 5: C |
| 6: B | 7: B | 8: B | 9: B | 10: B |
| 11: C | 12: B | 13: B | 14: B | 15: B |
| 16: B | 17: B | 18: B | 19: B | 20: B |
| 21: B | 22: B | 23: B | 24: B | 25: B |
| 26: B | 27: B | 28: B | 29: C | 30: B |
| 31: B | 32: B | 33: A | 34: B | 35: B |
| 36: B | 37: B | 38: B | 39: B | 40: B |
| 41: B | 42: B | 43: B | 44: B | 45: A |
| 46: B | 47: B | 48: B | 49: B | 50: B |
| 51: B | 52: B | 53: B | 54: A | 55: B |
| 56: B | 57: B | 58: B | 59: B | 60: B |
| 61: B | 62: B | 63: B | 64: B | 65: B |
