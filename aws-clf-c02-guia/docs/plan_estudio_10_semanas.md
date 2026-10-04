# Plan de Estudio — AWS Certified Cloud Practitioner (CLF-C02)

*Duración: 10 semanas · Dedicación estimada: 8-15 horas por semana · Objetivo: aprobar con más de 90% y dejar bases para Solutions Architect Associate.*

| Semana | Temas principales | Horas | Laboratorios | Lecturas | Videos | Práctica | Simuladores | Objetivo semanal |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Semana 1 | Cloud Computing: historia, IaaS/PaaS/SaaS/FaaS Modelos de despliegue, elasticidad, HA, DR | 8-10h | Crear cuenta AWS Free Tier + activar MFA root | AWS Overview whitepaper Cloud Practitioner Essentials (Skill Builder) | AWS Skill Builder: Cloud Practitioner Essentials Andrew Brown (freeCodeCamp) - módulo 1 | Glosario propio de 20 términos | — | Entender qué es la nube y por qué existe AWS |
| Semana 2 | Infraestructura global AWS: Regiones, AZ, Edge Locations Consola, CLI, SDK, IAM básico | 8-10h | Instalar y configurar AWS CLI Crear usuario IAM con MFA, dejar de usar root | AWS Global Infrastructure page IAM Best Practices whitepaper | Stephane Maarek - sección IAM AWS re:Invent - Global Infrastructure | Crear 2 policies IAM personalizadas | — | Manejar la consola y entender el modelo de identidad |
| Semana 3 | EC2 completo: AMI, tipos de instancia, Security Groups Auto Scaling y Elastic Load Balancer | 10-12h | Lanzar EC2 Free Tier Configurar Security Group Crear Auto Scaling Group + ALB | EC2 User Guide (secciones clave) | Adrian Cantrill - EC2 deep dive Digital Cloud Training - Auto Scaling | Comparar tipos de instancia t3 vs m5 vs c5 | 10 preguntas EC2 (propias) | Desplegar y escalar una instancia EC2 con criterio |
| Semana 4 | Lambda, ECS, EKS, Fargate Cómputo serverless vs contenedores vs VM | 8-10h | Crear función Lambda simple (Hello World) Invocar Lambda desde consola | Lambda Developer Guide - introducción | Neal Davis - Serverless en AWS AWS Skill Builder - Containers | Tabla comparativa EC2 vs Lambda vs Fargate | 10 preguntas cómputo | Elegir el servicio de cómputo correcto según el caso |
| Semana 5 | S3 completo: versionado, lifecycle, clases de almacenamiento EBS, EFS, FSx, Storage Gateway | 10-12h | Crear bucket S3, subir objetos, activar versionado Configurar regla de lifecycle a Glacier Adjuntar volumen EBS a EC2 | S3 User Guide - Storage Classes | Stephane Maarek - S3 deep dive | Calcular costo de 100GB en cada clase S3 con Pricing Calculator | 10 preguntas almacenamiento | Elegir la clase de almacenamiento óptima por costo/acceso |
| Semana 6 | RDS, Aurora, DynamoDB ElastiCache, Redshift, Neptune, DocumentDB | 8-10h | Lanzar RDS Free Tier (MySQL) Crear tabla DynamoDB y hacer consultas simples | RDS User Guide - Multi-AZ DynamoDB - conceptos básicos | Digital Cloud Training - Databases | Comparativa RDS vs DynamoDB en tabla propia | 10 preguntas bases de datos | Distinguir bases relacionales de NoSQL y sus casos de uso |
| Semana 7 | VPC completo: subnets, route tables, IGW, NAT, VPN, Direct Connect Route53, CloudFront, Security Groups vs NACL | 10-12h | Crear VPC con subnet pública y privada Configurar Internet Gateway y NAT Gateway Crear distribución CloudFront básica | VPC User Guide - conceptos | Adrian Cantrill - Networking Andrew Brown - VPC desde cero | Dibujar tu propia VPC en draw.io o Mermaid | 10 preguntas networking | Diseñar una VPC básica de dos capas |
| Semana 8 | Seguridad: Shared Responsibility, KMS, Secrets Manager, WAF, Shield, GuardDuty CloudTrail, Config, Observabilidad (CloudWatch, X-Ray) | 8-10h | Crear alarma CloudWatch Activar CloudTrail Revisar hallazgos de Trusted Advisor | Shared Responsibility Model (AWS) Security Best Practices whitepaper | AWS Skill Builder - Security Fundamentals | Mapear qué es responsabilidad de AWS vs del cliente (tabla) | 10 preguntas seguridad | Entender el modelo de responsabilidad compartida a fondo |
| Semana 9 | Integración: SQS, SNS, EventBridge, Step Functions, API Gateway Costos: Pricing, Billing, Cost Explorer, Savings Plans, RI, Spot | 10-12h | Crear cola SQS y tópico SNS Explorar AWS Pricing Calculator con un caso real | Pricing whitepaper SQS vs SNS - documentación oficial | Stephane Maarek - Integration services | Simular una arquitectura desacoplada con SQS+Lambda | 10 preguntas integración + costos | Optimizar costos y desacoplar arquitecturas con mensajería |
| Semana 10 | Well-Architected Framework (6 pilares) CloudFormation, Organizations, Control Tower, Migration Repaso general + simulacros | 12-15h | Desplegar un stack simple con CloudFormation Eliminar TODOS los recursos creados en el curso | Well-Architected Framework whitepaper (los 6 pilares) | AWS re:Invent - Well-Architected | Repasar tarjetas de memoria (flashcards) de todo el temario | 2 exámenes completos de 65 preguntas + repaso de fallos | Llegar al examen real con >90% en simulacros |

## Cómo usar este plan

- Cada semana corresponde aproximadamente a una o dos Partes del temario completo (ver documento de cada capítulo).
- Los laboratorios usan siempre AWS Free Tier. Al final de cada semana, elimina los recursos creados para evitar cargos.
- Las 'Horas' son estimadas para alguien con trabajo/estudios paralelos; si dedicas el día completo puedes comprimir el plan a 5-6 semanas.
- Los simuladores semanales son sets de 10 preguntas propias (incluidas al final de cada capítulo). Los simulacros de 65 preguntas se hacen en la semana 10 y en la guía final.
- Si en algún simulador semanal no superas el 80%, repite la teoría de esa semana antes de avanzar — no acumules huecos.

## Semáforo de progreso sugerido

Lleva un registro simple: 🔴 no visto · 🟡 visto pero inseguro · 🟢 dominado y explicable en voz alta sin notas. El objetivo antes del examen es tener el temario completo en verde.

## Próximo documento

El primer capítulo de contenido (Parte 1 — Introducción al Cloud Computing) se entrega como documento independiente, siguiendo la estructura de 9 secciones definida: objetivos, teoría, ejemplos, diagramas, laboratorios, errores comunes, comparaciones, 20 preguntas tipo examen y resumen.
