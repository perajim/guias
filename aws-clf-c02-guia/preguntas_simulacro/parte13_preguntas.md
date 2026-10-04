# Parte 13 — Servicios Adicionales — Preguntas tipo examen

19 preguntas de opción múltiple, sin respuestas marcadas, para autoevaluación.

**Pregunta 1.** ¿Qué es AWS CloudFormation?

- A) Un servicio de monitoreo de infraestructura
- B) Un servicio que permite definir y aprovisionar infraestructura de AWS de forma declarativa usando archivos de texto (JSON o YAML), tratando la infraestructura como código
- C) Un tipo de instancia EC2
- D) Un servicio exclusivo de backup

**Pregunta 2.** ¿Qué es el AWS Cloud Development Kit (CDK)?

- A) Un servicio de bases de datos NoSQL
- B) Un framework que permite definir infraestructura de AWS usando lenguajes de programación de propósito general (como Python, TypeScript o Java), que luego se sintetiza en plantillas de CloudFormation
- C) Un tipo de instancia EC2 optimizada para desarrollo
- D) Un servicio exclusivo de testing de software

**Pregunta 3.** Una empresa con docenas de cuentas de AWS quiere establecer una zona de aterrizaje (landing zone) con buenas prácticas de gobernanza preconfiguradas desde el inicio, simplificando la creación de nuevas cuentas que ya cumplan con esas políticas. ¿Qué servicio de AWS está diseñado específicamente para esto?

- A) AWS Control Tower
- B) AWS CloudFormation exclusivamente
- C) AWS Backup
- D) AWS DataSync

**Pregunta 4.** ¿Qué problema resuelve AWS Backup?

- A) Centralizar y automatizar la gestión de copias de seguridad (backups) de múltiples servicios de AWS (EBS, RDS, DynamoDB, EFS, entre otros) desde un único lugar, con políticas de retención definidas centralmente
- B) Migrar bases de datos entre distintos motores
- C) Transferir grandes volúmenes de datos físicamente mediante dispositivos
- D) Orquestar despliegues de infraestructura como código

**Pregunta 5.** Una empresa está evaluando qué aplicaciones y servidores on-premises son candidatos adecuados para migrar a la nube, y necesita una herramienta que le ayude a rastrear el progreso de una migración a gran escala con muchos servidores. ¿Qué servicio de AWS está diseñado para este propósito?

- A) AWS Migration Hub
- B) AWS Snowball
- C) Amazon Neptune
- D) AWS Shield

**Pregunta 6.** ¿Qué es AWS Database Migration Service (DMS)?

- A) Un servicio de backup exclusivo para RDS
- B) Un servicio que ayuda a migrar bases de datos hacia AWS de forma segura, permitiendo incluso migrar entre motores de base de datos distintos, con la base de datos de origen permaneciendo operativa durante la migración
- C) Un tipo de instancia EC2 optimizada para bases de datos
- D) Un servicio de análisis de datos

**Pregunta 7.** ¿Qué problema resuelve AWS DataSync?

- A) Migrar y sincronizar grandes volúmenes de datos entre sistemas de almacenamiento on-premises (o de otras nubes) y servicios de almacenamiento de AWS, de forma rápida y automatizada
- B) Migrar bases de datos relacionales entre motores distintos
- C) Orquestar despliegues de infraestructura como código
- D) Centralizar la gestión de backups de múltiples servicios

**Pregunta 8.** Una empresa necesita transferir 200 TB de datos históricos desde su data center hacia AWS, y su conexión a internet disponible tardaría varias semanas en completar esa transferencia. ¿Qué servicio de la familia Snow es el más adecuado para este volumen específico?

- A) AWS DataSync exclusivamente, sin usar ningún dispositivo físico
- B) AWS Snowball (o Snowball Edge, según el volumen y necesidad de cómputo local)
- C) AWS Database Migration Service
- D) AWS Migration Hub exclusivamente

**Pregunta 9.** ¿Qué distingue a AWS Snowball Edge de un dispositivo AWS Snowball estándar?

- A) No hay diferencia real entre ambos
- B) Snowball Edge añade capacidad de cómputo local (puede correr instancias EC2 o funciones Lambda directamente en el dispositivo) además de la transferencia de datos, útil para procesar datos en ubicaciones con conectividad limitada
- C) Snowball Edge solo puede usarse para bases de datos
- D) Snowball Edge es exclusivamente para transferencias menores a 1 GB

**Pregunta 10.** ¿Qué servicio de AWS proporciona recuperación ante desastres (disaster recovery) para servidores físicos, virtuales o en la nube, replicando continuamente esos servidores hacia AWS para poder recuperarlos rápidamente en caso de un desastre?

- A) AWS Elastic Disaster Recovery (DRS)
- B) AWS Backup exclusivamente
- C) AWS Snowball
- D) AWS Migration Hub

**Pregunta 11.** ¿Qué ventaja ofrece AWS CDK frente a escribir plantillas de CloudFormation directamente en YAML o JSON para infraestructura compleja?

- A) CDK elimina completamente la necesidad de CloudFormation
- B) CDK permite usar lenguajes de programación de propósito general con bucles, condicionales, funciones reutilizables y tipado, facilitando la construcción de infraestructura compleja y reutilizable, que luego se sintetiza en CloudFormation
- C) CDK solo funciona para bases de datos
- D) CDK es más lento que escribir YAML manualmente en cualquier escenario

**Pregunta 12.** Una organización usa AWS Control Tower para gestionar la creación de nuevas cuentas de AWS. ¿Qué servicio subyacente utiliza Control Tower para la gestión multi-cuenta y facturación consolidada?

- A) AWS Organizations
- B) AWS Backup
- C) AWS Snowball
- D) Amazon Route 53

**Pregunta 13.** ¿Qué diferencia principal existe entre AWS DMS y AWS SCT (Schema Conversion Tool), cuando se usan juntos en una migración heterogénea de base de datos (por ejemplo, de Oracle a Aurora PostgreSQL)?

- A) Son el mismo servicio con nombres distintos
- B) SCT convierte el esquema y el código de la base de datos de origen (procedimientos almacenados, vistas) a la sintaxis del motor de destino; DMS migra y sincroniza los DATOS en sí desde el origen hacia el destino
- C) DMS convierte esquemas; SCT migra datos
- D) Ninguno de los dos se usa para migraciones entre motores distintos

**Pregunta 14.** ¿Qué tipo de recursos puede proteger AWS Backup de forma centralizada?

- A) Únicamente instancias EC2, sin ningún otro servicio
- B) Múltiples tipos de recursos como volúmenes EBS, bases de datos RDS, tablas DynamoDB, sistemas de archivos EFS, y otros servicios compatibles, todo desde una consola centralizada
- C) Únicamente buckets de S3
- D) Únicamente configuraciones de IAM

**Pregunta 15.** Una empresa está migrando una aplicación monolítica compleja y quiere primero entender qué componentes existen, sus dependencias, y el estado de avance de la migración de cada uno, consolidando información proveniente de distintas herramientas de migración usadas por diferentes equipos. ¿Qué servicio de AWS ofrece esa visibilidad centralizada?

- A) AWS Migration Hub
- B) AWS Elastic Disaster Recovery
- C) AWS Snowmobile
- D) Amazon Neptune

**Pregunta 16.** ¿Cuál de los siguientes NO sería un caso de uso típico de AWS DataSync?

- A) Migrar un gran volumen de archivos desde un servidor NFS on-premises hacia Amazon S3
- B) Sincronizar de forma recurrente datos entre un sistema de archivos EFS y un almacenamiento on-premises para respaldo continuo
- C) Migrar el esquema y los datos de una base de datos Oracle hacia Amazon Aurora
- D) Transferir datos entre un bucket S3 y un sistema de archivos FSx for Windows

**Pregunta 17.** ¿Qué beneficio clave ofrece 'Infrastructure as Code' (infraestructura como código), como la que permite CloudFormation, frente a crear recursos manualmente clic a clic en la consola?

- A) Ningún beneficio real, ambos enfoques son equivalentes en la práctica
- B) Permite versionar, revisar, reutilizar y reproducir la infraestructura de forma consistente y automatizada, reduciendo errores humanos y facilitando la replicación de entornos idénticos
- C) Infrastructure as Code solo funciona para bases de datos
- D) Elimina completamente la necesidad de entender los servicios de AWS subyacentes

**Pregunta 18.** Una empresa con un data center que sufre un desastre natural necesita conmutar sus servidores críticos hacia AWS en cuestión de minutos, con la menor pérdida de datos posible, habiendo preparado previamente la replicación continua de esos servidores. ¿Qué servicio de AWS está diseñado exactamente para este escenario?

- A) AWS Elastic Disaster Recovery (DRS)
- B) AWS Snowball
- C) AWS CDK
- D) AWS Migration Hub exclusivamente

**Pregunta 19.** ¿Qué combinación de servicios describiría mejor una estrategia de migración de una gran empresa que necesita: (1) mover 500 TB de archivos históricos, (2) migrar su base de datos Oracle a Aurora, y (3) tener visibilidad centralizada del progreso completo?

- A) AWS Snowball para los archivos, AWS DMS (con SCT) para la base de datos, y AWS Migration Hub para la visibilidad centralizada
- B) Usar únicamente AWS CloudFormation para todo el proceso
- C) Usar únicamente AWS Backup para todo el proceso
- D) Usar únicamente Amazon Route 53 para todo el proceso
