# Parte 11 — Costos — Preguntas tipo examen

20 preguntas de opción múltiple, sin respuestas marcadas, para autoevaluación.

**Pregunta 1.** ¿Cuáles son los tres pilares fundamentales del modelo de precios de AWS?

- A) Cómputo, almacenamiento y soporte técnico
- B) Pagas por cómputo, pagas por almacenamiento, y pagas por transferencia de datos saliente (data transfer OUT)
- C) Solo el costo de las licencias de software
- D) Un precio fijo mensual único para toda la cuenta

**Pregunta 2.** ¿Qué herramienta de AWS te permite visualizar y analizar tus patrones de gasto histórico, con la posibilidad de filtrar por servicio, cuenta o etiqueta (tag)?

- A) AWS Budgets
- B) AWS Cost Explorer
- C) AWS Organizations
- D) Savings Plans

**Pregunta 3.** ¿Qué servicio de AWS te permite definir un umbral de gasto y recibir una alerta automática (por ejemplo, por correo) cuando tu gasto real o proyectado se acerca o supera ese umbral?

- A) AWS Cost Explorer
- B) AWS Budgets
- C) AWS Organizations
- D) Reserved Instances

**Pregunta 4.** Una empresa se compromete a usar una cantidad constante de gasto en cómputo por hora (por ejemplo, $10/hora) durante 1 año, a cambio de un descuento significativo, manteniendo flexibilidad para cambiar el tipo de instancia, sistema operativo o Región usada dentro de ese compromiso. ¿Qué modelo de precios de AWS describe esto?

- A) Reserved Instances tradicionales
- B) Savings Plans
- C) Instancias Spot
- D) AWS Free Tier

**Pregunta 5.** ¿Qué caracteriza a las instancias Spot de EC2 en cuanto a precio y disponibilidad?

- A) Precio fijo garantizado de por vida, sin posibilidad de interrupción
- B) Descuentos significativos (hasta 90% frente a On-Demand) sobre capacidad no utilizada de AWS, con la posibilidad de que AWS interrumpa la instancia con poco aviso cuando necesita esa capacidad de vuelta
- C) Requieren un compromiso obligatorio de 3 años
- D) Solo pueden usarse para bases de datos de producción crítica

**Pregunta 6.** Una empresa sabe con certeza que necesitará una instancia de base de datos específica funcionando de forma constante durante los próximos 3 años, y quiere el máximo descuento posible por ese compromiso a largo plazo. ¿Qué opción de precios sería la más económica en este escenario específico?

- A) Instancias On-Demand
- B) Instancias Spot
- C) Reserved Instances a 3 años (o Savings Plans a 3 años) con pago por adelantado
- D) AWS Free Tier exclusivamente

**Pregunta 7.** ¿Qué es AWS Organizations?

- A) Un servicio de gestión de proyectos de equipo
- B) Un servicio que permite gestionar y consolidar de forma centralizada múltiples cuentas de AWS, incluyendo facturación consolidada y políticas de control (SCPs)
- C) Un tipo de instancia EC2 optimizada para grandes empresas
- D) Un servicio exclusivo de Recursos Humanos

**Pregunta 8.** ¿Qué beneficio de facturación ofrece principalmente la facturación consolidada (consolidated billing) de AWS Organizations?

- A) Elimina completamente la necesidad de pagar por cualquier servicio de AWS
- B) Combina el uso de todas las cuentas miembro para calcular descuentos por volumen de forma agregada, y genera una sola factura consolidada para toda la organización
- C) Solo funciona con instancias Spot
- D) Requiere que todas las cuentas usen exactamente los mismos servicios

**Pregunta 9.** ¿Cuál de las siguientes es una estrategia típica de optimización de costos recomendada por AWS?

- A) Mantener siempre instancias On-Demand del mayor tamaño posible 'por si acaso'
- B) Redimensionar (rightsizing) instancias subutilizadas, eliminar recursos no utilizados, y usar el modelo de precios adecuado (Reserved/Savings Plans para cargas constantes, Spot para tolerantes a interrupciones)
- C) Deshabilitar todas las alarmas de CloudWatch para reducir costos de monitoreo
- D) Usar siempre la Región más cara disponible

**Pregunta 10.** ¿Qué herramienta de AWS ofrece recomendaciones específicas de optimización de costos, como identificar instancias EC2 subutilizadas que podrían reducirse de tamaño?

- A) AWS Budgets exclusivamente
- B) AWS Trusted Advisor, en su categoría de optimización de costos
- C) AWS Organizations exclusivamente
- D) Amazon CloudFront

**Pregunta 11.** Una startup con presupuesto ajustado quiere asegurarse de recibir una notificación automática si su gasto mensual proyectado en AWS va a superar los $500, antes de que eso ocurra. ¿Qué servicio configurarían?

- A) AWS Cost Explorer exclusivamente, sin ninguna alerta automática
- B) AWS Budgets, creando un presupuesto de costo con una alerta basada en el gasto proyectado (forecasted)
- C) AWS Organizations
- D) Reserved Instances

**Pregunta 12.** ¿Cuál de las siguientes cargas de trabajo es la MENOS adecuada para ejecutarse sobre instancias Spot?

- A) Procesamiento de renderizado de video que puede pausarse y reanudarse sin problema
- B) Un trabajo de análisis de big data tolerante a interrupciones con checkpoints frecuentes
- C) Una base de datos de producción crítica que no puede tolerar ninguna interrupción inesperada
- D) Pruebas de carga (load testing) de corta duración

**Pregunta 13.** ¿Qué diferencia principal existe entre Reserved Instances y Savings Plans en cuanto a la flexibilidad del compromiso?

- A) Son exactamente lo mismo con distinto nombre
- B) Reserved Instances comprometen un tipo de instancia específico en una Región específica; Savings Plans comprometen un monto de gasto por hora, aplicable de forma más flexible a distintos tipos de instancia, Región (en el caso de Compute Savings Plans) o incluso servicio de cómputo
- C) Savings Plans solo pueden usarse con Amazon RDS
- D) Reserved Instances no ofrecen ningún descuento frente a On-Demand

**Pregunta 14.** Una empresa multinacional con 20 cuentas de AWS distintas (una por país/división) quiere simplificar la gestión de la facturación y aplicar restricciones de seguridad comunes (como prohibir el uso de ciertas Regiones) a todas las cuentas desde un punto central. ¿Qué servicio de AWS resuelve ambas necesidades?

- A) AWS Budgets exclusivamente
- B) AWS Organizations, con facturación consolidada y Service Control Policies (SCPs)
- C) AWS Cost Explorer exclusivamente
- D) Reserved Instances

**Pregunta 15.** ¿Qué recurso de AWS es completamente gratuito de crear, sin importar cuántos se creen, aunque las acciones que realiza SÍ puedan generar costos en otros servicios?

- A) Instancias EC2
- B) Usuarios, grupos, roles y policies de IAM
- C) Volúmenes EBS
- D) Bases de datos RDS

**Pregunta 16.** ¿Qué elemento del modelo de precios de AWS suele sorprender más a los principiantes al recibir su primera factura, por no haberlo considerado explícitamente al diseñar su arquitectura?

- A) El costo de crear usuarios IAM
- B) El costo de la transferencia de datos SALIENTE (data transfer OUT) hacia internet, que a menudo no es tan visible como el costo de cómputo o almacenamiento
- C) El costo del usuario root
- D) El costo de las Availability Zones adicionales

**Pregunta 17.** ¿Qué acción de optimización de costos describe mejor el concepto de 'rightsizing'?

- A) Aumentar siempre el tamaño de todas las instancias para tener margen de sobra
- B) Ajustar el tipo y tamaño de una instancia (u otro recurso) para que coincida con la demanda real observada, ni sobredimensionado ni subdimensionado
- C) Eliminar completamente todas las instancias de la cuenta
- D) Cambiar únicamente de Región sin analizar el uso real

**Pregunta 18.** Una empresa quiere combinar lo mejor de dos mundos: un compromiso base de Savings Plans para cubrir su carga de trabajo constante y predecible, y complementarlo con instancias Spot para picos de procesamiento no crítico y tolerante a interrupciones. ¿Qué principio de optimización de costos ilustra esta combinación?

- A) Usar un único modelo de precios para toda la infraestructura sin excepción
- B) Adaptar el modelo de precios de cómputo a las características específicas de cada carga de trabajo dentro de la misma cuenta, en vez de aplicar un enfoque único para todo
- C) Evitar por completo el uso de instancias Spot en cualquier escenario
- D) Usar exclusivamente instancias On-Demand para simplificar la facturación

**Pregunta 19.** ¿Qué es AWS Free Tier y qué tipos de ofertas incluye?

- A) Un descuento permanente del 50% en todos los servicios de AWS
- B) Un conjunto de ofertas gratuitas para nuevos usuarios, que incluye ofertas de 12 meses gratis (con límites de uso), ofertas 'siempre gratis' dentro de ciertos límites, y pruebas gratuitas de corta duración para servicios específicos
- C) Un servicio exclusivo de soporte técnico gratuito ilimitado
- D) Solo aplica a Amazon S3

**Pregunta 20.** ¿Qué reporte o herramienta usarías para responder a la pregunta '¿cuánto gastamos exactamente en el servicio de EC2 durante el último trimestre, desglosado por equipo usando etiquetas (tags)'?

- A) AWS Organizations exclusivamente, sin ninguna otra herramienta
- B) AWS Cost Explorer, filtrando por servicio (EC2) y agrupando por la etiqueta (tag) correspondiente
- C) AWS Shield
- D) Amazon GuardDuty
