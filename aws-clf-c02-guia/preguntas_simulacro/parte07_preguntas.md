# Parte 7 — Networking — Preguntas tipo examen

20 preguntas de opción múltiple, sin respuestas marcadas, para autoevaluación.

**Pregunta 1.** ¿Qué es una Amazon VPC (Virtual Private Cloud)?

- A) Un tipo de instancia EC2 optimizada para redes
- B) Una red virtual aislada y lógicamente separada dentro de AWS, donde el cliente controla el direccionamiento IP, subredes, tablas de rutas y configuración de red
- C) Un servicio de DNS
- D) Un firewall físico dedicado

**Pregunta 2.** ¿Cuál es la diferencia principal entre una subred pública y una subred privada dentro de una VPC?

- A) No hay diferencia real entre ambas
- B) Una subred pública tiene una ruta hacia un Internet Gateway, permitiendo comunicación directa con internet; una subred privada no tiene esa ruta directa
- C) Las subredes privadas no pueden contener instancias EC2
- D) Las subredes públicas son siempre más grandes en tamaño de IP

**Pregunta 3.** ¿Qué componente de una VPC permite la comunicación bidireccional entre instancias dentro de una subred pública e internet?

- A) NAT Gateway
- B) Internet Gateway (IGW)
- C) VPN Gateway
- D) Direct Connect

**Pregunta 4.** Una instancia EC2 en una subred privada necesita descargar actualizaciones de software desde internet, pero no debe ser accesible directamente desde internet. ¿Qué componente de red permite esto?

- A) Internet Gateway directamente en la subred privada
- B) NAT Gateway ubicado en una subred pública, con una ruta desde la subred privada hacia él
- C) Un Security Group adicional
- D) Direct Connect

**Pregunta 5.** Una empresa necesita conectar su data center on-premises con su VPC de AWS de forma rápida y económica, aceptando cierta variabilidad en la latencia, usando internet como medio de transporte cifrado. ¿Qué servicio es el más adecuado?

- A) AWS Direct Connect
- B) Site-to-Site VPN
- C) AWS Snowball
- D) Amazon CloudFront

**Pregunta 6.** Una empresa requiere una conexión de red dedicada y privada entre su data center y AWS, con ancho de banda consistente y menor latencia que una conexión a través de internet público, para cargas de trabajo críticas de alto volumen. ¿Qué servicio es el más adecuado?

- A) Site-to-Site VPN exclusivamente
- B) AWS Direct Connect
- C) Amazon Route 53
- D) AWS WAF

**Pregunta 7.** ¿Cuál es la diferencia principal entre un Security Group y una Network ACL (NACL) en cuanto al estado de las conexiones?

- A) Ambos son stateful
- B) El Security Group es stateful (el tráfico de respuesta se permite automáticamente); la NACL es stateless (se deben definir reglas explícitas para el tráfico entrante Y saliente por separado)
- C) Ambos son stateless
- D) La NACL es stateful y el Security Group es stateless

**Pregunta 8.** ¿A qué nivel de la arquitectura de red opera una Network ACL, a diferencia de un Security Group?

- A) A nivel de instancia individual, igual que el Security Group
- B) A nivel de subred, controlando el tráfico que entra y sale de toda la subred
- C) A nivel de Región completa
- D) A nivel de cuenta de AWS completa

**Pregunta 9.** ¿Qué es Amazon Route 53?

- A) Un servicio de balanceo de carga exclusivamente
- B) Un servicio de DNS (Domain Name System) altamente disponible y escalable, que también ofrece registro de dominios y verificación de salud
- C) Un tipo de instancia EC2
- D) Un firewall de aplicaciones web

**Pregunta 10.** ¿Qué es Amazon CloudFront y qué problema resuelve principalmente?

- A) Un servicio de bases de datos distribuido
- B) Una red de entrega de contenido (CDN) que cachea contenido en Edge Locations cercanas a los usuarios finales, reduciendo la latencia de entrega
- C) Un servicio de backup automatizado
- D) Un tipo de VPN

**Pregunta 11.** Una arquitectura de tres capas (three-tier) típica coloca los servidores web en subredes públicas y la base de datos en subredes privadas. ¿Por qué se recomienda esta separación?

- A) Es simplemente una convención sin ningún beneficio real de seguridad
- B) Reduce la superficie de ataque: la base de datos, que contiene los datos más sensibles, no es directamente alcanzable desde internet, solo desde la capa de aplicación autorizada
- C) Las subredes privadas son más baratas que las públicas
- D) Es un requisito técnico obligatorio de AWS que no se puede evitar

**Pregunta 12.** ¿Qué elemento de una VPC define hacia dónde se dirige el tráfico de red según su IP de destino (por ejemplo, hacia el Internet Gateway, hacia un NAT Gateway, o dentro de la misma VPC)?

- A) Security Group
- B) Route Table (tabla de rutas)
- C) Network ACL
- D) AMI

**Pregunta 13.** Un usuario en Japón y un usuario en Brasil acceden al mismo sitio web servido a través de Amazon CloudFront. ¿Desde dónde recibe cada uno el contenido cacheado, en la mayoría de los casos?

- A) Ambos reciben el contenido siempre desde el mismo servidor de origen en Estados Unidos
- B) Cada uno recibe el contenido desde la Edge Location de CloudFront geográficamente más cercana a su ubicación
- C) Solo el usuario de Brasil recibe contenido cacheado
- D) CloudFront no distingue la ubicación geográfica de los usuarios

**Pregunta 14.** ¿Qué combinación de conceptos permite que una subred se considere 'privada' en una arquitectura estándar de AWS?

- A) Tener una ruta directa hacia un Internet Gateway
- B) NO tener una ruta directa hacia un Internet Gateway en su tabla de rutas (aunque puede tener una ruta hacia un NAT Gateway para tráfico saliente)
- C) Estar ubicada fuera de cualquier Availability Zone
- D) Tener un Security Group vacío

**Pregunta 15.** ¿Cuál de las siguientes afirmaciones sobre las Network ACL es correcta respecto al orden de evaluación de sus reglas?

- A) Las reglas de NACL se evalúan en orden numérico (de menor a mayor) y se aplica la primera regla que coincida
- B) Las reglas de NACL se evalúan en orden alfabético por nombre
- C) Solo se evalúa la última regla de la lista
- D) El orden de las reglas no importa en una NACL

**Pregunta 16.** Una empresa gubernamental necesita conectividad privada, dedicada y de alto ancho de banda entre su centro de datos y AWS, sin pasar por internet público, para transferir grandes volúmenes de datos sensibles de forma consistente todos los días. ¿Qué opción es la más adecuada a largo plazo?

- A) Site-to-Site VPN exclusivamente, por ser más simple de configurar
- B) AWS Direct Connect, por ofrecer una conexión física dedicada con mayor consistencia de ancho de banda y menor latencia
- C) Amazon CloudFront
- D) AWS Snowball exclusivamente

**Pregunta 17.** ¿Qué servicio de AWS traduciría un nombre de dominio como 'www.miempresa.com' a la dirección IP del Load Balancer correspondiente?

- A) Amazon CloudFront
- B) Amazon Route 53
- C) AWS Direct Connect
- D) Amazon VPC

**Pregunta 18.** ¿Qué combinación de Security Group y Network ACL representa el enfoque de 'defensa en profundidad' recomendado por AWS para proteger una subred con instancias EC2?

- A) Usar solo Security Groups y dejar la NACL en su configuración por defecto (permitir todo)
- B) Usar Security Groups restrictivos a nivel de instancia Y una NACL adicional a nivel de subred como capa de seguridad complementaria
- C) Usar solo NACL y eliminar todos los Security Groups
- D) No usar ninguno de los dos, confiando solo en IAM

**Pregunta 19.** Una aplicación de video bajo demanda quiere reducir el costo de transferencia de datos y la latencia al servir millones de reproducciones de video a usuarios en todo el mundo desde un único bucket S3 de origen. ¿Qué servicio deberían colocar delante del bucket S3?

- A) AWS Direct Connect
- B) Amazon CloudFront como CDN delante del bucket S3
- C) AWS Site-to-Site VPN
- D) Amazon Route 53 exclusivamente sin CDN

**Pregunta 20.** ¿Qué elemento de red permitiría que una instancia en una subred privada, sin IP pública, descargue un parche de seguridad desde internet, sin que ningún host externo pueda iniciar una conexión hacia esa instancia?

- A) Internet Gateway conectado directamente a la subred privada
- B) Un NAT Gateway en una subred pública, referenciado en la tabla de rutas de la subred privada
- C) Una Network ACL con todas las reglas en 'Deny'
- D) Ninguna combinación permite esto; las subredes privadas nunca pueden acceder a internet
