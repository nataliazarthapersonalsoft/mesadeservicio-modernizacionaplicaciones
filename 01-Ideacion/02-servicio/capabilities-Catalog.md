# Catálogo de Capacidades — Support System Operator

Fuente: `LibroCapabilities.xlsx` (6 hojas). Documento generado como referencia consolidada de la arquitectura de agentes para el rol de Support System Operator.

## Contenido

1. [Capacidades transversales](#1-capacidades-transversales)
2. [Canales de entrada](#2-canales-de-entrada-input-channels)
3. [Catálogo de agentes](#3-catálogo-de-agentes)
4. [Capa de herramientas (Tools — MCP / APIs)](#4-capa-de-herramientas-tools--mcp--apis)
5. [Catálogo de runbooks](#5-catálogo-de-runbooks)
6. [Guardrails y gobierno](#6-guardrails-y-gobierno)

---

## Escala de prioridad

Todas las tablas de este documento usan una escala de **5 niveles**:

| Nivel | Criterio |
|---|---|
| 🔴 **Alta** | Bloqueante o de valor central para el caso de uso; debe estar en la primera fase / MVP. |
| 🟠 **Media-Alta** | Impacto claro y relevante, pero no bloqueante; buena candidata justo después del MVP. |
| 🟡 **Media** | Mejora relevante de cobertura o eficiencia; fase 2. |
| 🟤 **Media-Baja** | Deseable, impacto acotado o de menor frecuencia de uso; fase 3 / bajo demanda. |
| ⚪ **Baja** | Nice-to-have, casos de borde, nicho o backlog sin fecha comprometida. |

---

## 1. Capacidades transversales

*Vistas y controles de operación de extremo a extremo sobre la plataforma de agentes*

| ID | Capacidad | Descripción | Elementos / Vistas clave | Fuente de datos | Prioridad (propuesta) |
|---|---|---|---|---|---|
| CT-01 | Dashboard de tickets | Visión consolidada del estado de todos los tickets originados en los distintos canales de entrada. | Volumen por estado (abiertos, en curso, resueltos)<br>Filtros por agente, servicio y periodo | ITSM, Ticket History | Media-Alta |
| CT-02 | Procesos en ejecución | Monitoreo en tiempo real de los agentes y runbooks que se están ejecutando en la plataforma. | Procesos activos y su paso actual<br>Agente responsable y runbook en curso<br>Duración, progreso y estado (ok / en espera / error)<br>Reintentos y errores en ejecución<br>Acción para pausar, reanudar o cancelar | Orquestador, Runbooks, Monitoring | Alta |
| CT-03 | Pendientes por aprobación | Cola de acciones que requieren validación humana (HITL) antes de que el agente actúe. | Solicitudes pendientes con contexto y acción propuesta<br>Aprobador o grupo asignado y nivel de riesgo<br>Antigüedad en cola y SLA de aprobación<br>Aprobar / rechazar / devolver con comentario<br>Registro de la decisión para auditoría | Guardrails / HITL, Orquestador | Alta |
| CT-04 | Métricas y KPIs | Indicadores de desempeño operativo de la solución de agentes. | Tasa de automatización y resolución sin intervención<br>Tiempo ahorrado y tickets desviados | ITSM, Monitoring, Ticket History | Media |
| CT-05 | Auditoría y trazabilidad | Registro completo de qué hizo cada agente, cuándo y con qué permisos, para gobierno y cumplimiento. | Bitácora de acciones por agente y por ticket<br>Trazabilidad de decisiones y aprobaciones (HITL)<br>Uso de herramientas y accesos (least privilege)<br>Enmascaramiento de PII y controles de entrada<br>Exportación de evidencia para auditoría | Guardrails / Governance, Database | Alta |
| CT-06 | SLA y alertas en riesgo | Vigilancia de tickets y procesos próximos a incumplir sus acuerdos de nivel de servicio. | Tickets próximos a vencer SLA<br>Procesos bloqueados o con reintentos<br>Notificaciones a responsables | Monitoring, ITSM, Orquestador | Media-Alta |
| CT-07 | FinOps — Costos por ejecución | Visibilidad y control del costo de operar los agentes, con costeo por ejecución, por ticket y por canal para optimizar el gasto. | Costo por ejecución, por ticket y por caso resuelto<br>Desglose por consumo de LLM/tokens, herramientas y APIs<br>Costo por agente, canal y tipo de proceso<br>Presupuestos, umbrales y alertas de sobrecosto<br>Costo vs. ahorro (ROI) y tendencia mensual | Orquestador, Billing / Cloud Cost, LLM usage | Media-Baja |
| CT-08 | Desktop Agent | Agente que opera aplicaciones de escritorio y sistemas legados sin API, ejecutando acciones en la interfaz como lo haría un usuario. | Automatización de apps de escritorio y sistemas legados (RPA)<br>Flujos guiados por interfaz (clics, formularios, extracción de pantalla)<br>Captura de evidencia de cada acción para auditoría<br>Ejecución supervisada con aprobación (HITL) para acciones sensibles | Orquestador, Runbooks, Desktop / RPA runtime | Baja |



---

## 2. Canales de entrada (Input Channels)

*Capacidad de la arquitectura de integración basada en agentes — punto de ingesta de solicitudes y eventos. Cada conector se implementa por separado, por lo que se lista de forma individual.*

| ID | Canal | Conector | Descripción del canal | Capacidades a integrar | Prioridad (propuesta) | Status |
|---|---|---|---|---|---|---|
| CN-MAIL-1 | Correo electrónico (Mail) | Microsoft Graph | Buzones compartidos donde usuarios y sistemas envían solicitudes e incidencias por correo. | Ingesta de buzones (IMAP/Graph/Gmail) y lectura de hilos<br>Parsing de asunto, cuerpo y firma; extracción de adjuntos (PDF, Excel)<br>Verificación del remitente y anti-spoofing (SPF/DKIM)<br>Creación automática de tickets y respuesta/acuse | Baja | — |
| CN-MAIL-2 | Correo electrónico (Mail) | Exchange / IMAP | Buzones compartidos donde usuarios y sistemas envían solicitudes e incidencias por correo. | Ingesta de buzones (IMAP/Graph/Gmail) y lectura de hilos<br>Parsing de asunto, cuerpo y firma; extracción de adjuntos (PDF, Excel)<br>Verificación del remitente y anti-spoofing (SPF/DKIM)<br>Creación automática de tickets y respuesta/acuse | Baja | — |
| CN-MAIL-3 | Correo electrónico (Mail) | Gmail API | Buzones compartidos donde usuarios y sistemas envían solicitudes e incidencias por correo. | Ingesta de buzones (IMAP/Graph/Gmail) y lectura de hilos<br>Parsing de asunto, cuerpo y firma; extracción de adjuntos (PDF, Excel)<br>Verificación del remitente y anti-spoofing (SPF/DKIM)<br>Creación automática de tickets y respuesta/acuse | Baja | — |
| CN-MAIL-4 | Correo electrónico (Mail) | SMTP | Buzones compartidos donde usuarios y sistemas envían solicitudes e incidencias por correo. | Ingesta de buzones (IMAP/Graph/Gmail) y lectura de hilos<br>Parsing de asunto, cuerpo y firma; extracción de adjuntos (PDF, Excel)<br>Verificación del remitente y anti-spoofing (SPF/DKIM)<br>Creación automática de tickets y respuesta/acuse | Baja | — |
| CN-ITSM-1 | ITSM | Zendesk API | Plataforma de gestión de servicios (p. ej. Zendesk / ServiceNow / Jira SM) que origina tickets. | Webhooks de creación y actualización de tickets<br>Sincronización bidireccional de estado, prioridad y SLA<br>Lectura de colas, categorías y asignaciones<br>Publicación de comentarios, notas internas y resolución<br>Adjuntar artículos de conocimiento y evidencias | Alta | — |
| CN-ITSM-2 | ITSM | ServiceNow REST | Plataforma de gestión de servicios (p. ej. Zendesk / ServiceNow / Jira SM) que origina tickets. | Webhooks de creación y actualización de tickets<br>Sincronización bidireccional de estado, prioridad y SLA<br>Lectura de colas, categorías y asignaciones<br>Publicación de comentarios, notas internas y resolución<br>Adjuntar artículos de conocimiento y evidencias | Media | — |
| CN-ITSM-3 | ITSM | Jira SM | Plataforma de gestión de servicios (p. ej. Zendesk / ServiceNow / Jira SM) que origina tickets. | Webhooks de creación y actualización de tickets<br>Sincronización bidireccional de estado, prioridad y SLA<br>Lectura de colas, categorías y asignaciones<br>Publicación de comentarios, notas internas y resolución<br>Adjuntar artículos de conocimiento y evidencias | Media-Baja | — |
| CN-ITSM-4 | ITSM | Azure DevOps Issues | Plataforma de gestión de servicios (p. ej. Zendesk / ServiceNow / Jira SM) que origina tickets. | Webhooks de creación y actualización de tickets<br>Sincronización bidireccional de estado, prioridad y SLA<br>Lectura de colas, categorías y asignaciones<br>Publicación de comentarios, notas internas y resolución<br>Adjuntar artículos de conocimiento y evidencias | Media | — |
| CN-ITSM-5 | ITSM | BMC Helix / Remedy | Plataforma de gestión de servicios (p. ej. Zendesk / ServiceNow / Jira SM) que origina tickets. | Webhooks de creación y actualización de tickets<br>Sincronización bidireccional de estado, prioridad y SLA<br>Lectura de colas, categorías y asignaciones<br>Publicación de comentarios, notas internas y resolución<br>Adjuntar artículos de conocimiento y evidencias | Media-Alta | — |
| CN-ITSM-6 | ITSM | GitHub Issues | Plataforma de gestión de servicios (p. ej. Zendesk / ServiceNow / Jira SM) que origina tickets. | Webhooks de creación y actualización de tickets<br>Sincronización bidireccional de estado, prioridad y SLA<br>Lectura de colas, categorías y asignaciones<br>Publicación de comentarios, notas internas y resolución<br>Adjuntar artículos de conocimiento y evidencias | Media-Baja | — |
| CN-MON-1 | Monitoreo y Observabilidad (Mon&Obs) | Prometheus / Alertmanager | Alertas y eventos de salud del sistema generados por herramientas de monitoreo. | Ingesta de alertas y métricas (Prometheus, Grafana, Datadog)<br>Umbrales y disparadores automáticos hacia el orquestador<br>Apertura automática de incidentes ante alertas críticas | Baja | — |
| CN-MON-2 | Monitoreo y Observabilidad (Mon&Obs) | Grafana | Alertas y eventos de salud del sistema generados por herramientas de monitoreo. | Ingesta de alertas y métricas (Prometheus, Grafana, Datadog)<br>Umbrales y disparadores automáticos hacia el orquestador<br>Apertura automática de incidentes ante alertas críticas | Media-Baja | — |
| CN-MON-3 | Monitoreo y Observabilidad (Mon&Obs) | Datadog | Alertas y eventos de salud del sistema generados por herramientas de monitoreo. | Ingesta de alertas y métricas (Prometheus, Grafana, Datadog)<br>Umbrales y disparadores automáticos hacia el orquestador<br>Apertura automática de incidentes ante alertas críticas | Media-Baja | — |
| CN-MON-4 | Monitoreo y Observabilidad (Mon&Obs) | Azure Monitor | Alertas y eventos de salud del sistema generados por herramientas de monitoreo. | Ingesta de alertas y métricas (Prometheus, Grafana, Datadog)<br>Umbrales y disparadores automáticos hacia el orquestador<br>Apertura automática de incidentes ante alertas críticas | Media | — |
| CN-MON-5 | Monitoreo y Observabilidad (Mon&Obs) | CloudWatch | Alertas y eventos de salud del sistema generados por herramientas de monitoreo. | Ingesta de alertas y métricas (Prometheus, Grafana, Datadog)<br>Umbrales y disparadores automáticos hacia el orquestador<br>Apertura automática de incidentes ante alertas críticas | Media | — |
| CN-CHAT-1 | Mensajería / ChatOps | Slack API | Canales conversacionales donde usuarios y equipos solicitan soporte o interactúan con los agentes en tiempo real. | Bots y slash-commands para crear y consultar tickets<br>Escucha de mensajes y menciones en canales/grupos<br>Respuestas interactivas (botones, formularios, hilos)<br>Notificaciones y aprobaciones (HITL) desde el chat<br>Autenticación de usuario y mapeo a identidad corporativa | Media-Alta | — |
| CN-CHAT-2 | Mensajería / ChatOps | Microsoft Teams (Bot Framework) | Canales conversacionales donde usuarios y equipos solicitan soporte o interactúan con los agentes en tiempo real. | Bots y slash-commands para crear y consultar tickets<br>Escucha de mensajes y menciones en canales/grupos<br>Respuestas interactivas (botones, formularios, hilos)<br>Notificaciones y aprobaciones (HITL) desde el chat<br>Autenticación de usuario y mapeo a identidad corporativa | Alta | — |
| CN-CHAT-3 | Mensajería / ChatOps | Telegram Bot API | Canales conversacionales donde usuarios y equipos solicitan soporte o interactúan con los agentes en tiempo real. | Bots y slash-commands para crear y consultar tickets<br>Escucha de mensajes y menciones en canales/grupos<br>Respuestas interactivas (botones, formularios, hilos)<br>Notificaciones y aprobaciones (HITL) desde el chat<br>Autenticación de usuario y mapeo a identidad corporativa | Media | — |

---

## 3. Catálogo de agentes

*Procedimientos automatizados que los agentes ejecutan ante eventos de los canales de entrada, usando las herramientas de la plataforma*

| ID | Agentes | Categoría | Disparador (Canal) | Objetivo y pasos clave | Herramientas (Tools) | HITL (Aprobación) | Prioridad | Nivel de automatización | Dueño / Equipo |
|---|---|---|---|---|---|---|---|---|---|
| AG-01 | Triage y clasificación de tickets | Gestión de tickets | Mail / ITSM / ChatOps | Clasificar, priorizar y enrutar automáticamente las solicitudes entrantes.<br>Leer ticket y adjuntos<br>Extraer intención y entidades<br>Determinar tipo (incidente vs. solicitud de servicio)<br>Asignar categoría y prioridad<br>Enrutar a cola / agente | Database, PDF, Excel | No | Alta | Total | Service Desk |
| AG-02 | Revisar casos duplicados | Gestión de tickets | ITSM / Mail | Detectar y agrupar tickets duplicados o relacionados para evitar trabajo redundante. | Database, ITSM | No | Media | Total | Service Desk |
| AG-03 | Revisar información faltante del caso | Gestión de tickets | Mail / ITSM | Verificar si el ticket tiene toda la información necesaria y solicitar lo que falte. | PDF, Database | Condicional | Media | Semi | Service Desk |
| AG-04 | Sugerir qué casos atender | Gestión de tickets | ITSM / Monitoreo y Obs. | Priorizar la cola y recomendar los próximos casos a atender según impacto y SLA. | Database, Monitoring | No | Media-Baja | Semi | Service Desk |
| AG-05 | Asignar al responsable correcto | Gestión de tickets | ITSM | Enrutar cada caso a la persona o equipo adecuado según categoría y carga. | Database, ITSM | No | Media-Alta | Total | Service Desk |
| AG-06 | Escalamiento por SLA en riesgo | Gestión de tickets | ITSM / Monitoreo y Obs. | Escalar tickets próximos a incumplir su SLA.<br>Detectar SLA en riesgo<br>Notificar al responsable<br>Reasignar o repriorizar<br>Registrar la acción | Database, Monitoring | No | Alta | Total | Service Desk |
| AG-07 | Informar avances al cliente | Comunicación | Mail / ChatOps | Mantener al cliente informado del progreso del caso con actualizaciones automáticas.<br>Solicitar confirmación de cierre al usuario | Mail, ChatOps | Condicional | Media | Semi | Service Desk |
| AG-08 | Relacionar incidentes similares | Diagnóstico | Monitoreo y Obs. / ITSM | Correlacionar el incidente con casos históricos similares para acelerar el análisis. | Database, Monitoring | No | Media | Semi | SRE |
| AG-09 | Sugerir siguientes pasos | Diagnóstico | ITSM / ChatOps | Recomendar las acciones a seguir con base en el diagnóstico y la KB.<br>Recomendar resolver vs. escalar, con justificación | Database | No | Media | Semi | SRE |
| AG-10 | Investigar el issue | Investigación | Monitoreo y Obs. / ITSM | Analizar el problema reportado recolectando logs, métricas y contexto. | Monitoring, Database | No | Media-Alta | Semi | SRE |
| AG-11 | Encontrar la causa raíz | Investigación | Monitoreo y Obs. | Determinar la causa raíz correlacionando síntomas, cambios y dependencias. | Monitoring, Azure SRE Agent | No | Media-Alta | Semi | SRE |
| AG-12 | Asistente de investigación | Investigación | ChatOps | Colaborar con un especialista humano durante la investigación en tiempo real. | ChatOps, Monitoring | Sí | Media-Baja | Asistido | SRE |
| AG-13 | Diagnóstico de alerta crítica | Incidentes / SRE | Monitoreo y Obs. | Diagnosticar una alerta de salud y proponer causa raíz.<br>Recibir alerta y contexto<br>Consultar métricas y logs<br>Correlacionar eventos<br>Generar hipótesis de causa raíz y abrir incidente | Monitoring, Azure SRE Agent, Database | No | Alta | Semi | SRE |
| AG-14 | Crear incidente | Incidentes / SRE | Monitoreo y Obs. / Mail | Abrir automáticamente un incidente cuando se detecta un evento relevante. | ITSM, Monitoring | No | Media-Alta | Total | SRE |
| AG-15 | Remediación de incidente en Azure | Incidentes / SRE | Monitoreo y Obs. / ITSM | Ejecutar acción correctiva sobre un recurso de Azure.<br>Validar diagnóstico<br>Proponer acción de remediación<br>Solicitar aprobación (HITL)<br>Ejecutar runbook y verificar salud | Azure SRE Agent, Monitoring | Sí | Alta | Asistido | SRE / Cloud Ops |
| AG-16 | Generar solución | Resolución | ITSM / ChatOps | Proponer o ejecutar la solución al problema y validar el resultado. | Azure SRE Agent, AWS DevOps Agent | Sí | Media-Alta | Asistido | SRE / DevOps |
| AG-17 | Validar en la KB | Conocimiento | ITSM / ChatOps | Buscar en la base de conocimiento artículos y soluciones aplicables al caso. | Database | No | Media | Total | SRE / Soporte |
| AG-18 | Documentar en la KB | Conocimiento | Cierre de incidente | Registrar la solución y el aprendizaje en la base de conocimiento.<br>Indexar el artículo en el Vector KB (embedding + upsert, vía DA-009)<br>Actualizar CMDB si cambió un activo<br>Asignar código de cierre | Database, PDF, CMDB, TL-10 (Vector KB) | Condicional | Baja | Semi | SRE / Soporte |
| AG-19 | Consultar una base de datos | Datos | Bajo demanda | Ejecutar consultas a bases de datos para obtener información de apoyo. | Database | No | Media-Alta | Total | Data / SRE |
| AG-20 | Informe post-incidente (RCA) | Reportes | Cierre de incidente | Documentar causa raíz y acciones tras un incidente.<br>Recopilar línea de tiempo y acciones<br>Consolidar métricas de impacto<br>Generar informe (PDF / Excel)<br>Adjuntar al ticket | PDF, Excel, Database | No | Media | Semi | SRE |
| AG-21 | Ajustar el modelo | MLOps / Mejora | Programado / bajo demanda | Reentrenar o afinar el modelo con la retroalimentación de casos resueltos. | Database, Excel | Sí | Baja | Asistido | Data / MLOps |
| AG-24 | Escalamiento funcional con contexto | Gestión de tickets | ITSM / ChatOps | Escalar a L2/L3, vendor o seguridad cuando el incidente supera el conocimiento o permiso del agente, empaquetando el diagnóstico previo.<br>Consolidar diagnóstico, pasos ejecutados y evidencia<br>Identificar equipo/nivel destino según categoría<br>Transferir con contexto completo<br>Notificar al responsable | Database, ITSM, ChatOps | Condicional | Alta | Semi | Service Desk / SRE |
| AG-28 | Gestión de problemas (Problem Record) | Conocimiento | Cierre de incidente / Programado | Detectar incidentes recurrentes con la misma causa raíz y convertirlos en un Problem Record, distinto del RCA puntual de AG-20.<br>Analizar tendencias de incidentes cerrados<br>Detectar causa raíz recurrente<br>Crear/actualizar Problem Record<br>Vincular incidentes relacionados | Database, Ticket History | Condicional | Media | Semi | SRE / Problem Management |

---

## 4. Capa de herramientas (Tools — MCP / APIs)

*Herramientas y conectores que los agentes invocan para leer, actuar y generar artefactos sobre la plataforma*

| ID | Herramienta | Categoría | Descripción | Tipo de operación | Capacidades clave | Conectores / Integración (MCP / API) | Prioridad (propuesta) |
|---|---|---|---|---|---|---|---|
| TL-01 | Excel (Reader / Create) | Documentos / Datos | Lectura y generación de hojas de cálculo usadas como insumo o como salida de los agentes. | Lectura y creación | Lectura de hojas, rangos y tablas<br>Extracción de datos estructurados<br>Escritura de resultados y métricas<br>Generación de reportes y plantillas | MCP Excel / Office.js / OpenPyXL | Alta |
| TL-02 | PDF (Reader / Create) | Documentos / Datos | Lectura de documentos PDF (incl. adjuntos de tickets) y generación de informes en PDF. | Lectura y creación | Extracción de texto y tablas<br>OCR de documentos escaneados<br>Lectura de adjuntos de tickets<br>Generación de reportes y evidencias | MCP PDF / pdfplumber / PDF renderer | Alta |
| TL-03 | Database | Datos | Acceso a bases de datos para consultar y persistir información operativa de los agentes. | Lectura y escritura | Consultas de lectura (SELECT)<br>Escritura / actualización controlada | SQL (PostgreSQL / SQL Server) / MCP Database | Alta |
| TL-04-1 | Monitoring — Prometheus / Grafana | Observabilidad | Consulta de métricas, alertas y estado de salud de los sistemas en Prometheus/Grafana para diagnóstico y verificación. | Lectura | Consulta de métricas y series de tiempo<br>Lectura de alertas activas<br>Correlación de eventos<br>Verificación de salud post-remediación | Prometheus / Grafana | Media |
| TL-04-2 | Monitoring — Datadog | Observabilidad | Consulta de métricas, alertas y estado de salud de los sistemas en Datadog para diagnóstico y verificación. | Lectura | Consulta de métricas y series de tiempo<br>Lectura de alertas activas<br>Correlación de eventos<br>Verificación de salud post-remediación | Datadog | Media |
| TL-04-3 | Monitoring — Azure Monitor | Observabilidad | Consulta de métricas, alertas y estado de salud de los sistemas en Azure Monitor para diagnóstico y verificación. | Lectura | Consulta de métricas y series de tiempo<br>Lectura de alertas activas<br>Correlación de eventos<br>Verificación de salud post-remediación | Azure Monitor | Media |
| TL-04-4 | Monitoring — CloudWatch | Observabilidad | Consulta de métricas, alertas y estado de salud de los sistemas en CloudWatch para diagnóstico y verificación. | Lectura | Consulta de métricas y series de tiempo<br>Lectura de alertas activas<br>Correlación de eventos<br>Verificación de salud post-remediación | CloudWatch | Media |
| TL-05 | Azure SRE Agent | Agentes especializados | Agente de confiabilidad (SRE) para diagnóstico y remediación de incidentes en Azure. | Lectura y acción | Diagnóstico de incidentes<br>Análisis de causa raíz<br>Ejecución de runbooks de remediación<br>Escalamiento con aprobación (HITL) | Azure SRE Agent | Media-Alta |
| TL-06 | AWS DevOps Agent | Agentes especializados | Agente para operaciones de DevOps y remediación en entornos AWS. | Lectura y acción | Diagnóstico de incidentes<br>Análisis de causa raíz<br>Ejecución de runbooks de remediación<br>Escalamiento con aprobación (HITL) | AWS DevOps Agent | Media |
| TL-07 | Azure DevOps | DevOps / SCM | Plataforma de gestión de código, pipelines y work items. | Lectura y creación | Lectura / creación de work items<br>Gestión de pipelines y builds<br>Consulta de repositorios y PRs<br>Trazabilidad de despliegues | Azure DevOps REST API | Media |
| TL-08 | GitHub | DevOps / SCM | Plataforma de repositorios de código, issues y automatización. | Lectura y creación | Lectura / creación de issues y PRs<br>Consulta de repositorios y commits<br>GitHub Actions / workflows<br>Gestión de code review | GitHub REST / GraphQL API / MCP GitHub | Baja |
| TL-09 | Postman | Integración / APIs | Cliente para probar, documentar y ejecutar llamadas a APIs REST usadas por los agentes. | Lectura y creación | Ejecución de requests REST (GET/POST/PUT/DELETE)<br>Colecciones y entornos reutilizables<br>Pruebas automatizadas de endpoints<br>Documentación y mocks de APIs | Postman API / Newman / OpenAPI | Media-Alta |
| TL-10 | Vector KB | Conocimiento y datos | Base de conocimiento vectorizada para búsqueda semántica de artículos, soluciones y casos previos. | Lectura y escritura | Búsqueda semántica (similarity search)<br>Recuperación de artículos y soluciones aplicables (RAG)<br>Soporte a agentes de diagnóstico y conocimiento (AG-09, AG-17)<br>Indexación incremental de artículos cerrados, con deduplicación (AG-18, DA-006 lado de escritura) | MCP Vector DB / Embeddings API | Media-Alta |
| TL-11 | CMDB | Conocimiento y datos | Base de datos de gestión de configuración con el inventario de activos, servicios y sus relaciones. | Lectura y escritura | Consulta de activos y componentes afectados<br>Relaciones e impacto entre servicios (CIs)<br>Contexto de configuración para diagnóstico y remediación<br>Actualización de activos tras cambio de hardware (AG-18) | CMDB API / ITSM (ServiceNow CMDB) | Media-Baja |
| TL-12 | Ticket History | Conocimiento y datos | Histórico de tickets resueltos, usado como fuente de contexto y de métricas para dashboards y correlación de incidentes. | Lectura | Consulta de tickets pasados y su resolución<br>Correlación de incidentes similares (AG-08)<br>Insumo para dashboards y KPIs | ITSM / Ticket History DB | Media-Alta |



---

## 5. Catálogo de runbooks

*Procedimientos automatizados que los agentes ejecutan ante eventos de los canales de entrada, usando las herramientas de la plataforma*

| ID | Runbook | Categoría | Disparador (Canal) | Objetivo y pasos clave | Herramientas (Tools) | HITL (Aprobación) | Prioridad | Nivel de automatización | Dueño / Equipo |
|---|---|---|---|---|---|---|---|---|---|
| RB-01 | Rollback de despliegue fallido | DevOps / CI-CD | Monitoreo y Obs. / ChatOps | Revertir un despliegue con errores post-release.<br>Detectar fallo tras el deploy<br>Identificar pipeline / commit<br>Ejecutar rollback<br>Notificar y registrar | Azure DevOps, GitHub, Monitoring | Sí | Media-Alta | Asistido | DevOps |
| RB-02 | Reseteo de acceso / desbloqueo de usuario | Service Desk | Mail / ChatOps / ITSM | Atender solicitudes de acceso comunes de forma segura.<br>Verificar identidad del solicitante<br>Validar política de acceso<br>Ejecutar reset / desbloqueo<br>Registrar para auditoría | Database | Condicional | Media-Alta | Semi | Service Desk / IAM |
| RB-03 | Health check post-remediación | SRE | Programado / tras remediación | Validar que el sistema quedó sano tras una acción correctiva.<br>Consultar métricas clave<br>Comparar contra umbrales<br>Cerrar incidente o reabrir si persiste<br>Notificar resultado | Monitoring, Azure SRE Agent | No | Alta | Total | SRE |

---

## 6. Guardrails y gobierno

*Controles transversales de seguridad, cumplimiento y supervisión aplicados antes, durante y después de que el agente actúa*

| ID | Control | Fase | Descripción / Objetivo | Mecanismo / Cómo se aplica | Herramientas / Fuente | Dueño / Responsable | Prioridad (propuesta) |
|---|---|---|---|---|---|---|---|
| GR-01 | Verificación del solicitante | Antes de actuar | Confirmar la identidad y legitimidad de quien origina la solicitud antes de procesarla. | Autenticación y mapeo a identidad corporativa<br>Verificación de remitente (SPF/DKIM) en correo<br>Validación de permisos del solicitante | Guardrails, InputChannels | Seguridad / IAM | Alta |
| GR-02 | Control de inyección de prompts | Antes de actuar | Detectar y neutralizar intentos de manipular al agente mediante entradas maliciosas. | Sanitización y validación de entradas<br>Detección de prompt injection y jailbreak<br>Listas de bloqueo y patrones sospechosos | Guardrails | Seguridad / Plataforma | Alta |
| GR-03 | Enmascaramiento de PII | Antes de actuar | Proteger datos personales y sensibles antes de que los procese el agente o el LLM. | Detección y redacción de PII<br>Tokenización / anonimización<br>Controles sobre datos de entrada | Guardrails, Database | Seguridad / Cumplimiento | Alta |
| GR-04 | Menor privilegio (Least privilege) | Durante la ejecución | Limitar los accesos y herramientas del agente al mínimo necesario para su tarea. | Roles y scopes por agente<br>Acceso just-in-time a herramientas<br>Segregación de credenciales | Guardrails / Governance | Seguridad / Plataforma | Alta |
| GR-05 | Aprobaciones HITL | Durante la ejecución | Requerir validación humana antes de acciones sensibles o de alto riesgo. | Cola de aprobación con contexto y nivel de riesgo<br>Aprobar / rechazar / devolver<br>Registro de la decisión | Guardrails / HITL, Orquestador | Operaciones / Owner del proceso | Alta |
| GR-06 | Límites de tasa (Rate limits) | Durante la ejecución | Controlar la frecuencia y el volumen de acciones para evitar abusos o sobrecostos. | Cuotas por agente, canal y herramienta<br>Throttling y backoff<br>Circuit breakers ante errores | Guardrails, Orquestador | Plataforma / FinOps | Media |
| GR-07 | Bitácora de auditoría | Después de actuar | Registrar de forma inmutable qué hizo cada agente, cuándo y con qué permisos. | Trazabilidad de acciones y decisiones<br>Evidencia exportable para auditoría<br>Retención y sellado de logs | Guardrails / Governance, Database | Cumplimiento / Auditoría | Alta |
| GR-08 | Métricas del agente | Después de actuar | Medir desempeño, calidad y comportamiento de los agentes en el tiempo. | Tasa de éxito y de intervención<br>Precisión y desvíos<br>Alertas de comportamiento anómalo | Monitoring, Database | SRE / Plataforma | Media |
| GR-09 | Red teaming | Después de actuar | Probar de forma adversarial la robustez y seguridad de los agentes. | Ejercicios de ataque controlado<br>Pruebas de fuga de datos y jailbreak<br>Hallazgos y remediación | Guardrails, herramientas de pruebas | Seguridad | Media-Baja |

