# Guía AWS Certified Cloud Practitioner (CLF-C02)

Guía de estudio completa en español para la certificación **AWS Certified Cloud Practitioner (CLF-C02)**: temario de 13 partes, plan de estudio de 10 semanas, estrategias de examen y 5 simulacros de 65 preguntas.

## Contenido

- **Temario completo (13 partes)** — cada una con objetivos, teoría, ejemplos, diagramas (Mermaid), laboratorios prácticos en AWS Free Tier, errores comunes, comparaciones de servicios, 20 preguntas tipo examen explicadas, resumen y recursos externos.
- **Plan de estudio de 10 semanas** — temas, horas estimadas, laboratorios, lecturas, videos y objetivos por semana.
- **Estrategias para aprobar el examen** — cómo piensa AWS al diseñar preguntas, palabras clave, técnica de eliminación, gestión del tiempo, qué memorizar vs qué comprender.
- **5 simulacros completos** (65 preguntas cada uno, 325 en total) — mismo nivel de dificultad y distribución de dominios que el examen oficial, con respuesta correcta, explicación y referencia al capítulo correspondiente.
- **Banco de preguntas sin respuestas** — las preguntas de cada parte del temario, sin marcar la correcta, para autoevaluación real antes de consultar las explicaciones.

## Estructura

```
.
├── README.md
├── docs/                              # Temario, en Markdown
│   ├── plan_estudio_10_semanas.md
│   ├── parte1_cloud_computing.md
│   ├── parte2_introduccion_aws.md
│   ├── parte3_iam.md
│   ├── parte4_computo.md
│   ├── parte5_almacenamiento.md
│   ├── parte6_bases_de_datos.md
│   ├── parte7_networking.md
│   ├── parte8_seguridad.md
│   ├── parte9_observabilidad.md
│   ├── parte10_integracion.md
│   ├── parte11_costos.md
│   ├── parte12_well_architected.md
│   ├── parte13_servicios_adicionales.md
│   └── estrategias_examen.md
├── simulacros/                        # 5 exámenes completos, CON respuestas y explicación
│   ├── simulacro_1.md
│   ├── simulacro_2.md
│   ├── simulacro_3.md
│   ├── simulacro_4.md
│   └── simulacro_5.md
├── preguntas/                         # Las mismas preguntas de docs/, SIN respuesta marcada
│   ├── parte1_preguntas.md
│   ├── parte2_preguntas.md
│   ├── parte3_preguntas.md
│   ├── parte4_preguntas.md
│   ├── parte5_preguntas.md
│   ├── parte6_preguntas.md
│   ├── parte7_preguntas.md
│   ├── parte8_preguntas.md
│   ├── parte9_preguntas.md
│   ├── parte10_preguntas.md
│   ├── parte11_preguntas.md
│   ├── parte12_preguntas.md
│   └── parte13_preguntas.md
└── docx/                              # Mismos contenidos en Word
    ├── plan_estudio_10_semanas.docx
    ├── parte1_cloud_computing.docx … parte13_servicios_adicionales.docx
    ├── estrategias_examen.docx
    ├── simulacro_1.docx … simulacro_5.docx
    ├── AWS_CLF-C02_Guia_Completa.docx          # las 20 piezas en un solo .docx
    └── AWS_CLF-C02_Guia_Completa_Bitter.docx   # misma guía, tipografía Bitter
```

## Temario

| # | Parte | Temas |
|---|-------|-------|
| 1 | Cloud Computing | Historia, IaaS/PaaS/SaaS/FaaS, modelos de despliegue, elasticidad, HA, DR |
| 2 | Introducción a AWS | Regiones, AZ, Edge Locations, consola/CLI/SDK/API |
| 3 | IAM | Users, Groups, Roles, Policies, MFA, mínimo privilegio, Identity Center |
| 4 | Servicios de Cómputo | EC2, AMI, Security Groups, Auto Scaling, ELB, Lambda, ECS/EKS/Fargate, Lightsail, Batch |
| 5 | Almacenamiento | S3, versionado, lifecycle, Glacier, EBS, EFS, FSx, Storage Gateway |
| 6 | Bases de Datos | RDS, Aurora, DynamoDB, ElastiCache, Redshift, Neptune, DocumentDB |
| 7 | Networking | VPC, subnets, route tables, IGW, NAT, VPN, Direct Connect, NACL, Route 53, CloudFront |
| 8 | Seguridad | Shared Responsibility, KMS, Secrets Manager, ACM, Shield, WAF, GuardDuty, Inspector, Macie, CloudTrail, Config |
| 9 | Observabilidad | CloudWatch, X-Ray, Health Dashboard, Trusted Advisor |
| 10 | Integración | SQS, SNS, EventBridge, Step Functions, API Gateway |
| 11 | Costos | Pricing, Billing, Cost Explorer, Budgets, Savings Plans, RI, Spot, Organizations |
| 12 | Well-Architected Framework | Los 6 pilares |
| 13 | Servicios Adicionales | CloudFormation, CDK, Control Tower, Backup, Migration Hub, DMS, DataSync, Snow Family, Elastic DR |

## Cómo usar este contenido

1. Sigue `docs/plan_estudio_10_semanas.md` como hoja de ruta semana a semana.
2. Estudia cada parte en `docs/`, incluyendo sus laboratorios prácticos.
3. Al terminar una parte, resuelve sus preguntas desde `preguntas/` (sin respuestas) antes de revisar las explicaciones ya incluidas al final de esa misma parte en `docs/`.
4. Antes del examen real, resuelve los 5 simulacros de `simulacros/` cronometrando 90 minutos cada uno.
5. Repasa `docs/estrategias_examen.md` el día previo al examen.

## Notas

- Las Partes 3 (IAM), 10 (Integración) y 13 (Servicios Adicionales) tienen 19 preguntas en vez de 20 en `preguntas/` y `docs/`.
- Los diagramas de arquitectura están en formato [Mermaid](https://mermaid.live) dentro de bloques de código; se renderizan de forma nativa en GitHub.
- Contenido basado en el blueprint oficial del examen CLF-C02; verifica siempre el [AWS Certified Cloud Practitioner Exam Guide](https://aws.amazon.com/certification/certified-cloud-practitioner/) vigente por si AWS actualiza dominios o pesos.
