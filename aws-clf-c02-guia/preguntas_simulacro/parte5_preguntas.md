# Parte 5 — Almacenamiento — Preguntas tipo examen

20 preguntas de opción múltiple, sin respuestas marcadas, para autoevaluación.

**Pregunta 1.** Una empresa necesita almacenar millones de imágenes de usuarios, accesibles vía internet, con alta durabilidad y sin límite práctico de capacidad. ¿Qué servicio de almacenamiento de AWS es el más adecuado?

- A) Amazon EBS
- B) Amazon S3
- C) Amazon EFS
- D) AWS Storage Gateway

**Pregunta 2.** ¿Qué es el versionado (versioning) en Amazon S3?

- A) Una función que borra automáticamente archivos antiguos
- B) Una función que mantiene múltiples variantes de un mismo objeto en el mismo bucket, permitiendo recuperar o restaurar versiones anteriores
- C) El número de versión del motor de S3
- D) Un tipo de clase de almacenamiento

**Pregunta 3.** Una empresa quiere reducir automáticamente el costo de almacenamiento de archivos que se acceden frecuentemente durante los primeros 30 días, pero rara vez después. ¿Qué función de S3 resuelve esto sin intervención manual?

- A) S3 Object Lock
- B) S3 Lifecycle Policies (reglas de ciclo de vida)
- C) S3 Versioning
- D) S3 Transfer Acceleration

**Pregunta 4.** ¿Cuál de las siguientes clases de almacenamiento de S3 está diseñada específicamente para archivado a muy largo plazo, con el costo por GB más bajo, pero con tiempos de recuperación que pueden tardar de minutos a horas?

- A) S3 Standard
- B) S3 Intelligent-Tiering
- C) S3 Glacier Deep Archive
- D) S3 One Zone-IA

**Pregunta 5.** ¿Qué tipo de almacenamiento de AWS se comporta como un disco duro virtual, se adjunta a UNA sola instancia EC2 a la vez (en la mayoría de los casos), y es ideal para el volumen raíz de un sistema operativo o bases de datos?

- A) Amazon S3
- B) Amazon EBS (Elastic Block Store)
- C) Amazon EFS
- D) AWS Snowball

**Pregunta 6.** Una aplicación necesita que múltiples instancias EC2, en distintas Availability Zones, accedan y modifiquen simultáneamente el mismo sistema de archivos compartido. ¿Qué servicio de almacenamiento es el más adecuado?

- A) Amazon EBS
- B) Amazon EFS (Elastic File System)
- C) Amazon S3 Glacier
- D) Amazon Lightsail

**Pregunta 7.** ¿Qué es Amazon FSx?

- A) Un servicio de almacenamiento de objetos económico
- B) Un servicio de sistemas de archivos totalmente administrados, optimizado para motores específicos como Windows File Server, Lustre, NetApp ONTAP o OpenZFS
- C) Un tipo de instancia EC2
- D) Un servicio exclusivo de backup

**Pregunta 8.** Una empresa con un data center on-premises quiere extender su almacenamiento local hacia la nube de forma transparente para sus aplicaciones existentes, sin reescribir su software. ¿Qué servicio de AWS es el más adecuado?

- A) AWS Storage Gateway
- B) Amazon S3 exclusivamente
- C) Amazon EBS exclusivamente
- D) AWS Direct Connect exclusivamente

**Pregunta 9.** ¿Cuál es la diferencia principal entre Amazon EBS y Amazon EFS en cuanto a cómo se comparte el almacenamiento?

- A) No hay diferencia, ambos son idénticos
- B) EBS típicamente se adjunta a una sola instancia EC2 a la vez; EFS puede ser montado simultáneamente por múltiples instancias en distintas AZ
- C) EFS solo funciona con Windows; EBS solo con Linux
- D) EBS es más barato que EFS en todos los casos de uso

**Pregunta 10.** Una empresa financiera debe conservar registros de transacciones por 7 años debido a regulaciones, con acceso extremadamente infrecuente pero garantizando que los archivos no puedan ser modificados ni eliminados antes de ese plazo. ¿Qué combinación de funciones de S3 resuelve este requisito?

- A) S3 Standard sin ninguna configuración adicional
- B) S3 Glacier o Glacier Deep Archive combinado con S3 Object Lock en modo de cumplimiento (Compliance mode)
- C) Solo versionado, sin clase de almacenamiento especial
- D) Amazon EBS con snapshots diarios

**Pregunta 11.** ¿Qué ocurre con las versiones anteriores de un objeto en S3 si NO se activa el versionado y subes un nuevo archivo con el mismo nombre (key)?

- A) Se conservan automáticamente todas las versiones anteriores
- B) El objeto anterior se sobrescribe permanentemente y no se puede recuperar
- C) AWS pide confirmación antes de sobrescribir
- D) El archivo nuevo se rechaza automáticamente

**Pregunta 12.** Una startup necesita almacenamiento de bajo costo para datos que se acceden con poca frecuencia pero que deben estar disponibles de inmediato (milisegundos) cuando se necesiten, sin tiempos de espera de recuperación. ¿Qué clase de S3 encaja mejor?

- A) S3 Glacier Deep Archive
- B) S3 Standard-Infrequent Access (S3 Standard-IA)
- C) S3 Glacier Flexible Retrieval
- D) Amazon EBS Cold HDD

**Pregunta 13.** ¿Qué hace la clase de almacenamiento S3 Intelligent-Tiering?

- A) Requiere que el usuario mueva manualmente los objetos entre niveles de acceso
- B) Mueve automáticamente los objetos entre niveles de acceso frecuente e infrecuente (y opcionalmente archivado) según los patrones de acceso reales, sin penalización por recuperación ni gestión manual
- C) Es la clase de almacenamiento más cara de todo S3
- D) Solo está disponible para archivos menores a 1 MB

**Pregunta 14.** Una empresa necesita transferir 100 TB de datos desde su data center on-premises hacia AWS, y su conexión a internet es demasiado lenta para hacerlo en un tiempo razonable. ¿Qué servicio de la familia Snow debería considerar?

- A) AWS Storage Gateway
- B) AWS Snowball (dispositivo físico de transferencia masiva de datos)
- C) Amazon S3 Transfer Acceleration exclusivamente
- D) Amazon EFS

**Pregunta 15.** ¿Cuál de las siguientes afirmaciones sobre la durabilidad de Amazon S3 Standard es correcta?

- A) S3 Standard está diseñado para una durabilidad del 99.999999999% (11 nueves) replicando datos automáticamente entre múltiples Availability Zones
- B) S3 Standard almacena los datos en una sola Availability Zone únicamente
- C) La durabilidad de S3 depende de que el cliente configure manualmente la replicación
- D) S3 no ofrece ninguna garantía de durabilidad

**Pregunta 16.** Una empresa de medios necesita almacenamiento de alto rendimiento y baja latencia compartido entre cientos de instancias EC2 que procesan renderizado de video en paralelo, similar a un sistema de archivos HPC tradicional. ¿Qué servicio es el más adecuado?

- A) Amazon S3 Standard
- B) Amazon FSx for Lustre
- C) AWS Storage Gateway (Tape Gateway)
- D) Amazon EBS Cold HDD

**Pregunta 17.** ¿Qué tipo de Storage Gateway presentaría un dispositivo de almacenamiento en bloque (similar a iSCSI) para que servidores on-premises lo usen como si fuera un disco local, mientras los datos se replican a AWS?

- A) File Gateway
- B) Volume Gateway
- C) Tape Gateway
- D) Amazon EFS

**Pregunta 18.** ¿Cuál de las siguientes opciones NO es un beneficio típico de usar reglas de ciclo de vida (Lifecycle) en S3?

- A) Reducir automáticamente costos de almacenamiento moviendo datos antiguos a clases más económicas
- B) Eliminar automáticamente objetos después de un periodo definido
- C) Aumentar automáticamente la durabilidad de los objetos por encima del 99.999999999%
- D) Automatizar la transición entre clases de almacenamiento sin intervención manual

**Pregunta 19.** Un equipo de desarrollo necesita el volumen raíz para el sistema operativo de una nueva instancia EC2 que ejecutará una base de datos con requerimientos de baja latencia consistente. ¿Qué tipo de almacenamiento deben usar?

- A) Amazon S3
- B) Amazon EBS (por ejemplo, un volumen tipo gp3 o io2)
- C) Amazon EFS
- D) AWS Snowball

**Pregunta 20.** Una empresa quiere compartir un mismo conjunto de archivos de configuración entre 50 instancias EC2 Linux que corren en tres Availability Zones distintas, con la posibilidad de que todas lean y escriban simultáneamente. ¿Qué servicio de almacenamiento cumple este requisito de la forma más directa?

- A) Amazon EBS con Multi-Attach en un solo volumen
- B) Amazon EFS montado simultáneamente en las 50 instancias vía NFS
- C) Amazon S3 Glacier Deep Archive
- D) AWS Snowball
