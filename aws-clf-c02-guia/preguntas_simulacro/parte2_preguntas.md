# Parte 2 — Introducción a AWS — Preguntas tipo examen

20 preguntas de opción múltiple, sin respuestas marcadas, para autoevaluación.

**Pregunta 1.** Una empresa necesita cumplir con una regulación que exige que los datos de sus clientes europeos nunca salgan de la Unión Europea. ¿Qué concepto de la infraestructura global de AWS le permite garantizar esto?

- A) Availability Zones
- B) Edge Locations
- C) Regiones
- D) Placement Groups

**Pregunta 2.** ¿Qué es una Availability Zone (AZ)?

- A) Un país donde AWS tiene presencia
- B) Uno o más data centers físicamente separados dentro de una Región, con energía, refrigeración y conectividad independientes
- C) Un servidor de caché cerca del usuario final
- D) El nombre técnico de una cuenta de AWS

**Pregunta 3.** ¿Por qué AWS recomienda desplegar aplicaciones críticas en al menos dos Availability Zones distintas?

- A) Porque es obligatorio por ley en todos los países
- B) Para reducir el costo total de la infraestructura
- C) Para que, si una AZ completa falla (por ejemplo, un corte eléctrico), la aplicación siga disponible desde la otra AZ
- D) Porque una sola AZ no puede alojar más de una instancia EC2

**Pregunta 4.** ¿Qué son las Edge Locations de AWS?

- A) Centros de datos completos donde se pueden lanzar instancias EC2
- B) Sitios más pequeños y numerosos, distribuidos globalmente, usados para entregar contenido con baja latencia (ej. CloudFront)
- C) Un sinónimo de Región
- D) El nombre de las oficinas comerciales de AWS

**Pregunta 5.** Una empresa de streaming de video quiere que sus usuarios en todo el mundo experimenten baja latencia al cargar el contenido. ¿Qué componente de la infraestructura global de AWS es más relevante para este objetivo?

- A) Regiones adicionales exclusivamente
- B) Availability Zones adicionales exclusivamente
- C) Edge Locations a través de Amazon CloudFront
- D) AWS Direct Connect

**Pregunta 6.** ¿Cuál de las siguientes afirmaciones sobre las Regiones de AWS es correcta?

- A) Todas las Regiones tienen exactamente el mismo conjunto de servicios disponibles
- B) Cada Región está compuesta por múltiples Availability Zones aisladas entre sí
- C) Una Región y una Availability Zone son el mismo concepto
- D) Las Regiones solo existen en Estados Unidos

**Pregunta 7.** Un arquitecto debe elegir en qué Región desplegar una nueva aplicación. ¿Cuál de los siguientes NO es un criterio típico mencionado por AWS para esta decisión?

- A) Cumplimiento normativo y soberanía de datos
- B) Latencia hacia los usuarios finales
- C) Disponibilidad de servicios específicos en esa Región
- D) El color del logotipo regional de AWS

**Pregunta 8.** ¿Qué herramienta de AWS permite interactuar con los servicios escribiendo comandos en una terminal, ideal para automatización y scripts?

- A) AWS Management Console
- B) AWS CLI (Command Line Interface)
- C) AWS Marketplace
- D) Amazon Chime

**Pregunta 9.** Un desarrollador quiere integrar llamadas a servicios de AWS directamente dentro del código de su aplicación Python, sin usar la consola ni la terminal. ¿Qué debería usar?

- A) AWS Management Console
- B) AWS CLI
- C) Un AWS SDK (por ejemplo, Boto3 para Python)
- D) AWS Snowball

**Pregunta 10.** ¿Cuál es la forma más básica y de más bajo nivel de interactuar con los servicios de AWS, sobre la cual se construyen tanto la consola como el CLI y los SDK?

- A) AWS Marketplace
- B) Las APIs de AWS (llamadas HTTPS con firma)
- C) AWS Organizations
- D) Amazon Connect

**Pregunta 11.** Una empresa nueva en AWS quiere que su equipo, sin experiencia técnica en línea de comandos, pueda lanzar y configurar recursos de forma visual. ¿Qué herramienta es la más adecuada para empezar?

- A) AWS CLI
- B) AWS Management Console
- C) AWS SDK para Java
- D) API Gateway

**Pregunta 12.** ¿Qué comando de AWS CLI usarías para listar los buckets de S3 en tu cuenta?

- A) aws ec2 describe-instances
- B) aws s3 ls
- C) aws iam list-users
- D) aws lambda list-functions

**Pregunta 13.** Una empresa con oficinas en Japón, Alemania y Brasil quiere ofrecer baja latencia a sus usuarios en cada una de esas regiones geográficas, además de cumplir requisitos de residencia de datos locales en cada país. ¿Qué estrategia de infraestructura global es más adecuada?

- A) Desplegar todo en una única Región de Estados Unidos
- B) Desplegar la aplicación en múltiples Regiones de AWS cercanas a cada mercado (ej. ap-northeast-1, eu-central-1, sa-east-1)
- C) Usar únicamente Edge Locations sin ninguna Región adicional
- D) Usar solo una Availability Zone adicional en la misma Región

**Pregunta 14.** ¿Qué diferencia principal existe entre una Región y una Availability Zone?

- A) Son sinónimos, AWS los usa indistintamente
- B) Una Región es un área geográfica que contiene múltiples Availability Zones aisladas físicamente entre sí
- C) Una Availability Zone contiene múltiples Regiones
- D) Las Availability Zones solo existen fuera de Estados Unidos

**Pregunta 15.** Un equipo de DevOps necesita automatizar el despliegue de 50 instancias EC2 idénticas como parte de un pipeline de integración continua, sin intervención manual. ¿Qué método de acceso a AWS es el más apropiado?

- A) AWS Management Console exclusivamente
- B) AWS CLI o AWS SDK dentro de un script automatizado
- C) Llamar a un representante de soporte de AWS
- D) AWS Artifact

**Pregunta 16.** ¿Cuál de las siguientes NO es una razón típica para que AWS lance una nueva Región en un país?

- A) Reducir la latencia para usuarios de esa zona geográfica
- B) Cumplir con requisitos de soberanía y residencia de datos locales
- C) Dar servicio a clientes gubernamentales o regulados de ese país
- D) Aumentar el número de acciones de la empresa en la bolsa de ese país

**Pregunta 17.** ¿Qué característica NO corresponde a las Edge Locations?

- A) Son más numerosas que las Regiones
- B) Se usan para cachear contenido y reducir latencia con CloudFront
- C) Permiten lanzar instancias EC2 completas de forma directa como en una Región
- D) También son usadas por Route 53 para resolución DNS de baja latencia

**Pregunta 18.** Un arquitecto está diseñando la primera arquitectura de una startup y debe decidir cuántas Availability Zones usar como mínimo para tener alta disponibilidad real. ¿Cuál es la recomendación estándar de AWS?

- A) Una sola AZ es suficiente en cualquier caso
- B) Al menos dos AZ distintas dentro de la misma Región
- C) Es obligatorio usar todas las AZ de la Región
- D) Ninguna AZ, solo Edge Locations

**Pregunta 19.** ¿Qué es AWS Local Zones?

- A) Un sinónimo de Región
- B) Una extensión de infraestructura de AWS más cercana a grandes centros de población/industria, para cargas de trabajo que requieren latencia de un solo dígito de milisegundos
- C) El nombre técnico del usuario root
- D) Una herramienta de facturación

**Pregunta 20.** Un examinador presenta un escenario donde una empresa necesita elegir entre usar la consola, el CLI o un SDK para una tarea puntual de configurar manualmente, por primera vez, una VPC nueva mientras aprende sus opciones visualmente. ¿Cuál es la mejor elección?

- A) AWS SDK
- B) AWS CLI
- C) AWS Management Console
- D) AWS Direct Connect
