# Parte 12 — Well-Architected Framework — Preguntas tipo examen

20 preguntas de opción múltiple, sin respuestas marcadas, para autoevaluación.

**Pregunta 1.** ¿Cuántos pilares componen el AWS Well-Architected Framework en su versión actual?

- A) Cuatro
- B) Cinco
- C) Seis
- D) Ocho

**Pregunta 2.** ¿Qué pilar del Well-Architected Framework se enfoca en la capacidad de ejecutar y monitorear sistemas para entregar valor de negocio, y en mejorar continuamente los procesos y procedimientos de soporte?

- A) Seguridad
- B) Excelencia Operacional (Operational Excellence)
- C) Sostenibilidad
- D) Eficiencia del Rendimiento

**Pregunta 3.** ¿Qué pilar del Well-Architected Framework aborda la protección de la información, los sistemas y los activos, aplicando el principio de mínimo privilegio y trazabilidad de acciones?

- A) Fiabilidad
- B) Seguridad (Security)
- C) Optimización de costos
- D) Excelencia operacional

**Pregunta 4.** ¿Qué pilar del Well-Architected Framework se enfoca en la capacidad de un sistema de recuperarse de interrupciones de infraestructura o servicio, adquirir dinámicamente recursos, y mitigar problemas como errores de configuración o de red?

- A) Fiabilidad (Reliability)
- B) Sostenibilidad
- C) Excelencia operacional
- D) Seguridad

**Pregunta 5.** ¿Qué pilar del Well-Architected Framework se centra en usar los recursos de cómputo de forma eficiente para satisfacer los requisitos del sistema, y en mantener esa eficiencia a medida que cambian la demanda y las tecnologías disponibles?

- A) Eficiencia del Rendimiento (Performance Efficiency)
- B) Optimización de costos
- C) Seguridad
- D) Fiabilidad

**Pregunta 6.** ¿Qué pilar del Well-Architected Framework se enfoca en evitar gastos innecesarios y en obtener el mayor valor de negocio del dinero invertido en la nube?

- A) Sostenibilidad
- B) Optimización de Costos (Cost Optimization)
- C) Fiabilidad
- D) Excelencia operacional

**Pregunta 7.** ¿Qué pilar del Well-Architected Framework, añadido más recientemente a los cinco originales, se enfoca en minimizar el impacto ambiental de ejecutar cargas de trabajo en la nube?

- A) Sostenibilidad (Sustainability)
- B) Seguridad
- C) Fiabilidad
- D) Excelencia operacional

**Pregunta 8.** Una empresa automatiza sus despliegues usando pipelines de CI/CD, documenta sus procedimientos operativos estándar, y realiza revisiones periódicas ('game days') simulando fallos para mejorar su capacidad de respuesta ante incidentes. ¿Qué pilar del Well-Architected Framework ilustran mejor estas prácticas?

- A) Optimización de costos
- B) Excelencia Operacional
- C) Sostenibilidad
- D) Seguridad

**Pregunta 9.** Una aplicación aplica cifrado en tránsito (TLS) y en reposo (KMS) a todos sus datos, sigue el principio de mínimo privilegio en sus roles de IAM, y mantiene un registro completo de auditoría con CloudTrail. ¿Qué pilar del Well-Architected Framework describe mejor este conjunto de prácticas?

- A) Fiabilidad
- B) Seguridad
- C) Eficiencia del rendimiento
- D) Sostenibilidad

**Pregunta 10.** Una aplicación está desplegada en múltiples Availability Zones con Auto Scaling, realiza backups automáticos regulares, y tiene un plan de recuperación ante desastres probado periódicamente en una Región secundaria. ¿Qué pilar ilustran mejor estas decisiones de diseño?

- A) Fiabilidad
- B) Optimización de costos exclusivamente
- C) Sostenibilidad exclusivamente
- D) Excelencia operacional exclusivamente

**Pregunta 11.** Un equipo realiza pruebas de carga periódicas para validar que su arquitectura sigue cumpliendo los requisitos de rendimiento a medida que crece el tráfico, y evalúa regularmente si existen tipos de instancia más nuevos y eficientes disponibles para su carga de trabajo. ¿Qué pilar describen mejor estas prácticas?

- A) Eficiencia del Rendimiento
- B) Seguridad
- C) Optimización de costos exclusivamente, sin relación con rendimiento
- D) Sostenibilidad exclusivamente

**Pregunta 12.** Un equipo revisa mensualmente sus recomendaciones de Trusted Advisor, elimina recursos no utilizados, y ajusta el tamaño de sus instancias según patrones de uso reales observados en CloudWatch. ¿Qué pilar del Well-Architected Framework describen mejor estas acciones?

- A) Optimización de Costos
- B) Fiabilidad exclusivamente
- C) Seguridad exclusivamente
- D) Sostenibilidad exclusivamente, sin relación con costos

**Pregunta 13.** Una empresa decide migrar sus cargas de trabajo esporádicas de servidores EC2 siempre encendidos hacia AWS Lambda, reduciendo el tiempo de cómputo ocioso y, como consecuencia, tanto el costo como el consumo energético asociado. ¿Qué DOS pilares del Well-Architected Framework se benefician simultáneamente de esta decisión?

- A) Seguridad y Fiabilidad exclusivamente
- B) Optimización de Costos y Sostenibilidad
- C) Excelencia Operacional exclusivamente
- D) Eficiencia del rendimiento exclusivamente, sin relación con costos ni sostenibilidad

**Pregunta 14.** ¿Qué herramienta gratuita de AWS permite realizar una revisión estructurada de una carga de trabajo específica contra los seis pilares del Well-Architected Framework, generando un reporte de riesgos identificados y recomendaciones?

- A) AWS Trusted Advisor exclusivamente
- B) AWS Well-Architected Tool
- C) Amazon Inspector
- D) AWS Config exclusivamente

**Pregunta 15.** Una empresa evalúa reducir el tamaño de sus componentes de infraestructura al mínimo necesario para cumplir los requisitos de negocio, evitando sobreaprovisionar 'por si acaso', como parte de su estrategia para reducir tanto costos como huella ambiental. ¿A qué principio de diseño del Well-Architected Framework corresponde esto más directamente?

- A) Un principio compartido entre Optimización de Costos y Sostenibilidad: maximizar la utilización y evitar el desperdicio de recursos aprovisionados
- B) Un principio exclusivo de Seguridad
- C) Un principio exclusivo de Fiabilidad, sin relación con costos
- D) No corresponde a ningún principio formal del framework

**Pregunta 16.** ¿Qué principio de diseño del pilar de Fiabilidad sugiere probar procedimientos de recuperación mediante fallos simulados en lugar de esperar a que ocurra un fallo real para descubrir si el plan de recuperación funciona?

- A) Automatizar la recuperación ante fallos y probarla mediante simulacros (como 'game days' o chaos engineering)
- B) Usar siempre la instancia EC2 más grande disponible
- C) Evitar cualquier tipo de automatización
- D) Desactivar los backups para simplificar la arquitectura

**Pregunta 17.** Un arquitecto está diseñando una nueva carga de trabajo y se pregunta: '¿cómo sabré si algo va mal, y podré responder rápidamente si ocurre?'. ¿A qué pilar del Well-Architected Framework corresponde principalmente esta pregunta?

- A) Excelencia Operacional, especialmente en cuanto a monitoreo y respuesta a eventos
- B) Sostenibilidad exclusivamente
- C) Optimización de costos exclusivamente
- D) Eficiencia del rendimiento exclusivamente

**Pregunta 18.** ¿Cuál de las siguientes afirmaciones describe correctamente la relación entre los seis pilares del Well-Architected Framework?

- A) Son completamente independientes entre sí y nunca se relacionan en las decisiones de arquitectura reales
- B) Con frecuencia existen trade-offs entre pilares (por ejemplo, mayor fiabilidad mediante redundancia puede aumentar el costo), y las decisiones de arquitectura deben balancear conscientemente estos pilares según las prioridades del negocio
- C) Solo el pilar de Seguridad importa realmente; los demás son opcionales
- D) Los seis pilares deben maximizarse simultáneamente al 100% en cualquier carga de trabajo, sin excepción

**Pregunta 19.** ¿Qué recomienda el pilar de Sostenibilidad respecto a la elección de la Región de AWS para desplegar una carga de trabajo, cuando el requisito de latencia lo permite?

- A) Elegir siempre la Región más cara disponible
- B) Considerar Regiones donde la infraestructura de AWS use una mayor proporción de energía renovable, cuando otros requisitos (latencia, cumplimiento, costo) lo permitan
- C) La elección de Región nunca tiene relación con la sostenibilidad
- D) Elegir siempre la Región con más Availability Zones, sin importar otros factores

**Pregunta 20.** Una startup en etapa muy temprana decide priorizar la velocidad de lanzamiento al mercado (time-to-market) sobre una arquitectura de fiabilidad máxima con múltiples Regiones redundantes, planeando invertir en mayor redundancia una vez validado el producto. ¿Es esta decisión coherente con la filosofía del Well-Architected Framework?

- A) No, el framework exige implementar el máximo nivel de los seis pilares desde el día uno sin excepción
- B) Sí, el framework reconoce que las decisiones de arquitectura implican trade-offs conscientes según el contexto de negocio, y una startup en validación temprana puede priorizar razonablemente velocidad sobre fiabilidad máxima, revisando esa decisión a medida que el negocio madura
- C) No, esta decisión viola directamente el pilar de Seguridad
- D) El framework no tiene ninguna opinión sobre priorización de pilares según etapa de negocio
