# Parte 9 — Observabilidad — Preguntas tipo examen

20 preguntas de opción múltiple, sin respuestas marcadas, para autoevaluación.

**Pregunta 1.** ¿Qué es Amazon CloudWatch?

- A) Un servicio de backup automatizado
- B) Un servicio de monitoreo que recopila métricas, logs y eventos de los recursos de AWS, permitiendo visualizarlos, crear alarmas y automatizar respuestas
- C) Un firewall de aplicaciones web
- D) Un servicio exclusivo de facturación

**Pregunta 2.** ¿Qué es una CloudWatch Alarm y para qué se usa típicamente?

- A) Un tipo de instancia EC2
- B) Un mecanismo que monitorea una métrica y ejecuta una acción automática (como notificar por SNS o disparar Auto Scaling) cuando esa métrica cruza un umbral definido
- C) Un servicio de almacenamiento de logs exclusivamente
- D) Un reporte mensual de facturación

**Pregunta 3.** ¿Qué almacena CloudWatch Logs?

- A) Únicamente métricas numéricas de CPU
- B) Registros de eventos (logs) generados por aplicaciones, servicios de AWS y sistemas operativos, organizados en grupos y flujos de log
- C) Solo información de facturación
- D) Imágenes de máquinas virtuales (AMIs)

**Pregunta 4.** Una aplicación distribuida en microservicios experimenta lentitud intermitente, y el equipo necesita identificar exactamente en qué servicio específico de la cadena de llamadas se origina el retraso. ¿Qué servicio de AWS está diseñado específicamente para este tipo de diagnóstico?

- A) Amazon CloudWatch exclusivamente
- B) AWS X-Ray
- C) AWS Trusted Advisor
- D) AWS Health Dashboard

**Pregunta 5.** ¿Qué es AWS Trusted Advisor?

- A) Una herramienta que analiza tu cuenta de AWS y ofrece recomendaciones personalizadas en categorías como optimización de costos, rendimiento, seguridad, tolerancia a fallos y límites de servicio
- B) Un servicio de soporte técnico exclusivo por chat en vivo
- C) Un tipo de instancia EC2 optimizada
- D) Un servicio de rastreo distribuido de solicitudes

**Pregunta 6.** ¿Qué es el AWS Health Dashboard (anteriormente conocido como Service Health Dashboard / Personal Health Dashboard)?

- A) Un dashboard de métricas de una sola aplicación específica del cliente
- B) Un panel que informa sobre el estado operativo de los servicios de AWS a nivel global, y también sobre eventos que afectan específicamente a los recursos de tu cuenta
- C) Un servicio de facturación detallada
- D) Una herramienta exclusiva de optimización de costos

**Pregunta 7.** ¿Cuál de los siguientes NO es uno de los cinco pilares de recomendaciones que ofrece AWS Trusted Advisor?

- A) Optimización de costos
- B) Rendimiento
- C) Seguridad
- D) Diseño gráfico de interfaces de usuario

**Pregunta 8.** ¿Qué diferencia principal existe entre las métricas 'estándar' de CloudWatch y las 'métricas personalizadas' (custom metrics)?

- A) No hay diferencia, ambas son idénticas en costo y origen
- B) Las métricas estándar son publicadas automáticamente por los servicios de AWS; las métricas personalizadas son publicadas explícitamente por el cliente (por ejemplo, desde el código de su aplicación) usando la API de CloudWatch
- C) Las métricas personalizadas solo pueden verse por soporte de AWS, no por el cliente
- D) Las métricas estándar requieren instalar un agente obligatoriamente

**Pregunta 9.** Un equipo de DevOps quiere que, automáticamente, se envíe una notificación por correo electrónico al equipo de guardia cuando el uso de CPU de una instancia EC2 crítica supere el 90% durante 5 minutos consecutivos. ¿Qué combinación de servicios resuelve esto?

- A) AWS X-Ray exclusivamente
- B) Una CloudWatch Alarm sobre la métrica de CPU, con una acción configurada hacia un tópico de Amazon SNS
- C) AWS Trusted Advisor exclusivamente
- D) AWS Health Dashboard exclusivamente

**Pregunta 10.** ¿Qué nivel de soporte de AWS es necesario para acceder a TODAS las verificaciones de Trusted Advisor, incluidas las de seguridad y límites de servicio de forma completa?

- A) El plan Basic Support (gratuito) ya incluye acceso completo a todas las verificaciones
- B) Los planes Business o Enterprise Support (de pago) desbloquean el conjunto completo de verificaciones; Basic Support solo incluye un subconjunto limitado
- C) Ningún plan de soporte incluye Trusted Advisor
- D) Solo se puede acceder a Trusted Advisor mediante un ticket manual de soporte

**Pregunta 11.** ¿Qué tipo de dato registra AWS X-Ray para cada solicitud que atraviesa una aplicación distribuida?

- A) Solo el costo asociado a la solicitud
- B) Un 'trace' (traza) que muestra el recorrido completo de la solicitud a través de los distintos servicios/componentes, incluyendo tiempos de cada segmento
- C) Únicamente el nombre de usuario de IAM que hizo la solicitud
- D) Solo si la solicitud fue exitosa o fallida, sin ningún otro detalle

**Pregunta 12.** Una empresa quiere revisar de forma proactiva si tiene instancias EC2 subutilizadas que podrían reducirse de tamaño para ahorrar costos, sin tener que analizar manualmente cada instancia. ¿Qué herramienta de AWS le ayudaría directamente con esta recomendación?

- A) AWS X-Ray
- B) AWS Trusted Advisor, en su categoría de optimización de costos
- C) AWS Health Dashboard
- D) Amazon CloudWatch Logs exclusivamente

**Pregunta 13.** ¿Qué te permitiría saber el AWS Health Dashboard que Trusted Advisor NO cubre directamente?

- A) Recomendaciones de optimización de costos
- B) Si un evento operativo específico de AWS (como mantenimiento programado en una AZ, o una degradación de servicio) está afectando o va a afectar a los recursos específicos de TU cuenta
- C) Verificaciones de seguridad de configuración de IAM
- D) Límites de servicio de tu cuenta

**Pregunta 14.** ¿Qué componente de CloudWatch permite crear paneles visuales personalizados combinando múltiples métricas de distintos servicios en una sola vista?

- A) CloudWatch Logs Insights
- B) CloudWatch Dashboards
- C) CloudWatch Alarms
- D) CloudWatch Events exclusivamente

**Pregunta 15.** Un desarrollador quiere consultar y filtrar rápidamente millones de líneas de logs de una función Lambda usando un lenguaje de consulta similar a SQL, sin descargar manualmente los archivos de log. ¿Qué herramienta de CloudWatch le ayudaría?

- A) CloudWatch Alarms
- B) CloudWatch Logs Insights
- C) AWS X-Ray exclusivamente
- D) AWS Trusted Advisor

**Pregunta 16.** ¿Cuál de las siguientes combinaciones describe mejor la relación entre CloudWatch y X-Ray?

- A) Son el mismo servicio con nombres distintos
- B) CloudWatch se enfoca en métricas y logs agregados de infraestructura y aplicaciones; X-Ray se enfoca en el rastreo detallado del recorrido de solicitudes individuales a través de servicios distribuidos
- C) X-Ray reemplaza completamente a CloudWatch en aplicaciones modernas
- D) CloudWatch solo funciona con EC2; X-Ray solo funciona con Lambda

**Pregunta 17.** Una startup en su plan de soporte Basic (gratuito) quiere saber si algún servicio de AWS a nivel global está experimentando una interrupción reportada por AWS en este momento. ¿Dónde debería consultarlo?

- A) AWS Trusted Advisor exclusivamente (requiere plan de pago)
- B) AWS Health Dashboard, en su vista de Service Health (disponible para todos los clientes sin importar el plan de soporte)
- C) AWS X-Ray
- D) Amazon CloudWatch Logs exclusivamente

**Pregunta 18.** ¿Qué acción NO es una acción típica que se puede configurar para que dispare una CloudWatch Alarm?

- A) Enviar una notificación a un tópico de Amazon SNS
- B) Disparar una política de Auto Scaling para añadir o quitar instancias
- C) Detener, terminar, reiniciar o recuperar automáticamente una instancia EC2
- D) Aprobar automáticamente solicitudes de acceso de nuevos usuarios IAM

**Pregunta 19.** Un equipo de arquitectura está revisando si su cuenta de AWS se acerca a algún límite de servicio (por ejemplo, número máximo de VPCs permitidas por Región) antes de que eso bloquee un proyecto de expansión. ¿Qué herramienta consultarían primero?

- A) AWS X-Ray
- B) AWS Trusted Advisor, categoría de límites de servicio (Service Limits)
- C) CloudWatch Logs Insights
- D) AWS Health Dashboard exclusivamente

**Pregunta 20.** ¿Qué diferencia hay entre las métricas de CloudWatch con resolución 'estándar' (1 minuto) y resolución 'de alta frecuencia' (high-resolution, hasta 1 segundo)?

- A) No existe tal diferencia, todas las métricas de CloudWatch usan la misma resolución obligatoriamente
- B) Las métricas de alta resolución permiten detectar cambios más rápidos y granulares en el comportamiento de un recurso, a cambio de mayor costo de almacenamiento de esos puntos de datos adicionales
- C) Las métricas de alta resolución solo están disponibles para Amazon S3
- D) La resolución de las métricas no afecta el costo de CloudWatch
