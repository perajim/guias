# Parte 1 — Introducción al Cloud Computing — Preguntas tipo examen

20 preguntas de opción múltiple, sin respuestas marcadas, para autoevaluación.

**Pregunta 1.** Una startup quiere lanzar una aplicación web sin comprar ni administrar servidores físicos, pagando solo por lo que consume. ¿Qué modelo de cloud computing describe mejor esta necesidad?

- A) On-premises con virtualización
- B) IaaS tradicional con servidores reservados por años
- C) Cloud computing público bajo modelo pay-as-you-go
- D) Un data center privado gestionado por un tercero

**Pregunta 2.** Una empresa contrata Gmail para el correo corporativo de sus empleados sin instalar ni mantener ningún servidor. ¿Qué modelo de servicio en la nube representa esto?

- A) IaaS
- B) PaaS
- C) SaaS
- D) FaaS

**Pregunta 3.** Un equipo de desarrollo quiere desplegar su código sin preocuparse por el sistema operativo, parches ni el servidor subyacente, pero sí controla la lógica de la aplicación. ¿Qué modelo encaja mejor?

- A) IaaS
- B) PaaS
- C) SaaS
- D) On-premises

**Pregunta 4.** ¿Qué modelo de servicio da al cliente el mayor control sobre el sistema operativo y el software instalado, a cambio de mayor responsabilidad de administración?

- A) SaaS
- B) PaaS
- C) IaaS
- D) FaaS

**Pregunta 5.** Una empresa ejecuta una función que procesa imágenes solo cuando un usuario sube un archivo, sin mantener ningún servidor corriendo el resto del tiempo. ¿Qué modelo es este?

- A) IaaS
- B) PaaS
- C) SaaS
- D) FaaS (serverless)

**Pregunta 6.** ¿Cuál de las siguientes NO es una característica esencial del cloud computing según la definición estándar (NIST)?

- A) Autoservicio bajo demanda
- B) Acceso amplio a la red
- C) Propiedad exclusiva del hardware por parte del cliente
- D) Elasticidad rápida

**Pregunta 7.** Una empresa mantiene datos sensibles en su propio data center pero usa AWS para picos de demanda en época navideña. ¿Qué modelo de despliegue es este?

- A) Nube pública
- B) Nube privada
- C) Nube híbrida
- D) Nube comunitaria

**Pregunta 8.** ¿Qué técnica permite ejecutar múltiples máquinas virtuales aisladas sobre un mismo servidor físico?

- A) Contenedorización
- B) Virtualización
- C) Elasticidad
- D) Federación de identidades

**Pregunta 9.** Una aplicación en AWS aumenta automáticamente el número de instancias EC2 durante un pico de tráfico y las reduce cuando el tráfico baja. ¿Qué concepto de la nube ilustra esto?

- A) Alta disponibilidad
- B) Elasticidad
- C) Tolerancia a fallos
- D) Recuperación ante desastres

**Pregunta 10.** ¿Cuál es la diferencia principal entre escalabilidad y elasticidad?

- A) Son sinónimos exactos
- B) Escalabilidad es la capacidad del sistema de crecer para soportar más carga; elasticidad es hacerlo automáticamente y de forma reversible según demanda
- C) Elasticidad solo aplica a bases de datos
- D) Escalabilidad solo se logra con hardware físico

**Pregunta 11.** Una aplicación crítica está desplegada en dos Availability Zones distintas dentro de la misma región para que si una falla, la otra siga sirviendo tráfico. Esto es un ejemplo de:

- A) Recuperación ante desastres
- B) Alta disponibilidad
- C) Escalabilidad vertical
- D) FaaS

**Pregunta 12.** ¿Qué diferencia a la tolerancia a fallos de la alta disponibilidad?

- A) No hay diferencia
- B) La tolerancia a fallos busca que el sistema siga funcionando SIN degradación perceptible ante el fallo de un componente; la alta disponibilidad minimiza el downtime pero puede tolerar una breve degradación
- C) La tolerancia a fallos solo aplica a redes
- D) La alta disponibilidad requiere múltiples regiones obligatoriamente

**Pregunta 13.** Una empresa replica su infraestructura crítica en una región de AWS distinta a la principal, con capacidad de activarla en minutos si la región principal falla por completo. Esto describe:

- A) Elasticidad
- B) Recuperación ante desastres (Disaster Recovery)
- C) Virtualización
- D) PaaS

**Pregunta 14.** ¿Cuál de los siguientes es un beneficio típico del cloud computing frente a infraestructura on-premises?

- A) Eliminación total de cualquier responsabilidad de seguridad para el cliente
- B) Conversión de CAPEX (gasto de capital) en OPEX (gasto operativo)
- C) Garantía de cero downtime en todos los casos
- D) Imposibilidad de sufrir sobrecostos

**Pregunta 15.** Una empresa pequeña sin equipo de TI grande decide migrar a la nube principalmente porque no quiere encargarse de reemplazar hardware ni parchear sistemas operativos de forma manual. ¿Qué beneficio del cloud busca principalmente?

- A) Velocidad de despliegue global
- B) Reducción de la carga operativa (menos 'undifferentiated heavy lifting')
- C) Elasticidad de red
- D) Federación de identidades

**Pregunta 16.** ¿Qué modelo de despliegue de nube es utilizado exclusivamente por una sola organización, ya sea gestionado internamente o por un tercero?

- A) Nube pública
- B) Nube privada
- C) Nube híbrida
- D) Multi-cloud

**Pregunta 17.** En el examen CLF-C02, una pregunta describe una empresa que necesita capacidad de cómputo solo durante 3 horas al día para procesar reportes nocturnos, y quiere minimizar costos. ¿Qué característica del cloud es más relevante para resolver este caso?

- A) Alta disponibilidad
- B) Elasticidad y modelo de pago por uso
- C) Tolerancia a fallos
- D) Nube comunitaria

**Pregunta 18.** ¿Cuál de estas opciones describe mejor la 'agilidad' como beneficio del cloud computing?

- A) La capacidad de aprovisionar recursos de TI en minutos en lugar de semanas o meses
- B) La velocidad de la red interna de AWS
- C) La cantidad de regiones disponibles
- D) El número de Availability Zones por región

**Pregunta 19.** Una empresa global despliega su aplicación en varias regiones de AWS para que los usuarios de cada continente tengan baja latencia. ¿Qué beneficio del cloud está aprovechando principalmente?

- A) Elasticidad
- B) Alcance global (Go Global in Minutes)
- C) Tolerancia a fallos exclusivamente
- D) PaaS

**Pregunta 20.** Un examinador pregunta cuál es la MEJOR razón para que una empresa adopte un modelo de nube híbrida en lugar de ir 100% a la nube pública de inmediato. ¿Cuál es la respuesta más alineada con el enfoque de AWS?

- A) Porque la nube pública siempre es más cara
- B) Porque permite una migración gradual manteniendo cargas de trabajo con requisitos regulatorios o de latencia específicos on-premises mientras se migra el resto
- C) Porque AWS no ofrece suficiente capacidad
- D) Porque la nube híbrida elimina la necesidad de IAM
