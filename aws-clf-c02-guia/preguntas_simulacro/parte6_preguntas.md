# Parte 6 — Bases de Datos — Preguntas tipo examen

20 preguntas de opción múltiple, sin respuestas marcadas, para autoevaluación.

**Pregunta 1.** Una empresa necesita migrar su base de datos MySQL on-premises a AWS, manteniendo el mismo motor y minimizando cambios en la aplicación, además de que AWS administre los parches y backups automáticamente. ¿Qué servicio es el más adecuado?

- A) Amazon DynamoDB
- B) Amazon RDS
- C) Amazon Redshift
- D) Amazon Neptune

**Pregunta 2.** ¿Qué es Amazon Aurora?

- A) Un motor de base de datos NoSQL exclusivo de AWS
- B) Un motor de base de datos relacional compatible con MySQL y PostgreSQL, desarrollado por AWS, con mayor rendimiento y disponibilidad que las versiones estándar de esos motores en RDS
- C) Un servicio de caché en memoria
- D) Un servicio exclusivo para grafos

**Pregunta 3.** Una aplicación de comercio electrónico con millones de usuarios necesita una base de datos NoSQL capaz de manejar picos masivos de tráfico con latencia de un solo dígito de milisegundos y escalado prácticamente automático. ¿Qué servicio es el más adecuado?

- A) Amazon RDS
- B) Amazon DynamoDB
- C) Amazon Redshift
- D) Amazon DocumentDB

**Pregunta 4.** ¿Qué tipo de carga de trabajo está diseñado para resolver Amazon Redshift?

- A) Transacciones OLTP de baja latencia para una aplicación web
- B) Análisis de datos a gran escala (OLAP) y data warehousing, ejecutando consultas complejas sobre grandes volúmenes históricos de datos
- C) Almacenamiento de sesiones de usuario en caché
- D) Almacenamiento de grafos de relaciones sociales

**Pregunta 5.** Una aplicación de red social necesita almacenar y consultar eficientemente relaciones complejas entre usuarios (amigos de amigos, recomendaciones basadas en conexiones). ¿Qué tipo de base de datos de AWS es la más adecuada?

- A) Amazon Neptune (base de datos de grafos)
- B) Amazon Redshift
- C) Amazon RDS
- D) AWS Snowball

**Pregunta 6.** Una aplicación web experimenta una carga alta de lecturas repetidas sobre los mismos datos desde su base de datos relacional, generando latencia innecesaria. ¿Qué servicio de AWS puede reducir esa carga añadiendo una capa de caché en memoria?

- A) Amazon ElastiCache
- B) Amazon Redshift
- C) AWS Batch
- D) Amazon FSx

**Pregunta 7.** ¿Qué es Amazon DocumentDB?

- A) Un servicio de almacenamiento de archivos PDF
- B) Un servicio de base de datos de documentos totalmente administrado, compatible con MongoDB
- C) Un motor exclusivo de bases de datos relacionales
- D) Un servicio de backup para RDS

**Pregunta 8.** ¿Qué característica de Amazon RDS Multi-AZ mejora la disponibilidad de una base de datos?

- A) Aumenta automáticamente el tamaño del volumen de almacenamiento
- B) Mantiene una réplica en espera (standby) sincronizada en otra Availability Zone, a la que se conmuta automáticamente el tráfico si la instancia primaria falla
- C) Reduce el costo de la base de datos a la mitad
- D) Convierte automáticamente la base de datos en NoSQL

**Pregunta 9.** ¿Cuál es la diferencia principal entre una base de datos relacional (SQL) como RDS y una base de datos NoSQL como DynamoDB, en cuanto al modelo de datos?

- A) No hay diferencia real entre ambos modelos
- B) Las bases relacionales organizan los datos en tablas con esquema fijo y relaciones entre ellas (usando SQL); las NoSQL como DynamoDB usan modelos más flexibles (clave-valor, documentos) sin esquema fijo, optimizados para escalado horizontal
- C) DynamoDB solo puede almacenar números
- D) RDS no puede usarse para aplicaciones web

**Pregunta 10.** Una empresa de análisis financiero necesita ejecutar consultas complejas sobre petabytes de datos históricos de transacciones para generar reportes de negocio. ¿Qué servicio de base de datos de AWS es el más adecuado?

- A) Amazon DynamoDB
- B) Amazon Redshift
- C) Amazon ElastiCache
- D) Amazon RDS para transacciones en tiempo real

**Pregunta 11.** ¿Qué modelo de precios utiliza principalmente Amazon DynamoDB para el consumo de capacidad de lectura/escritura?

- A) Solo un precio fijo mensual sin importar el uso
- B) Modo de capacidad aprovisionada (defines unidades de lectura/escritura) o modo bajo demanda (pagas por solicitud real, sin definir capacidad previa)
- C) Únicamente por gigabyte de almacenamiento, sin cargo por operaciones
- D) Un precio único de por vida al crear la tabla

**Pregunta 12.** Un equipo de desarrollo migra su aplicación de MongoDB on-premises hacia AWS y quiere minimizar los cambios de código relacionados con la base de datos. ¿Qué servicio de AWS es el más adecuado?

- A) Amazon Aurora
- B) Amazon DocumentDB (con compatibilidad MongoDB)
- C) Amazon Redshift
- D) Amazon Neptune

**Pregunta 13.** ¿Qué ventaja ofrece Amazon Aurora frente a ejecutar MySQL directamente en Amazon RDS estándar?

- A) Aurora es siempre más económico en cualquier escenario, sin excepción
- B) Aurora ofrece mayor rendimiento y disponibilidad gracias a su arquitectura de almacenamiento distribuido diseñada específicamente por AWS, manteniendo compatibilidad con MySQL
- C) Aurora no requiere ningún tipo de administración por parte de AWS
- D) Aurora solo funciona fuera de la nube de AWS

**Pregunta 14.** Una aplicación de e-commerce quiere reducir la latencia de las consultas al catálogo de productos, que se leen miles de veces por segundo pero cambian con poca frecuencia. ¿Qué arquitectura de base de datos sería más eficiente?

- A) Consultar siempre directamente a RDS sin ninguna capa adicional
- B) Colocar Amazon ElastiCache delante de RDS/Aurora como capa de caché para las consultas de lectura más frecuentes
- C) Migrar todo el catálogo a Amazon Redshift
- D) Usar exclusivamente Amazon Neptune

**Pregunta 15.** ¿Cuál de las siguientes NO es una característica típica de una base de datos NoSQL como DynamoDB, en comparación con una base de datos relacional?

- A) Escalado horizontal sencillo a través de múltiples servidores
- B) Esquema flexible, sin necesidad de definir todas las columnas de antemano
- C) Soporte nativo y obligatorio para JOINs complejos entre múltiples tablas, igual que SQL
- D) Latencia muy baja y consistente a cualquier escala

**Pregunta 16.** Una empresa de gaming necesita almacenar el estado de sesión de millones de jugadores simultáneos, con lecturas y escrituras extremadamente rápidas y un modelo de datos simple tipo clave-valor. ¿Qué servicio encaja mejor?

- A) Amazon Redshift
- B) Amazon DynamoDB
- C) Amazon Neptune
- D) Amazon RDS con Oracle

**Pregunta 17.** ¿Qué servicio de AWS sería el más adecuado para detectar patrones de fraude analizando las relaciones entre cuentas, transacciones y dispositivos como un grafo de conexiones?

- A) Amazon Redshift
- B) Amazon Neptune
- C) Amazon ElastiCache
- D) AWS Batch

**Pregunta 18.** Un arquitecto está diseñando una base de datos RDS para una aplicación crítica de producción. ¿Qué configuración debería considerar para maximizar la disponibilidad ante el fallo de una Availability Zone?

- A) Usar una sola instancia RDS sin ninguna configuración adicional
- B) Activar RDS Multi-AZ para tener una réplica standby sincronizada en otra AZ con failover automático
- C) Reducir el tamaño de la instancia para ahorrar costos
- D) Deshabilitar los backups automáticos

**Pregunta 19.** ¿Qué son las Read Replicas en Amazon RDS y para qué se usan principalmente?

- A) Copias de solo lectura de la base de datos, usadas para descargar el tráfico de lectura de la instancia principal y mejorar el rendimiento de consultas de lectura, no para alta disponibilidad automática
- B) Backups automáticos diarios de la base de datos
- C) Una función exclusiva de DynamoDB, no de RDS
- D) Un mecanismo para cifrar datos en tránsito

**Pregunta 20.** Una startup necesita elegir entre una base de datos relacional (RDS) y NoSQL (DynamoDB) para el catálogo de productos de su nueva tienda online, que tendrá relaciones complejas entre categorías, variantes, proveedores y pedidos, con la necesidad de hacer consultas relacionales flexibles. ¿Qué opción es probablemente más adecuada al inicio?

- A) Amazon DynamoDB, porque siempre escala mejor que cualquier base relacional
- B) Amazon RDS o Aurora, porque el modelo relacional facilita consultas complejas con JOINs entre categorías, variantes, proveedores y pedidos
- C) Amazon Redshift, porque es la opción más económica para cualquier caso
- D) Amazon Neptune, porque todos los datos de un e-commerce son grafos
