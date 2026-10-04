# Parte 3 — IAM — Preguntas tipo examen

19 preguntas de opción múltiple, sin respuestas marcadas, para autoevaluación.

**Pregunta 1.** Una empresa tiene 40 empleados que necesitan acceso similar a AWS (todos en el equipo de desarrollo necesitan los mismos permisos sobre S3 y EC2). ¿Cuál es la forma más eficiente de gestionar estos permisos?

- A) Crear 40 policies individuales, una por usuario
- B) Crear un IAM Group con la policy necesaria y añadir los 40 usuarios a ese grupo
- C) Compartir las credenciales del usuario root entre los 40 empleados
- D) Crear 40 IAM Roles, uno por usuario

**Pregunta 2.** ¿Cuál es la diferencia fundamental entre un IAM User y un IAM Role?

- A) No hay diferencia, son sinónimos
- B) Un IAM User tiene credenciales permanentes asociadas a una identidad específica; un IAM Role no tiene credenciales propias y es asumido temporalmente por quien lo necesite
- C) Un IAM Role solo puede ser usado por el usuario root
- D) Un IAM User solo puede acceder a S3

**Pregunta 3.** Una aplicación EC2 necesita leer archivos de un bucket S3. Según las mejores prácticas de AWS, ¿cómo debería otorgarse este acceso?

- A) Creando un IAM User con access keys y guardando esas keys en el código de la aplicación
- B) Asignando un IAM Role a la instancia EC2 con permisos de solo lectura sobre ese bucket específico
- C) Haciendo el bucket S3 completamente público
- D) Usando las credenciales del usuario root en la aplicación

**Pregunta 4.** ¿Qué es una IAM Policy?

- A) Un tipo de instancia EC2
- B) Un documento JSON que define qué acciones están permitidas o denegadas sobre qué recursos
- C) El nombre de un grupo de usuarios
- D) Un servicio de facturación de AWS

**Pregunta 5.** ¿Qué elemento de una IAM Policy determina si el permiso se PERMITE o se DENIEGA explícitamente?

- A) Resource
- B) Action
- C) Effect
- D) Version

**Pregunta 6.** Si un usuario IAM tiene una policy que le PERMITE acceso completo a S3, pero otra policy adjunta le DENIEGA explícitamente el acceso a un bucket específico, ¿qué ocurre?

- A) Prevalece siempre el permiso más reciente que se haya adjuntado
- B) Un DENY explícito siempre prevalece sobre un ALLOW, sin importar el orden en que se evalúen las policies
- C) AWS pide confirmación manual al usuario
- D) El acceso se permite porque hay al menos una policy que lo permite

**Pregunta 7.** ¿Qué es el 'principio de mínimo privilegio' en el contexto de IAM?

- A) Otorgar a cada usuario acceso administrador completo por defecto para evitar problemas operativos
- B) Otorgar a cada identidad únicamente los permisos estrictamente necesarios para realizar su tarea, ni uno más
- C) Usar siempre el usuario root para todas las operaciones
- D) Nunca usar IAM Roles, solo IAM Users

**Pregunta 8.** ¿Qué es MFA (Multi-Factor Authentication) y por qué AWS lo recomienda enfáticamente para el usuario root?

- A) Es un segundo nombre de usuario que se debe recordar
- B) Es una capa adicional de seguridad que requiere un segundo factor (ej. código de una app o dispositivo físico) además de la contraseña, dificultando el acceso no autorizado aunque la contraseña sea robada
- C) Es un tipo de IAM Role especial
- D) Es el nombre técnico de una VPC segura

**Pregunta 9.** Una empresa mediana con cientos de empleados usa Microsoft Active Directory internamente y quiere que sus empleados puedan acceder a AWS usando sus credenciales corporativas existentes, sin crear un IAM User separado para cada uno. ¿Qué solución de AWS es la más adecuada?

- A) Crear 500 IAM Users manualmente
- B) Usar Federación de identidades (Identity Federation), por ejemplo mediante AWS IAM Identity Center o SAML 2.0
- C) Compartir las credenciales del usuario root
- D) Deshabilitar IAM completamente

**Pregunta 10.** ¿Qué es AWS IAM Identity Center (anteriormente conocido como AWS SSO)?

- A) Un tipo de instancia EC2 optimizada para IAM
- B) Un servicio que centraliza el acceso de los usuarios a múltiples cuentas de AWS y aplicaciones empresariales mediante inicio de sesión único (SSO)
- C) Una policy predeterminada de solo lectura
- D) Un servicio exclusivo para IAM Roles de servicios de AWS

**Pregunta 11.** Un desarrollador externo de otra empresa necesita acceso temporal a ciertos recursos específicos de tu cuenta de AWS por un proyecto de 3 meses. Según las mejores prácticas, ¿qué deberías usar?

- A) Crear un IAM User permanente con contraseña compartida por email
- B) Crear un IAM Role que ese desarrollador pueda asumir (cross-account role), con permisos limitados y de duración limitada
- C) Darle las credenciales del usuario root de tu cuenta
- D) Deshabilitar IAM MFA para facilitarle el acceso

**Pregunta 12.** ¿Cuál de las siguientes afirmaciones sobre el usuario root de una cuenta de AWS es correcta?

- A) El usuario root debería usarse para las tareas diarias del equipo
- B) El usuario root tiene control total e irrestricto sobre la cuenta y debería protegerse con MFA y usarse solo para tareas que estrictamente lo requieran
- C) El usuario root no puede eliminarse ni renombrarse, pero tampoco tiene permisos especiales
- D) El usuario root es lo mismo que un IAM Role

**Pregunta 13.** ¿Qué elemento identifica de forma única un recurso específico de AWS dentro de una IAM Policy (por ejemplo, un bucket S3 concreto)?

- A) El Access Key ID
- B) El ARN (Amazon Resource Name)
- C) El Account ID únicamente
- D) El nombre de la Región

**Pregunta 14.** Un IAM Role tiene dos componentes principales de configuración. ¿Cuáles son?

- A) Una policy de permisos (qué puede hacer) y una policy de confianza (quién puede asumir el rol)
- B) Solo un nombre de usuario y una contraseña
- C) Solo una dirección de correo electrónico
- D) Un Access Key ID y un Secret Access Key permanentes

**Pregunta 15.** ¿Qué tipo de policy de IAM viene predefinida y mantenida por AWS, lista para usarse sin tener que escribirla desde cero (ej. 'AmazonS3ReadOnlyAccess')?

- A) Customer managed policy
- B) Inline policy
- C) AWS managed policy
- D) Resource-based policy

**Pregunta 16.** Una startup con un solo desarrollador está usando el usuario root para todo su trabajo diario en AWS, incluyendo lanzar instancias EC2 y configurar S3. ¿Cuál es el riesgo principal y la recomendación correcta?

- A) No hay ningún riesgo, root es igual de seguro que cualquier IAM User
- B) El riesgo es que si las credenciales root se comprometen, el atacante tiene control total de la cuenta; se recomienda crear un IAM User con permisos administrativos para el trabajo diario y reservar root solo para tareas excepcionales
- C) El riesgo es que root no puede lanzar instancias EC2
- D) Se recomienda deshabilitar IAM completamente para simplificar

**Pregunta 17.** ¿Qué ocurre con las credenciales generadas cuando una aplicación asume un IAM Role?

- A) Son permanentes y nunca expiran
- B) Son temporales, con una duración configurable, y se rotan automáticamente sin intervención manual
- C) Son idénticas a las credenciales del usuario root
- D) Deben guardarse manualmente en un archivo de texto por el desarrollador

**Pregunta 18.** Una empresa quiere que los desarrolladores de su equipo de Machine Learning solo puedan ver y usar servicios relacionados con ML (SageMaker, S3 de sus buckets de datasets), sin poder tocar EC2, RDS ni facturación. ¿Qué concepto de IAM aplica directamente este control?

- A) Elasticidad
- B) El principio de mínimo privilegio, implementado mediante policies específicas adjuntas a un grupo de ML
- C) Availability Zones
- D) Edge Locations

**Pregunta 19.** ¿Cuál de las siguientes es una mejor práctica de seguridad recomendada por AWS respecto a las IAM Policies?

- A) Usar siempre la policy 'AdministratorAccess' para todos los usuarios para simplificar la gestión
- B) Revisar y auditar periódicamente los permisos otorgados, eliminando accesos no utilizados, y preferir permisos granulares sobre accesos amplios
- C) Nunca usar AWS managed policies, siempre escribir todo desde cero
- D) Compartir una sola IAM Policy con permisos completos entre todos los equipos
