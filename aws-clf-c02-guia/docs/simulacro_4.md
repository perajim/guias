# AWS Certified Cloud Practitioner (CLF-C02)

**Simulacro de Examen 4 de 5 — 65 preguntas**

Mismo nivel de dificultad y distribución de dominios que el examen oficial CLF-C02: Cloud Concepts, Security and Compliance, Cloud Technology and Services, y Billing and Pricing. Cada pregunta incluye la respuesta correcta, una explicación, y una referencia al capítulo de la guía donde puedes repasar el tema si fallaste.

> **Cómo usar este simulacro:** Resuélvelo primero completo, sin mirar las respuestas, cronometrando 90 minutos como en el examen real. Después revisa cada pregunta, prestando especial atención a las que fallaste, y repasa el capítulo referenciado antes de tu siguiente simulacro.

## Preguntas

**Pregunta 1.** ¿Qué característica esencial del cloud computing permite a un cliente aprovisionar recursos sin interacción humana con el proveedor?

A) Servicio medido

**B)** **Autoservicio bajo demanda**

C) Acceso amplio a la red

D) Pool de recursos compartidos

**Respuesta correcta: B.** 

*El autoservicio bajo demanda permite a los clientes aprovisionar capacidad de cómputo automáticamente, sin requerir interacción humana con AWS.*

Referencia: Parte 1

**Pregunta 2.** ¿Qué modelo de despliegue de nube está compartido entre varias organizaciones con requisitos comunes, como agencias gubernamentales afines?

A) Nube pública

B) Nube privada

**C)** **Nube comunitaria**

D) Nube híbrida

**Respuesta correcta: C.** 

*La nube comunitaria es compartida entre organizaciones con necesidades similares, como requisitos regulatorios comunes.*

Referencia: Parte 1

**Pregunta 3.** ¿Qué analogía describe mejor la diferencia entre IaaS y SaaS?

A) IaaS es como pedir pizza a domicilio; SaaS es cocinar desde cero

**B)** **IaaS es como comprar ingredientes crudos; SaaS es pedir la pizza ya lista**

C) Ambos son exactamente iguales

D) SaaS requiere más administración que IaaS

**Respuesta correcta: B.** 

*IaaS entrega los 'ingredientes' básicos que el cliente administra; SaaS entrega el producto terminado listo para consumir.*

Referencia: Parte 1

**Pregunta 4.** ¿Cuál de los siguientes es un criterio real que AWS menciona para elegir en qué Región desplegar una carga de trabajo?

A) El color corporativo de la Región

**B)** **Disponibilidad de servicios específicos en esa Región**

C) El número de empleados de soporte técnico local

D) La cantidad de universidades cercanas

**Respuesta correcta: B.** 

*AWS menciona cumplimiento, latencia, disponibilidad de servicios y costo como los cuatro criterios reales para elegir Región.*

Referencia: Parte 2

**Pregunta 5.** ¿Qué SDK de AWS se usa comúnmente para interactuar con servicios de AWS desde código Python?

**A)** **Boto3**

B) AWS CLI

C) CloudFormation

D) AWS Config

**Respuesta correcta: A.** 

*Boto3 es el SDK oficial de AWS para Python, permitiendo llamar a los servicios de AWS directamente desde el código.*

Referencia: Parte 2

**Pregunta 6.** ¿Qué regla de evaluación de IAM Policies tiene mayor prioridad, sin importar cuántas otras policies otorguen el permiso?

A) Un Allow explícito

**B)** **Un Deny explícito**

C) El orden de creación de las policies

D) La antigüedad del usuario

**Respuesta correcta: B.** 

*Un Deny explícito siempre prevalece sobre cualquier Allow, sin importar cuántas otras policies otorguen el permiso.*

Referencia: Parte 3

**Pregunta 7.** ¿Qué mejor práctica de IAM ayuda a reducir el impacto si las credenciales de una aplicación se filtran accidentalmente?

A) Otorgar acceso administrador completo a la aplicación

**B)** **Aplicar el principio de mínimo privilegio, otorgando solo los permisos estrictamente necesarios**

C) Usar siempre el usuario root para aplicaciones

D) Deshabilitar CloudTrail para simplificar auditoría

**Respuesta correcta: B.** 

*El mínimo privilegio limita el daño posible ante una filtración de credenciales, restringiendo los permisos a lo estrictamente necesario.*

Referencia: Parte 3

**Pregunta 8.** ¿Qué componente de EC2 define qué software y sistema operativo tendrá una instancia al lanzarse?

A) El Security Group

**B)** **La AMI (Amazon Machine Image)**

C) La Route Table

D) El IAM Role

**Respuesta correcta: B.** 

*La AMI es la plantilla que define el sistema operativo y software preinstalado de una instancia EC2 al lanzarse.*

Referencia: Parte 4

**Pregunta 9.** ¿Qué servicio orquesta contenedores usando el estándar open source Kubernetes de forma administrada?

A) Amazon ECS

**B)** **Amazon EKS**

C) AWS Fargate exclusivamente

D) AWS Batch

**Respuesta correcta: B.** 

*Amazon EKS es la versión administrada de Kubernetes de AWS, compatible con el ecosistema estándar de herramientas Kubernetes.*

Referencia: Parte 4

**Pregunta 10.** ¿Qué mecanismo de un Elastic Load Balancer deja de enviar tráfico a una instancia que no responde correctamente?

**A)** **Health checks (verificaciones de salud)**

B) Security Groups

C) AMI versioning

D) IAM Roles

**Respuesta correcta: A.** 

*Los health checks periódicos del ELB detectan instancias no saludables y dejan de enrutarles tráfico automáticamente.*

Referencia: Parte 4

**Pregunta 11.** ¿Qué clase de almacenamiento de S3 ofrece acceso instantáneo con menor costo que Standard, apta para datos infrecuentes que deben recuperarse de inmediato?

A) S3 Glacier Deep Archive

**B)** **S3 Standard-IA**

C) S3 Glacier Flexible Retrieval

D) S3 One Zone-IA exclusivamente para datos críticos

**Respuesta correcta: B.** 

*S3 Standard-IA reduce el costo de almacenamiento manteniendo acceso instantáneo, ideal para datos de acceso infrecuente pero urgente cuando se necesitan.*

Referencia: Parte 5

**Pregunta 12.** ¿Qué permite S3 Object Lock que S3 Versioning por sí solo no garantiza?

A) Reducir el costo de almacenamiento automáticamente

**B)** **Bloquear objetos para que no puedan eliminarse ni sobrescribirse durante un periodo definido (WORM)**

C) Aumentar la velocidad de descarga

D) Replicar automáticamente entre Regiones

**Respuesta correcta: B.** 

*Object Lock impone la restricción WORM (Write Once Read Many), algo que el versionado por sí solo no garantiza (ya que las versiones podrían eliminarse manualmente).*

Referencia: Parte 5

**Pregunta 13.** ¿Qué tipo de EBS Snapshot se recomienda antes de eliminar una instancia EC2 cuyo volumen se quiere conservar?

A) Ninguno, los volúmenes se conservan automáticamente para siempre

**B)** **Un snapshot manual del volumen antes de terminar la instancia**

C) Un backup de RDS

D) Una imagen de contenedor en ECR

**Respuesta correcta: B.** 

*Crear un snapshot manual del volumen EBS antes de terminar la instancia permite conservar los datos y recrear el volumen después si es necesario.*

Referencia: Parte 5

**Pregunta 14.** ¿Qué servicio de base de datos administrado ofrece compatibilidad con MongoDB para minimizar cambios de código durante una migración?

A) Amazon Aurora

**B)** **Amazon DocumentDB**

C) Amazon Neptune

D) Amazon Redshift

**Respuesta correcta: B.** 

*DocumentDB fue diseñado con compatibilidad de API con MongoDB, facilitando migraciones con cambios mínimos de código.*

Referencia: Parte 6

**Pregunta 15.** ¿Qué caso de uso es más adecuado para Amazon Neptune frente a una base de datos relacional tradicional?

A) Transacciones financieras simples de un solo registro

**B)** **Análisis de relaciones altamente conectadas, como redes sociales o detección de fraude**

C) Almacenamiento de archivos grandes de video

D) Caché de sesiones de usuario

**Respuesta correcta: B.** 

*Neptune está optimizado para navegar relaciones altamente conectadas, un patrón ineficiente de modelar con JOINs relacionales tradicionales a gran profundidad.*

Referencia: Parte 6

**Pregunta 16.** ¿Qué es cierto sobre las Read Replicas de RDS en cuanto a failover automático?

A) Ofrecen failover automático igual que Multi-AZ

**B)** **No ofrecen failover automático; están diseñadas para escalar lecturas, aunque pueden promoverse manualmente**

C) Solo existen en DynamoDB, no en RDS

D) Requieren detener la base de datos primaria

**Respuesta correcta: B.** 

*Las Read Replicas escalan el tráfico de lectura y no ofrecen failover automático como Multi-AZ, aunque pueden promoverse manualmente si es necesario.*

Referencia: Parte 6

**Pregunta 17.** ¿Qué elemento de una VPC asocia una subred con las reglas que determinan hacia dónde se dirige su tráfico?

A) El Security Group

**B)** **La Route Table**

C) El IAM Role

D) La AMI

**Respuesta correcta: B.** 

*La tabla de rutas asociada a una subred determina el destino del tráfico según la IP, definiendo si esa subred es pública o privada.*

Referencia: Parte 7

**Pregunta 18.** ¿Qué servicio sería el más adecuado para servir contenido estático de un sitio web con baja latencia a usuarios distribuidos globalmente?

A) AWS Direct Connect

**B)** **Amazon CloudFront**

C) AWS Site-to-Site VPN

D) Amazon EBS

**Respuesta correcta: B.** 

*CloudFront distribuye contenido cacheado desde Edge Locations cercanas a cada usuario, reduciendo la latencia de entrega.*

Referencia: Parte 7

**Pregunta 19.** ¿Qué es cierto sobre el tráfico dentro de una VPC entre dos subredes de la misma Región, por defecto?

A) Está bloqueado completamente por defecto en todos los casos

**B)** **La 'main route table' por defecto permite tráfico dentro de la propia VPC**

C) Requiere obligatoriamente un NAT Gateway

D) Requiere pasar por internet público

**Respuesta correcta: B.** 

*La tabla de rutas principal por defecto de una VPC permite el tráfico entre recursos dentro de la misma VPC sin pasar por internet.*

Referencia: Parte 7

**Pregunta 20.** ¿Qué responsabilidad NUNCA recae en AWS, sin importar cuán administrado sea el servicio?

A) Parches del hipervisor

**B)** **La clasificación y el contenido de los datos del cliente**

C) La infraestructura eléctrica de los data centers

D) La red troncal global de AWS

**Respuesta correcta: B.** 

*La clasificación, contenido y configuración de los propios datos del cliente es siempre responsabilidad del cliente, sin excepción.*

Referencia: Parte 8

**Pregunta 21.** ¿Qué servicio ofrecería protección contra patrones de ataque como cross-site scripting (XSS) en el tráfico HTTP de una aplicación web?

A) AWS Shield exclusivamente

**B)** **AWS WAF**

C) Amazon GuardDuty

D) AWS Config

**Respuesta correcta: B.** 

*AWS WAF opera en capa de aplicación, filtrando patrones de ataque HTTP conocidos como XSS e inyección SQL.*

Referencia: Parte 8

**Pregunta 22.** ¿Qué servicio usarías para confirmar exactamente qué usuario de IAM eliminó un bucket S3 específico y a qué hora?

A) AWS Config

**B)** **AWS CloudTrail**

C) Amazon GuardDuty

D) AWS Trusted Advisor

**Respuesta correcta: B.** 

*CloudTrail registra el historial detallado de llamadas a la API, incluyendo quién realizó una acción específica y cuándo.*

Referencia: Parte 8

**Pregunta 23.** ¿Qué combinación de servicios de seguridad cubriría tanto la detección de comportamiento anómalo como el escaneo de vulnerabilidades conocidas en instancias EC2?

**A)** **GuardDuty (comportamiento) e Inspector (vulnerabilidades)**

B) Solo Macie

C) Solo AWS Shield

D) Solo AWS Config

**Respuesta correcta: A.** 

*GuardDuty detecta actividad anómala/maliciosa; Inspector escanea vulnerabilidades conocidas (CVEs) en EC2, contenedores y Lambda — se complementan.*

Referencia: Parte 8

**Pregunta 24.** ¿Qué servicio permite visualizar en qué segmento específico de una arquitectura distribuida se origina la latencia de una solicitud?

A) Amazon CloudWatch exclusivamente

**B)** **AWS X-Ray**

C) AWS Health Dashboard

D) AWS Trusted Advisor

**Respuesta correcta: B.** 

*X-Ray traza el recorrido de solicitudes individuales, mostrando el tiempo consumido en cada segmento de la arquitectura distribuida.*

Referencia: Parte 9

**Pregunta 25.** ¿Qué categoría de AWS Trusted Advisor identificaría que el MFA del usuario root no está activado?

A) Optimización de costos

**B)** **Seguridad**

C) Rendimiento

D) Límites de servicio

**Respuesta correcta: B.** 

*La categoría de Seguridad de Trusted Advisor incluye verificaciones como la activación de MFA en el usuario root.*

Referencia: Parte 9

**Pregunta 26.** ¿Qué acción sobre una instancia EC2 puede disparar directamente una CloudWatch Alarm, además de notificaciones SNS y Auto Scaling?

**A)** **Detener, terminar, reiniciar o recuperar la instancia**

B) Cambiar automáticamente su tipo de instancia a uno más grande

C) Migrarla automáticamente a otra Región

D) Aprobar automáticamente cambios de IAM

**Respuesta correcta: A.** 

*Las CloudWatch Alarms pueden disparar acciones directas sobre instancias EC2 como detener, terminar, reiniciar o recuperar, además de SNS y Auto Scaling.*

Referencia: Parte 9

**Pregunta 27.** ¿Qué servicio de integración sería el más adecuado para desacoplar un servicio productor de un servicio consumidor que procesa mensajes a su propio ritmo?

A) Amazon SNS

**B)** **Amazon SQS**

C) Amazon Route 53

D) AWS Certificate Manager

**Respuesta correcta: B.** 

*SQS actúa como buffer entre productor y consumidor, permitiendo que el consumidor procese a su propio ritmo sin afectar al productor.*

Referencia: Parte 10

**Pregunta 28.** ¿Qué servicio permite orquestar visualmente un proceso de negocio de múltiples pasos con ramificación condicional y manejo de reintentos?

A) Amazon SQS

**B)** **AWS Step Functions**

C) Amazon SNS

D) Amazon API Gateway

**Respuesta correcta: B.** 

*Step Functions representa flujos de trabajo como una máquina de estados visual, con manejo nativo de reintentos y ramificación condicional.*

Referencia: Parte 10

**Pregunta 29.** ¿Qué transferencia de datos en AWS típicamente SÍ tiene costo asociado?

A) Transferencia entrante hacia S3 desde internet

**B)** **Transferencia saliente hacia internet desde EC2**

C) Transferencia entre dos instancias en la misma AZ usando IP privada

D) Ninguna transferencia tiene costo en AWS

**Respuesta correcta: B.** 

*La transferencia saliente hacia internet tiene costo (con una capa gratuita limitada); la entrante es generalmente gratuita.*

Referencia: Parte 11

**Pregunta 30.** ¿Qué modelo de precios de cómputo sería el más adecuado para una carga de trabajo de renderizado nocturno que puede reintentarse si se interrumpe?

A) On-Demand exclusivamente

B) Reserved Instances a 3 años

**C)** **Spot Instances**

D) Dedicated Hosts

**Respuesta correcta: C.** 

*Las cargas tolerantes a interrupciones con capacidad de reintento son el caso de uso ideal para instancias Spot, maximizando el ahorro.*

Referencia: Parte 11

**Pregunta 31.** ¿Qué pilar del Well-Architected Framework evalúa si una arquitectura puede recuperarse de errores de configuración transitorios o de red?

A) Seguridad

**B)** **Fiabilidad**

C) Optimización de costos

D) Sostenibilidad

**Respuesta correcta: B.** 

*El pilar de Fiabilidad abarca la mitigación de problemas como errores de configuración transitorios o de red, además de recuperación ante fallos.*

Referencia: Parte 12

**Pregunta 32.** ¿Qué servicio de AWS aprovisiona infraestructura a partir de plantillas declarativas versionables en un repositorio de código?

**A)** **AWS CloudFormation**

B) AWS Config

C) AWS Trusted Advisor

D) Amazon CloudWatch

**Respuesta correcta: A.** 

*CloudFormation implementa Infrastructure as Code mediante plantillas declarativas versionables como cualquier otro código fuente.*

Referencia: Parte 13

**Pregunta 33.** ¿Qué servicio de AWS sincroniza archivos entre un sistema NFS on-premises y Amazon S3 de forma recurrente y automatizada?

**A)** **AWS DataSync**

B) AWS DMS

C) AWS Snowmobile

D) AWS Migration Hub

**Respuesta correcta: A.** 

*AWS DataSync automatiza la transferencia y sincronización recurrente de archivos entre almacenamiento on-premises y servicios de AWS.*

Referencia: Parte 13

**Pregunta 34.** ¿Qué diferencia principal existe entre un data center on-premises tradicional y una Región de AWS, en cuanto a redundancia interna?

A) No existe ninguna diferencia real

**B)** **Una Región de AWS está compuesta por múltiples Availability Zones redundantes por diseño; un data center tradicional único no lo está**

C) Un data center on-premises siempre tiene más AZ que AWS

D) AWS no ofrece ninguna redundancia interna en sus Regiones

**Respuesta correcta: B.** 

*Cada Región de AWS se diseña con múltiples AZ redundantes desde el inicio, algo que un único data center on-premises tradicional no ofrece por sí mismo.*

Referencia: Parte 1 y 2

**Pregunta 35.** ¿Qué es cierto sobre el costo de crear un IAM Role en una cuenta de AWS?

A) Tiene un costo mensual fijo

**B)** **Es gratuito, como todos los elementos de IAM**

C) Solo es gratuito si se usa con EC2

D) Cuesta lo mismo que una instancia t2.micro

**Respuesta correcta: B.** 

*IAM (Users, Groups, Roles, Policies) es completamente gratuito en cualquier cantidad, sin importar el servicio con el que se use.*

Referencia: Parte 3

**Pregunta 36.** ¿Qué tipo de instancia EC2 prioriza un balance entre CPU, memoria y red, ideal para aplicaciones web típicas?

A) Compute optimized (c)

**B)** **General purpose (t, m)**

C) Storage optimized (i, d)

D) Memory optimized (r, x)

**Respuesta correcta: B.** 

*La familia 'general purpose' (t, m) ofrece un balance adecuado para la mayoría de las aplicaciones web típicas sin requisitos extremos específicos.*

Referencia: Parte 4

**Pregunta 37.** ¿Qué servicio de AWS sería el más adecuado para ejecutar miles de trabajos de simulación financiera con gestión automática de la cola y del cómputo necesario?

**A)** **AWS Batch**

B) Amazon Lightsail

C) Amazon Route 53

D) AWS Certificate Manager

**Respuesta correcta: A.** 

*AWS Batch planifica y ejecuta trabajos por lotes a gran escala, gestionando automáticamente la cola de trabajos y el aprovisionamiento de cómputo.*

Referencia: Parte 4

**Pregunta 38.** ¿Qué sucede si intentas eliminar un bucket S3 que aún contiene objetos, sin haberlo vaciado primero?

A) Se elimina sin problema junto con todos sus objetos

**B)** **S3 rechaza la operación hasta que el bucket esté vacío**

C) Solo se eliminan los objetos más antiguos automáticamente

D) El bucket se vuelve público automáticamente

**Respuesta correcta: B.** 

*S3 no permite eliminar un bucket que aún contiene objetos (o versiones, si el versionado está activo); debe vaciarse primero.*

Referencia: Parte 5

**Pregunta 39.** ¿Qué servicio de AWS ofrecería almacenamiento compartido de alto rendimiento compatible con SMB y Active Directory para un entorno Windows?

A) Amazon EFS

**B)** **Amazon FSx for Windows File Server**

C) Amazon S3

D) AWS Storage Gateway Tape Gateway

**Respuesta correcta: B.** 

*FSx for Windows File Server ofrece compatibilidad nativa SMB e integración con Active Directory, ideal para entornos Windows tradicionales.*

Referencia: Parte 5

**Pregunta 40.** ¿Qué servicio de AWS sería el más adecuado para almacenar el catálogo de productos de un e-commerce con relaciones complejas entre categorías, variantes y proveedores?

A) Amazon DynamoDB exclusivamente

**B)** **Amazon RDS o Aurora**

C) Amazon Redshift

D) Amazon ElastiCache

**Respuesta correcta: B.** 

*Cuando existen relaciones complejas entre múltiples entidades que requieren consultas relacionales flexibles, un modelo relacional (RDS/Aurora) suele ser más natural.*

Referencia: Parte 6

**Pregunta 41.** ¿Qué diferencia a Amazon Redshift de Amazon RDS en cuanto al tipo de carga de trabajo para el que están optimizados?

A) Son idénticos en propósito

**B)** **Redshift = analítica (OLAP) sobre grandes volúmenes históricos; RDS = transacciones (OLTP) frecuentes y pequeñas**

C) RDS es exclusivamente para analítica

D) Redshift no puede almacenar datos históricos

**Respuesta correcta: B.** 

*Redshift está optimizado para consultas analíticas complejas sobre grandes volúmenes; RDS/Aurora están optimizados para transacciones OLTP frecuentes.*

Referencia: Parte 6

**Pregunta 42.** ¿Qué elemento de un Security Group determina que solo se permitan conexiones SSH desde una IP administrativa específica, no desde cualquier IP?

**A)** **Una regla de tipo 'Allow' restringida a esa IP en el puerto 22**

B) Una regla de tipo 'Deny' genérica

C) Una Network ACL exclusivamente

D) El IAM Role de la instancia

**Respuesta correcta: A.** 

*Un Security Group permite definir reglas de Allow restringidas a rangos de IP específicos, como limitar SSH a la IP del equipo de administración.*

Referencia: Parte 4

**Pregunta 43.** ¿Qué elemento haría que una arquitectura de tres capas sea considerada más segura, respecto a la ubicación de la base de datos?

A) Colocar la base de datos en la misma subred pública que el Load Balancer

**B)** **Colocar la base de datos en una subred privada, sin ruta directa a un Internet Gateway**

C) Deshabilitar todos los Security Groups de la base de datos

D) Hacer la base de datos accesible públicamente para simplificar el acceso

**Respuesta correcta: B.** 

*Colocar la base de datos en una subred privada reduce la superficie de ataque, ya que no es directamente alcanzable desde internet.*

Referencia: Parte 7

**Pregunta 44.** ¿Qué servicio de AWS sería el más adecuado para dar acceso temporal a un contratista externo a recursos específicos y limitados de tu cuenta durante 2 meses?

A) Crear un IAM User permanente con contraseña compartida

**B)** **Crear un IAM Role de acceso entre cuentas (cross-account) con permisos limitados y duración limitada**

C) Compartir las credenciales del usuario root

D) Deshabilitar MFA para facilitarle el acceso

**Respuesta correcta: B.** 

*Un Role de acceso cruzado entre cuentas, con permisos limitados, es la práctica recomendada para colaboración temporal externa sin credenciales permanentes.*

Referencia: Parte 3

**Pregunta 45.** ¿Qué combinación de AWS Shield y AWS WAF describe correctamente su alcance de protección?

A) Ambos protegen exactamente lo mismo

**B)** **Shield protege contra DDoS a nivel de red/transporte; WAF filtra patrones maliciosos específicos en tráfico HTTP de capa de aplicación**

C) WAF protege contra DDoS; Shield filtra inyección SQL

D) Ninguno de los dos ofrece protección real

**Respuesta correcta: B.** 

*Shield y WAF protegen capas distintas: Shield ataques volumétricos DDoS, WAF patrones específicos de ataque en el tráfico de aplicación.*

Referencia: Parte 8

**Pregunta 46.** ¿Qué es cierto sobre AWS Shield Standard?

A) Requiere activación manual y tiene costo adicional

**B)** **Está activo automáticamente y sin costo adicional para todos los clientes de AWS**

C) Solo protege bases de datos RDS

D) Reemplaza completamente la necesidad de Security Groups

**Respuesta correcta: B.** 

*Shield Standard viene activado automáticamente sin costo adicional para todos los clientes, ofreciendo protección básica contra DDoS.*

Referencia: Parte 8

**Pregunta 47.** ¿Qué describe mejor el propósito de Amazon Macie dentro de una estrategia de seguridad de datos?

A) Escanear vulnerabilidades de software en instancias EC2

**B)** **Descubrir y clasificar automáticamente datos sensibles almacenados en S3**

C) Filtrar tráfico DDoS

D) Rotar contraseñas de bases de datos automáticamente

**Respuesta correcta: B.** 

*Macie usa machine learning para identificar y clasificar datos sensibles (como PII) en buckets S3, alertando sobre configuraciones de riesgo.*

Referencia: Parte 8

**Pregunta 48.** ¿Qué diferencia a AWS Config de Amazon CloudWatch en cuanto a su enfoque principal?

A) Son el mismo servicio

**B)** **Config evalúa el estado de configuración de recursos y cumplimiento de reglas; CloudWatch monitorea métricas y logs operativos en tiempo real**

C) CloudWatch solo funciona con S3

D) Config no puede evaluar cumplimiento de ninguna regla

**Respuesta correcta: B.** 

*Config se enfoca en configuración y cumplimiento a lo largo del tiempo; CloudWatch se enfoca en métricas y logs operativos en tiempo casi real.*

Referencia: Parte 8 y 9

**Pregunta 49.** ¿Qué combinación de servicios formaría una arquitectura serverless completa para procesar pedidos de un e-commerce mediante eventos?

A) EC2 + RDS exclusivamente, sin ningún servicio serverless

**B)** **API Gateway + Lambda + DynamoDB + SQS/SNS según el flujo de eventos**

C) Solo Amazon Redshift

D) Solo AWS Direct Connect

**Respuesta correcta: B.** 

*Una arquitectura serverless típica combina API Gateway (entrada), Lambda (lógica), DynamoDB (datos) y SQS/SNS (desacoplamiento) según el flujo de eventos.*

Referencia: Parte 4, 6 y 10

**Pregunta 50.** ¿Qué recomienda AWS Budgets a diferencia de AWS Cost Explorer, en cuanto al tipo de información que ofrece?

A) Ambos ofrecen exactamente la misma información

**B)** **Budgets ofrece alertas proactivas sobre gasto futuro/proyectado; Cost Explorer analiza el gasto histórico ya ocurrido**

C) Cost Explorer solo funciona con instancias Spot

D) Budgets no puede configurarse con umbrales personalizados

**Respuesta correcta: B.** 

*Budgets es proactivo (alerta antes de superar un umbral); Cost Explorer es retrospectivo (analiza qué pasó con el gasto histórico).*

Referencia: Parte 11

**Pregunta 51.** ¿Qué elemento describe mejor un Compute Savings Plan frente a un EC2 Instance Savings Plan?

A) Son exactamente iguales en flexibilidad

**B)** **Compute Savings Plan es más flexible, aplicándose a EC2 de cualquier familia/Región, Fargate y Lambda; EC2 Instance Savings Plan es más específico a una familia dentro de una Región**

C) EC2 Instance Savings Plan es más flexible que Compute Savings Plan

D) Ninguno de los dos ofrece descuento real

**Respuesta correcta: B.** 

*Compute Savings Plans ofrecen la mayor flexibilidad, aplicándose a múltiples servicios de cómputo; EC2 Instance Savings Plans son más específicos con mayor descuento a cambio de menos flexibilidad.*

Referencia: Parte 11

**Pregunta 52.** ¿Qué pilar del Well-Architected Framework evaluaría si una empresa está midiendo la eficiencia de su gasto en relación con el valor de negocio generado?

A) Seguridad

**B)** **Optimización de Costos**

C) Fiabilidad

D) Excelencia Operacional

**Respuesta correcta: B.** 

*El pilar de Optimización de Costos incluye medir la eficiencia general relacionando el gasto con el valor de negocio generado, no solo el número absoluto.*

Referencia: Parte 12

**Pregunta 53.** ¿Qué recomienda el Well-Architected Framework respecto a maximizar los seis pilares simultáneamente en una carga de trabajo?

A) Siempre deben maximizarse los seis al 100% sin excepción

**B)** **Reconoce trade-offs conscientes entre pilares según el contexto y prioridades reales del negocio**

C) Solo el pilar de Seguridad debe priorizarse siempre

D) Los pilares no tienen ninguna relación entre sí

**Respuesta correcta: B.** 

*El framework reconoce que los pilares generan trade-offs (más fiabilidad puede costar más), y las decisiones deben balancearse conscientemente según el negocio.*

Referencia: Parte 12

**Pregunta 54.** ¿Qué servicio de AWS ofrecería visibilidad centralizada del progreso de una migración de aplicaciones que usa DMS, DataSync y Snowball simultáneamente?

**A)** **AWS Migration Hub**

B) AWS CloudFormation

C) Amazon CloudWatch

D) AWS Config

**Respuesta correcta: A.** 

*Migration Hub consolida el estado de avance de distintas herramientas de migración en un único panel centralizado.*

Referencia: Parte 13

**Pregunta 55.** ¿Qué diferencia a AWS Backup de una estrategia de snapshots manuales configurados individualmente en cada servicio?

A) No hay diferencia real

**B)** **AWS Backup centraliza políticas de backup (frecuencia, retención) aplicándolas consistentemente a múltiples tipos de recursos desde un único lugar**

C) AWS Backup solo funciona con instancias EC2

D) Los snapshots manuales son siempre más seguros que AWS Backup

**Respuesta correcta: B.** 

*AWS Backup evita configurar backups de forma separada e inconsistente en cada servicio, centralizando políticas aplicadas a múltiples tipos de recursos.*

Referencia: Parte 13

**Pregunta 56.** ¿Qué describe mejor el uso de AWS Elastic Disaster Recovery frente a AWS Backup, en un escenario donde un data center completo queda inoperativo por un desastre natural?

A) AWS Backup restauraría el data center completo en minutos automáticamente

**B)** **AWS Elastic Disaster Recovery permite conmutar hacia instancias funcionales en AWS en minutos, gracias a la replicación continua previa**

C) Ninguno de los dos servicios ayuda en este escenario

D) AWS Backup y DRS son exactamente el mismo servicio

**Respuesta correcta: B.** 

*DRS está diseñado exactamente para este escenario: replicación continua previa que permite un failover rápido hacia AWS ante un desastre del entorno completo.*

Referencia: Parte 13

**Pregunta 57.** ¿Qué característica de AWS CDK lo distingue de escribir plantillas de CloudFormation directamente en YAML?

A) CDK elimina la necesidad de CloudFormation por completo

**B)** **CDK permite usar bucles, condicionales y abstracciones reutilizables de un lenguaje de programación, sintetizando hacia CloudFormation**

C) CDK solo puede usarse para bases de datos

D) CDK es más lento en cualquier escenario que escribir YAML manualmente

**Respuesta correcta: B.** 

*CDK aprovecha las capacidades de un lenguaje de programación completo, generando internamente plantillas estándar de CloudFormation para el despliegue real.*

Referencia: Parte 13

**Pregunta 58.** ¿Qué es cierto sobre el AWS Well-Architected Tool en cuanto a su costo?

A) Tiene un costo mensual según el número de cargas de trabajo evaluadas

**B)** **Es completamente gratuito de usar**

C) Solo está disponible con planes de soporte Enterprise

D) Cuesta lo mismo que un simulacro de examen oficial

**Respuesta correcta: B.** 

*El AWS Well-Architected Tool es un servicio gratuito, disponible para cualquier cuenta de AWS sin costo adicional.*

Referencia: Parte 12

**Pregunta 59.** ¿Qué elemento describe mejor la relación entre escalabilidad horizontal y la nube pública?

A) La escalabilidad horizontal solo es posible on-premises

**B)** **La nube pública facilita la escalabilidad horizontal al permitir añadir más instancias bajo demanda sin comprar hardware físico adicional**

C) La escalabilidad horizontal requiere siempre downtime en la nube

D) No existe relación entre ambos conceptos

**Respuesta correcta: B.** 

*La elasticidad de la nube pública facilita añadir instancias adicionales (escalado horizontal) rápidamente, sin necesidad de comprar hardware físico.*

Referencia: Parte 1

**Pregunta 60.** ¿Qué servicio de AWS registra eventos de ciclo de vida de recursos (como la creación de una instancia EC2) y puede enrutarlos según reglas de contenido hacia distintos destinos?

A) Amazon SQS

**B)** **Amazon EventBridge**

C) AWS Certificate Manager

D) Amazon Route 53

**Respuesta correcta: B.** 

*EventBridge captura eventos de servicios de AWS (incluyendo cambios de estado de recursos) y los enruta según reglas basadas en su contenido.*

Referencia: Parte 10

**Pregunta 61.** ¿Qué es cierto sobre los IAM Access Keys de un usuario que ya no está activo en la empresa?

A) Deben mantenerse activas indefinidamente por si se necesitan después

**B)** **Deben desactivarse o eliminarse de inmediato como parte de la gestión del ciclo de vida de accesos**

C) No es necesario ninguna acción, IAM las desactiva automáticamente

D) Solo AWS puede eliminarlas, no el administrador de la cuenta

**Respuesta correcta: B.** 

*Las credenciales de usuarios que ya no requieren acceso deben desactivarse o eliminarse de inmediato, como parte de una buena gestión de identidades.*

Referencia: Parte 3

**Pregunta 62.** ¿Qué describe mejor el propósito de un Application Load Balancer frente a un Network Load Balancer?

A) Ambos son idénticos en funcionalidad

**B)** **ALB opera en capa 7 con enrutamiento HTTP/HTTPS avanzado; NLB opera en capa 4 para TCP/UDP de altísimo rendimiento**

C) NLB solo funciona con bases de datos

D) ALB no puede usarse con instancias EC2

**Respuesta correcta: B.** 

*El ALB enruta tráfico HTTP/HTTPS con reglas avanzadas basadas en contenido; el NLB está optimizado para tráfico TCP/UDP de muy alto rendimiento y baja latencia.*

Referencia: Parte 4

**Pregunta 63.** ¿Qué es cierto sobre el costo de S3 Standard comparado con S3 Glacier Deep Archive para el mismo volumen de datos?

A) S3 Standard siempre es más barato

**B)** **S3 Glacier Deep Archive tiene un costo de almacenamiento por GB significativamente menor, a cambio de mayores tiempos de recuperación**

C) Ambas clases tienen exactamente el mismo costo

D) El costo depende únicamente del tamaño del bucket, no de la clase elegida

**Respuesta correcta: B.** 

*Glacier Deep Archive ofrece el costo por GB más bajo de todas las clases de S3, a cambio de tiempos de recuperación de varias horas.*

Referencia: Parte 5

**Pregunta 64.** ¿Qué es cierto sobre AWS Organizations en relación con Reserved Instances y Savings Plans?

A) Cada cuenta miembro debe comprar sus propios compromisos sin ningún beneficio compartido

**B)** **El beneficio de RI y Savings Plans puede compartirse entre las cuentas miembro de una organización con facturación consolidada**

C) AWS Organizations no tiene relación alguna con modelos de precios de cómputo

D) Solo la cuenta de gestión puede beneficiarse de RI o Savings Plans

**Respuesta correcta: B.** 

*La facturación consolidada de Organizations permite compartir el beneficio de Reserved Instances y Savings Plans entre las cuentas miembro.*

Referencia: Parte 11

**Pregunta 65.** ¿Qué servicio de AWS sería el más adecuado para desplegar la misma arquitectura de red y seguridad de forma idéntica en 8 cuentas distintas de una organización?

A) Repetir manualmente los mismos clics en cada cuenta

**B)** **AWS CloudFormation (o CDK), desplegando la misma plantilla en cada cuenta**

C) AWS Trusted Advisor

D) Amazon Route 53

**Respuesta correcta: B.** 

*Infrastructure as Code permite reproducir exactamente la misma arquitectura en múltiples cuentas de forma consistente, evitando errores de configuración manual repetitiva.*

Referencia: Parte 13

## Hoja de respuestas rápida

| # | # | # | # | # |
| --- | --- | --- | --- | --- |
| 1: B | 2: C | 3: B | 4: B | 5: A |
| 6: B | 7: B | 8: B | 9: B | 10: A |
| 11: B | 12: B | 13: B | 14: B | 15: B |
| 16: B | 17: B | 18: B | 19: B | 20: B |
| 21: B | 22: B | 23: A | 24: B | 25: B |
| 26: A | 27: B | 28: B | 29: B | 30: C |
| 31: B | 32: A | 33: A | 34: B | 35: B |
| 36: B | 37: A | 38: B | 39: B | 40: B |
| 41: B | 42: A | 43: B | 44: B | 45: B |
| 46: B | 47: B | 48: B | 49: B | 50: B |
| 51: B | 52: B | 53: B | 54: A | 55: B |
| 56: B | 57: B | 58: B | 59: B | 60: B |
| 61: B | 62: B | 63: B | 64: B | 65: B |
