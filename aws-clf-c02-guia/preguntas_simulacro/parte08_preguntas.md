# Parte 8 — Seguridad — Preguntas tipo examen

20 preguntas de opción múltiple, sin respuestas marcadas, para autoevaluación.

**Pregunta 1.** Según el Modelo de Responsabilidad Compartida de AWS, ¿de quién es la responsabilidad de aplicar los parches del hipervisor y la infraestructura física de los data centers?

- A) Del cliente
- B) De AWS (seguridad DE la nube)
- C) Es una responsabilidad compartida al 50/50 en todos los casos
- D) De un proveedor externo contratado por el cliente

**Pregunta 2.** En el Modelo de Responsabilidad Compartida, ¿quién es responsable de configurar correctamente las políticas de IAM y los Security Groups de una aplicación desplegada en EC2?

- A) AWS exclusivamente
- B) El cliente (seguridad EN la nube)
- C) Ninguno de los dos, es automático
- D) Depende del plan de soporte contratado

**Pregunta 3.** ¿Qué es AWS KMS (Key Management Service)?

- A) Un servicio de monitoreo de logs
- B) Un servicio administrado para crear y controlar las claves criptográficas usadas para cifrar datos en distintos servicios de AWS
- C) Un firewall de aplicaciones web
- D) Un servicio exclusivo de backup

**Pregunta 4.** ¿Qué problema resuelve AWS Secrets Manager?

- A) Compilar código fuente de forma segura
- B) Almacenar, rotar y recuperar de forma segura credenciales sensibles como contraseñas de bases de datos, API keys y otros secretos, evitando que se hardcodeen en el código
- C) Cifrar el tráfico de red entre Availability Zones
- D) Escanear vulnerabilidades en imágenes de contenedores

**Pregunta 5.** ¿Qué es AWS Certificate Manager (ACM)?

- A) Un servicio para gestionar licencias de software de terceros
- B) Un servicio que permite aprovisionar, administrar y desplegar certificados SSL/TLS públicos y privados para usar con servicios de AWS como CloudFront o Elastic Load Balancer
- C) Un servicio exclusivo de firma de contratos digitales
- D) Un tipo de instancia EC2 optimizada para criptografía

**Pregunta 6.** ¿Qué tipo de ataque está diseñado para mitigar principalmente AWS Shield?

- A) Ataques de inyección SQL
- B) Ataques de Denegación de Servicio Distribuido (DDoS)
- C) Robo de credenciales por phishing
- D) Fugas de datos por mala configuración de S3

**Pregunta 7.** ¿Qué servicio de AWS protegería una aplicación web contra ataques comunes de inyección SQL y cross-site scripting (XSS) a nivel de capa de aplicación (capa 7)?

- A) AWS Shield exclusivamente
- B) AWS WAF (Web Application Firewall)
- C) Amazon GuardDuty
- D) AWS Config

**Pregunta 8.** ¿Qué es Amazon GuardDuty?

- A) Un firewall de aplicaciones web
- B) Un servicio de detección de amenazas que monitorea continuamente la cuenta de AWS en busca de actividad maliciosa o no autorizada, usando machine learning y fuentes de inteligencia de amenazas
- C) Un servicio de cifrado de datos en reposo
- D) Un servicio de backup automatizado

**Pregunta 9.** ¿Qué evalúa principalmente Amazon Inspector?

- A) El cumplimiento de políticas de facturación
- B) Vulnerabilidades de seguridad y desviaciones de mejores prácticas en instancias EC2, imágenes de contenedores y funciones Lambda
- C) El tráfico DDoS entrante
- D) Los registros de auditoría de acciones de usuarios de IAM

**Pregunta 10.** Una empresa necesita identificar automáticamente si tiene información sensible (como números de tarjetas de crédito o datos personales) almacenada sin protección adecuada en sus buckets de S3. ¿Qué servicio de AWS está diseñado específicamente para esto?

- A) Amazon Macie
- B) AWS Config
- C) Amazon Inspector
- D) AWS Shield

**Pregunta 11.** ¿Qué servicio de AWS registra un historial detallado de TODAS las llamadas a la API realizadas en una cuenta de AWS, incluyendo quién hizo qué, cuándo y desde dónde?

- A) Amazon CloudWatch
- B) AWS CloudTrail
- C) AWS Config
- D) Amazon GuardDuty

**Pregunta 12.** ¿Qué servicio de AWS evalúa continuamente si la configuración de tus recursos cumple con reglas definidas (por ejemplo, 'todos los buckets S3 deben tener cifrado activado'), y registra el historial de cambios de configuración a lo largo del tiempo?

- A) AWS CloudTrail
- B) AWS Config
- C) AWS Trusted Advisor
- D) Amazon Inspector

**Pregunta 13.** ¿Cuál es la diferencia principal entre AWS CloudTrail y AWS Config?

- A) Son el mismo servicio con nombres distintos
- B) CloudTrail registra QUIÉN hizo QUÉ acción (llamadas a la API); Config registra el ESTADO de configuración de los recursos a lo largo del tiempo y evalúa cumplimiento contra reglas
- C) Config solo funciona con S3; CloudTrail funciona con todos los servicios
- D) CloudTrail es de pago; Config es completamente gratuito en todos los casos

**Pregunta 14.** Una aplicación web en AWS necesita servir contenido mediante HTTPS con un certificado SSL/TLS válido, integrado directamente con su Application Load Balancer, sin costo adicional por el certificado en sí. ¿Qué servicio deberían usar?

- A) AWS KMS
- B) AWS Certificate Manager (ACM)
- C) AWS Secrets Manager
- D) Amazon Macie

**Pregunta 15.** ¿Qué combinación de servicios de seguridad de AWS te ayudaría a: (1) detectar actividad maliciosa en tu cuenta, y (2) escanear vulnerabilidades conocidas en tus instancias EC2?

- A) AWS Config y AWS CloudTrail
- B) Amazon GuardDuty y Amazon Inspector
- C) AWS Shield y AWS WAF
- D) AWS KMS y AWS Secrets Manager

**Pregunta 16.** Una empresa quiere rotar automáticamente, cada 30 días, la contraseña de su base de datos RDS sin tener que actualizar manualmente el código de la aplicación cada vez. ¿Qué servicio de AWS resuelve esto de forma nativa?

- A) AWS Secrets Manager, con rotación automática configurada
- B) AWS KMS exclusivamente
- C) Amazon Macie
- D) AWS Shield

**Pregunta 17.** ¿Qué elemento del Modelo de Responsabilidad Compartida cambia según el tipo de servicio que se use (por ejemplo, EC2 tipo IaaS vs un servicio totalmente administrado como Lambda)?

- A) Nada cambia nunca, la división es siempre exactamente la misma
- B) La línea divisoria se desplaza: en servicios más administrados (como Lambda o RDS), AWS asume más responsabilidades operativas (como parchear el sistema operativo subyacente) que en servicios IaaS como EC2
- C) AWS siempre es responsable de todo, sin importar el servicio
- D) El cliente siempre es responsable de todo, sin importar el servicio

**Pregunta 18.** ¿Qué servicio de AWS ayudaría a demostrar, durante una auditoría regulatoria, que un bucket S3 específico tuvo cifrado activado de forma continua durante los últimos 6 meses, y en qué momento (si acaso) se desactivó?

- A) Amazon GuardDuty
- B) AWS Config, revisando el historial de configuración del recurso
- C) AWS Shield
- D) Amazon Macie exclusivamente

**Pregunta 19.** Un equipo de seguridad recibe una alerta indicando que una instancia EC2 dentro de su cuenta está comunicándose con una dirección IP conocida por distribuir malware. ¿Qué servicio de AWS generó probablemente esta alerta?

- A) AWS Config
- B) Amazon GuardDuty
- C) AWS Certificate Manager
- D) AWS Secrets Manager

**Pregunta 20.** ¿Cuál de las siguientes afirmaciones describe mejor la relación entre AWS Shield Standard y AWS Shield Advanced?

- A) Son el mismo servicio, con nombres distintos según la Región
- B) Shield Standard se activa automáticamente sin costo para todos los clientes con protección básica contra DDoS; Shield Advanced ofrece protección más sofisticada, con costo adicional, e incluye acceso a un equipo de respuesta especializado
- C) Shield Advanced es gratuito y Shield Standard tiene costo
- D) Shield Standard solo protege bases de datos, no aplicaciones web
