# Estudio de Mercado: Mesa de Servicios de Próxima Generación (Gen Next)
## Investigación Estratégica para el Diseño de una Mesa de Servicio de Nueva Generción
*Documento v1.0 — Julio 2026. Actualizado con ITIL (Version 5), mercado Colombia/Latam, pricing outcome-based, XLA y agentic AI.*

---

## Resumen Ejecutivo

El mercado global de IT Service Desk alcanzó entre USD 7.8 y USD 11.4 mil millones en 2024, dependiendo si se mide solo software o incluyendo servicios administrados, con tasas de crecimiento entre el 9% y el 17% anual hacia 2033–2035 ([Growth Market Reports](https://growthmarketreports.com/report/it-service-desk-market)) ([Apps Run The World](https://www.appsruntheworld.com/top-10-it-service-management-software-vendors-and-market-forecast/)). El hilo conductor de este estudio es una transformación estructural: la mesa de servicio está dejando de ser un centro de costos reactivo para convertirse en una plataforma de valor autónoma, predictiva y orientada a la experiencia del empleado.

Los hallazgos clave de esta investigación son:

- **Gartner retiró el Magic Quadrant de plataformas ITSM en 2023** por "comoditización", y en 2024 lanzó un nuevo cuadrante específico para **AI Applications in ITSM** — señal inequívoca de que la diferenciación ya no está en la plataforma, sino en la inteligencia que la habilita ([InvGate](https://blog.invgate.com/itsm-gartner-magic-quadrant)).
- **Los 12 grandes proveedores** han convergido hacia el mismo mensaje: "AI-first", agentes virtuales, XLA sobre SLA y remediación autónoma. La diferenciación real está en la plataforma propietaria, la profundidad de la IA y la madurez del modelo de gobierno.
- **ITIL ya está en su Version 5**, lanzada oficialmente el 12 de febrero de 2026 por PeopleCert, y reemplaza el concepto de Service Value Chain por un ciclo de vida de 8 etapas (Discover→Design→Acquire→Build→Transition→Operate→Deliver→Support), consolida el marco DPSM (Digital Product and Service Management) y establece un modelo formal de gobernanza de IA ([Tideline Insights](https://www.tidelineinsights.com/blog/itil-5-whats-coming.html)) ([Rixmind](https://rixmind.com/itil-5-what-changed-and-why-it-matters/)).
- **HDI** ofrece el marco de certificación y métricas de referencia más estructurado de la industria, con benchmarks de FCR, MTTR, CSAT y costo por ticket que permiten comparar objetivamente la madurez de cualquier mesa.
- El **mercado de plataformas ITSM** está dominado por ServiceNow (44.4% de cuota entre los top 10 proveedores, según [Apps Run The World](https://www.appsruntheworld.com/top-10-it-service-management-software-vendors-and-market-forecast/)), y la batalla competitiva se libra en la capa de IA agéntica, AIOps y experiencia del empleado (DEX).
- El **casi 70% de las empresas planea adoptar Experience Level Agreements (XLA) en 2026** (XLA Institute "State of XLA 2025"), con expansión de esta disciplina más allá de TI hacia salud, RR.HH. y finanzas, según el primer reporte global "State of XLA 2025" del XLA Institute ([EIN Presswire](https://www.einpresswire.com/article/823090394/xla-institute-releases-groundbreaking-state-of-xla-2025-report?code=9Hv3x5D-vwZo-peK)).
- La **agentic AI** pasó de la experimentación a la producción, pero con matices importantes: 51% de las empresas ya tiene agentes de IA desplegados de alguna forma, pero solo el 11% opera en producción plena, mientras Gartner proyecta que más del 40% de los proyectos de IA agéntica serán cancelados hacia fines de 2027 por costos, gobernanza o valor de negocio poco claro ([Brilo AI, vía G2/OneReach.ai y Gartner](https://www.brilo.ai/resources/agentic-ai-statistics)).
- El **mercado ITSM (Gestión Integral de los Servicios de TI) en Colombia** está valuado en aproximadamente USD 108.5 millones en 2026 y crecerá a una tasa del 14.08% CAGR hasta 2031, impulsado por adopción cloud (63.45%), un sector de servicios que crece más rápido (13.82% CAGR) que el de soluciones, y un ecosistema financiero que ya usa IA en el 81% de sus establecimientos de crédito ([Mordor Intelligence Colombia ITSM](https://www.mordorintelligence.com/industry-reports/colombia-information-technology-service-management-itsm-market)) ([Superintendencia Financiera de Colombia](https://www.superfinanciera.gov.co/publicaciones/10116043/sistema-financiero-acelera-implementacion-de-canales-digitales/)).

---

## 1. Evolución Histórica de las Mesas de Servicio

### 1.1 La Línea de Tiempo: Del Timbre al Agente Autónomo

La evolución de las mesas de servicio no es lineal — es una secuencia de ampliaciones de alcance y de automatización progresiva de la inteligencia humana.

| Etapa | Período | Características Principales | Tecnología Habilitadora |
|---|---|---|---|
| **Help Desk** | 1970s–1990s | Punto único de contacto; "gatekeeper"; solo restauración de servicio; múltiples help desks por aplicación | Teléfono, correo, bases de datos de tickets rudimentarias |
| **Service Desk (ITIL v2)** | 2001 | Alcance ampliado: incidentes + solicitudes + cambios; "habilitador de servicios" | ITSM software, CMDB básico, bases de conocimiento |
| **Service Desk (ITIL v3)** | 2007 | Integración en el ciclo de vida del servicio; rol formal en Service Operation | Portales web, SLA, herramientas de reporting |
| **Enterprise Service Management** | 2010–2016 | Extensión a RR.HH., finanzas, operaciones; ESM como categoría propia | Workflows cross-funcionales, catálogos de servicio |
| **Digital Workplace / Virtual Agent** | 2015–2020 | Autoservicio inteligente; chatbots NLP; portales de empleado | AI básica, NLP, RPA, Office 365 integration |
| **AI-Augmented Service Desk (AITSM)** | 2020–2023 | IA como capa de inteligencia sobre ITSM; GenAI para tickets; predictive analytics | GenAI, ML, LLM, AIOps, análisis de sentimiento |
| **Autonomous Service Desk** | 2023–2026 | Agentes de IA que persiguen objetivos; resolución end-to-end sin humanos; "zero incidents" como aspiración | Agentic AI, multi-agent systems, AIOps avanzado, DEX |
| **Digital Twins Operations** | Emergente | Réplica digital de la infraestructura y procesos; operaciones predictivas basadas en simulación | Digital twins, process mining, observabilidad continua |

*(Fuentes: [DITY/SlideShare](https://fr.slideshare.net/slideshow/dit-yvol4iss03/29363674), [ServiceNow Newsroom](https://newsroom.servicenow.com/press-releases/details/2025/ServiceNow-Sets-New-Standard-for-Fully-Autonomous-IT-Envisioning-a-Zero-Downtime-Zero-Outage-Future-With-Agentic-AI/default.aspx), [Ivanti](https://www.ivanti.com/en-gb/blog/agentic-ai-it-service-autonomy))*


---

### Línea de Tiempo Visual

![Línea de tiempo — Evolución de las mesas de servicio](https://d2z0o16i8xm8ak.cloudfront.net/d93eac35-3c61-4da0-96a8-ed5148a1ce99/d64d77ad-ec99-4ab3-959e-0137d5566ad9/svg2_timeline.png?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiaHR0cHM6Ly9kMnowbzE2aTh4bThhay5jbG91ZGZyb250Lm5ldC9kOTNlYWMzNS0zYzYxLTRkYTAtOTZhOC1lZDUxNDhhMWNlOTkvZDY0ZDc3YWQtZWM5OS00YWIzLTk1OWUtMDEzN2Q1NTY2YWQ5L3N2ZzJfdGltZWxpbmUucG5nPyoiLCJDb25kaXRpb24iOnsiRGF0ZUxlc3NUaGFuIjp7IkFXUzpFcG9jaFRpbWUiOjE3ODQ2NTU0NDZ9fX1dfQ__&Signature=EqgBEHhWltrryxZlPyVlOf55QHHgViWRvk-8ba1G5Vk7sQkNKA07L9Kqk6o2JXTA4ogZGa0nrnRAREZ84-pLaDzxFZRmR6jbsftolDAKB4gFZHbWn7pnZGFx5HderDYWqy1mpcWv~oaQH0h2T815vqdM8ibGYrh8RAt2N36Dp4AGV3k-R8w2PXzUKK6b6MojtnzCVwmX-1qLa-J~K8A8baTU3L0EzmdHwSSx4DjoJFxvnpTyoWe3Ih~7DtumoUnkchbFLIGw9XeGH9~HNdHJukySq61fsW8I27DIh8UR0spUpq4in3D7y5Dix9Eo~Jl4FgZMA-d1hoknVoxXX8D86w__&Key-Pair-Id=K1BF7XGXAIMYNX)

---



### 1.2 La Distinción Fundacional: Call Center vs. Help Desk vs. Service Desk

---

### Evolución Visual de las Mesas de Servicio

![Línea de tiempo — Evolución de las mesas de servicio](https://d2z0o16i8xm8ak.cloudfront.net/d93eac35-3c61-4da0-96a8-ed5148a1ce99/d64d77ad-ec99-4ab3-959e-0137d5566ad9/svg2_timeline.png?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiaHR0cHM6Ly9kMnowbzE2aTh4bThhay5jbG91ZGZyb250Lm5ldC9kOTNlYWMzNS0zYzYxLTRkYTAtOTZhOC1lZDUxNDhhMWNlOTkvZDY0ZDc3YWQtZWM5OS00YWIzLTk1OWUtMDEzN2Q1NTY2YWQ5L3N2ZzJfdGltZWxpbmUucG5nPyoiLCJDb25kaXRpb24iOnsiRGF0ZUxlc3NUaGFuIjp7IkFXUzpFcG9jaFRpbWUiOjE3ODQ2NTU0NDZ9fX1dfQ__&Signature=EqgBEHhWltrryxZlPyVlOf55QHHgViWRvk-8ba1G5Vk7sQkNKA07L9Kqk6o2JXTA4ogZGa0nrnRAREZ84-pLaDzxFZRmR6jbsftolDAKB4gFZHbWn7pnZGFx5HderDYWqy1mpcWv~oaQH0h2T815vqdM8ibGYrh8RAt2N36Dp4AGV3k-R8w2PXzUKK6b6MojtnzCVwmX-1qLa-J~K8A8baTU3L0EzmdHwSSx4DjoJFxvnpTyoWe3Ih~7DtumoUnkchbFLIGw9XeGH9~HNdHJukySq61fsW8I27DIh8UR0spUpq4in3D7y5Dix9Eo~Jl4FgZMA-d1hoknVoxXX8D86w__&Key-Pair-Id=K1BF7XGXAIMYNX)

---



| Función | Misión Principal | Alcance |
|---|---|---|
| **Call Center** | Manejar grandes volúmenes de llamadas; filtrar y derivar | Punto de contacto y distribución estructurada |
| **Help Desk** | Coordinación para la restauración del servicio; "arreglar cosas" | Infraestructura, herramientas de seguimiento, base de conocimiento |
| **Service Desk** | Servicio integral: incidentes, solicitudes, consultas, altas/bajas/cambios | Alcance configurable; representa al usuario dentro de TI |

*(Fuente: [DITY/SlideShare](https://fr.slideshare.net/slideshow/dit-yvol4iss03/29363674))*

### 1.3 El Salto Hacia la Autonomía: Predicciones de Gartner

Ivanti cita predicciones de Gartner que cuantifican la velocidad de la transición hacia la autonomía:

| Predicción de Gartner | Cifra | Horizonte |
|---|---|---|
| Apps empresariales con agentes de IA específicos | ~40% (desde <5% en 2025) | Fin de 2026 |
| Empresas que desplegarán agentes de IA agéntica para operar su infraestructura TI | 70% | 2029 |
| Decisiones diarias de trabajo tomadas autónomamente por IA | al menos 15% | 2028 |
| Proyectos de IA agéntica cancelados por costo/valor/riesgo inadecuados | más del 40% | Fin 2027 |

*(Fuente: [Ivanti citando Gartner](https://www.ivanti.com/en-gb/blog/agentic-ai-it-service-autonomy))*

---

## 2. Cómo los Analistas Clasifican el Mercado

### 2.1 Gartner: El Pivot Hacia la IA

**El cambio más importante:** Gartner retiró su *Magic Quadrant for ITSM Platforms* en 2023 por "comoditización y falta de diferenciación" en las plataformas ([InvGate](https://blog.invgate.com/itsm-gartner-magic-quadrant)). En 2024 lanzó el primer **Magic Quadrant for AI Applications in ITSM**, con una segunda edición en 2025. Este reposicionamiento es la señal más clara de que la diferenciación en el mercado ya no está en la plataforma base, sino en la inteligencia aplicada sobre ella.

**Magic Quadrant for AI Applications in ITSM — Edición 2024:**

| Cuadrante | Vendors |
|---|---|
| **Leaders** | Aisera, ServiceNow |
| **Challengers** | Moveworks |
| **Niche Players** | BMC, Espressive, Freshworks, Halo Service Solutions, OpenText, Serviceaide, SymphonyAI |

*(Fuente: [Gartner Reprint vía Scribd](https://www.scribd.com/document/809079051/Gartner-Reprint))*

En la edición **2025**, ServiceNow fue el único Líder del cuadrante, y se incorporaron Atlassian, ManageEngine y SysAid como Niche Players nuevos; BMC Helix ascendió a Visionario ([DataLunix](https://www.datalunix.com/post/freshservice-magic-quadrant)) ([Synta](https://www.synta.pro/post/artificial-intelligence-in-itsm-key-takeaways-from-the-gartner-magic-quadrant-2024-2025)).

**Las 9 Capacidades Críticas según Gartner** (un producto debe incluir al menos 5 para ser evaluado):

| Capacidad | Descripción |
|---|---|
| Virtual support agent | Interfaz conversacional orientada al consumidor de negocio |
| Public knowledge discovery | Descubrimiento de conocimiento usando LLM públicos |
| Intelligent escalation | Escalamiento antes de superar umbrales de SLA cronometrados |
| Intelligent risk advisory | Asesoría de riesgo de cambios planeados usando historial |
| Intelligent triage | Guía sobre priorización de incidentes |
| Intelligent categorization | Categorización por servicio, CI o solución |
| Intelligent swarming | Identificación de expertos y grupos resolutores |
| Major incident detection | Detección de incidentes de alto impacto |
| Problem detection | Detección de múltiples incidentes con causa raíz común |

*(Fuente: [Gartner Reprint vía Scribd](https://www.scribd.com/document/809079051/Gartner-Reprint))*

**Gartner Hype Cycle for ITSM 2025:** Las innovaciones más nuevas son *agent-native I&O*, *natural language case extraction* y *AI-powered IT agent advisory*. "ITSM platforms" fue retirado del Hype Cycle por alcanzar estatus *mainstream*, confirmando la comoditización ([Faddom/Gartner Hype Cycle ITSM 2025](https://faddom.com/wp-content/uploads/2026/03/2025-Hype-Cycle-for-ITSM-Gartner-Report.pdf)).

### 2.2 ITIL (Version 5): La Evolución hacia DPSM y Gobernanza de IA

El nombre oficial correcto del nuevo marco es **"ITIL (Version 5)"** — no "ITIL 5" — y fue lanzado por **PeopleCert**, que absorbió completamente la marca Axelos y es ahora el único organismo rector de ITIL, PRINCE2 y marcos relacionados ([Tideline Insights](https://www.tidelineinsights.com/blog/itil-5-whats-coming.html)). PeopleCert enfatiza que la actualización **"no es un reinicio"**: el conocimiento, la experiencia y las certificaciones ITIL 4 existentes "permanecen totalmente vigentes", y ITIL 4 sigue disponible como ruta de certificación para quienes deseen continuarla ([PeopleCert — ITIL Version 5 Explained](https://www.peoplecert.org/news-and-announcements/itil-version-5-explained)).

**Timeline oficial de lanzamiento:**

| Fecha | Hito |
|---|---|
| 29 de enero de 2026 | Anuncio oficial de ITIL (Version 5) |
| 12 de febrero de 2026 | Lanzamiento del examen ITIL (Version 5) Foundation |
| 26 de febrero de 2026 | Lanzamiento del Foundation Bridge para poseedores de ITIL 4 (examen de actualización enfocado en el 36% de contenido nuevo y el modelo de ciclo de vida actualizado) |
| 19 de marzo de 2026 | Publicación del módulo ITIL Experience |
| 26 de marzo de 2026 | Publicación del módulo ITIL Product |
| 2 de abril de 2026 | Publicación del módulo ITIL Service |
| 9 de abril de 2026 | Publicación de ITIL Strategy / ITIL Transformation |
| 14 de mayo de 2026 | Publicación de los módulos MPT (Managing Professional Transition) restantes |

*(Fuentes: [Tideline Insights](https://www.tidelineinsights.com/blog/itil-5-whats-coming.html), [Rixmind](https://rixmind.com/itil-5-what-changed-and-why-it-matters/))*

**Composición del contenido:** ITIL (Version 5) se compone de **40% de contenido retenido directamente de ITIL 4, 24% de contenido actualizado o mejorado y 36% completamente nuevo** ([Tideline Insights](https://www.tidelineinsights.com/blog/itil-5-whats-coming.html)) ([Rixmind](https://rixmind.com/itil-5-what-changed-and-why-it-matters/)).

**El nuevo ciclo de vida de 8 etapas — Product and Service Lifecycle:** Reemplaza la Service Value Chain de ITIL 4 dentro del Service Value System (SVS), que se mantiene y se actualiza:

1. **Discover** — identificación de necesidades de negocio, oportunidades y señales de demanda (formaliza lo que ITIL 4 dejaba implícito)
2. **Design** — traducción de necesidades a especificaciones y arquitecturas de servicio
3. **Acquire** — obtención de componentes (tecnología, personas, proveedores); etapa explícita nueva
4. **Build** — desarrollo o configuración de los componentes del servicio, incluyendo configuración de agentes de IA en entornos AI-native
5. **Transition** — paso del servicio de desarrollo a operación en vivo
6. **Operate** — ejecución del servicio en producción (incident management, request fulfilment, event management se retienen íntegramente)
7. **Deliver** — formaliza la realización y demostración del valor como fase explícita del ciclo de vida, con obligaciones de medición propias
8. **Support** — sostenimiento del servicio, incluyendo mejora continua embebida en el ciclo de vida (antes era una pista paralela)

*(Fuente: [Tideline Insights](https://www.tidelineinsights.com/blog/itil-5-whats-coming.html))*

**De ITSM a DPSM:** ITIL (Version 5) amplía el marco hacia la **Digital Product and Service Management (DPSM)**, unificando la gestión de productos digitales, aplicaciones, plataformas y APIs junto con los servicios de TI tradicionales — reflejando que muchas organizaciones ya gestionan estos elementos de forma convergente ([Rixmind](https://rixmind.com/itil-5-what-changed-and-why-it-matters/)).

**El 6C AI Capability Model:** Es el elemento donde se concentra la mayor parte del contenido genuinamente nuevo (36%). PeopleCert lo introduce como marco para que las organizaciones de TI construyan y gobiernen capacidades de IA dentro de la gestión de servicios, sirviendo como herramienta de auditoría retrospectiva para quienes ya usan IA en triage, agentes virtuales o analítica predictiva, y como hoja de ruta para quienes recién comienzan ([Tideline Insights](https://www.tidelineinsights.com/blog/itil-5-whats-coming.html)). Los 6 componentes son:

| Componente | Descripción |
|---|---|
| **Creation** | Generación de nuevo contenido, configuraciones o soluciones usando IA |
| **Curation** | Filtrado, organización y mantenimiento de outputs generados o asistidos por IA |
| **Clarification** | Uso de IA para interpretar solicitudes ambiguas o extraer intención de datos ruidosos |
| **Cognition** | Análisis impulsado por IA, reconocimiento de patrones y soporte a la decisión |
| **Communication** | Interacciones mediadas por IA entre usuarios y sistemas de gestión de servicios |
| **Coordination** | Orquestación de agentes de IA y actores humanos a través de flujos de trabajo de servicio |

El modelo incluye además obligaciones explícitas de gobernanza: responsabilidad sobre los outputs de IA, requisitos de transparencia para decisiones mediadas por IA, y rutas de escalamiento cuando falla la coordinación entre agentes ([Tideline Insights](https://www.tidelineinsights.com/blog/itil-5-whats-coming.html)). Adicionalmente, **AI Governance** se instituye como el único módulo de extensión independiente dentro del nuevo esquema de certificación, junto a **ITIL Experience**, que se separa como disciplina propia con su propia base de conocimiento ([Rixmind](https://rixmind.com/itil-5-what-changed-and-why-it-matters/)).

**Qué se mantiene igual:**


---

### ITIL (Version 5): Diagrama del Ciclo de Vida y Modelo 6C

![ITIL Version 5 — Ciclo de vida 8 etapas y Modelo 6C de IA](https://d2z0o16i8xm8ak.cloudfront.net/d93eac35-3c61-4da0-96a8-ed5148a1ce99/facfc879-5417-4627-8603-fbba8ec1160e/svg5_itil_v5.png?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiaHR0cHM6Ly9kMnowbzE2aTh4bThhay5jbG91ZGZyb250Lm5ldC9kOTNlYWMzNS0zYzYxLTRkYTAtOTZhOC1lZDUxNDhhMWNlOTkvZmFjZmM4NzktNTQxNy00NjI3LTg2MDMtZmJiYThlYzExNjBlL3N2ZzVfaXRpbF92NS5wbmc~KiIsIkNvbmRpdGlvbiI6eyJEYXRlTGVzc1RoYW4iOnsiQVdTOkVwb2NoVGltZSI6MTc4NDY1NTQ0Nn19fV19&Signature=m06xn2k~V6llnrS4BbadQjMGyLKmOozWfqpKEbtrau3B0fnDv6F5RuO~ILBboFBBdbMcevQ-ceNU-FA8dDdseQ1lbmIdzXEYDx0garLdRRkp9H8KkB6cqahF4n2SjxIXq12Kc3svNLRdksbqpVyKZVuJyVIJ5L4WL4jLziG7-FY8pUcU6P98x1hDtNvsyQHI50quVRbiCkbcQ3po7QbYuI7fCkX1snlmuFDqGmi7IUwzmlY0QOyh~VPTOrj3SHVdz6FpcVg355Fr8WSTzT0ufLc7JXqLJKEaLnGM8S~5msra3reg8YyOCd9EIJK70Q4-2zoi8cA5GL5VzgcJUJaejw__&Key-Pair-Id=K1BF7XGXAIMYNX)

---



| Elemento | Estado en ITIL (Version 5) |
|---|---|
| Los 7 Guiding Principles (Focus on Value, Start Where You Are, Progress Iteratively with Feedback, Collaborate and Promote Visibility, Think and Work Holistically, Keep It Simple and Practical, Optimize and Automate) | Se mantienen sin cambios |
| Four Dimensions of Service Management | Se conservan, actualizadas para reflejar contextos de IA y digitales |
| Service Value System (SVS) | Se retiene y actualiza, no se reemplaza |
| Las 34 prácticas de ITIL 4 | Se retienen todas; 5 son recategorizadas, ninguna se elimina (ejemplos: Change Enablement, Incident Management, Problem Management) |
| Certificaciones ITIL 4 existentes | Siguen siendo válidas |

*(Fuentes: [PeopleCert — ITIL Version 5 Explained](https://www.peoplecert.org/news-and-announcements/itil-version-5-explained), [Tideline Insights](https://www.tidelineinsights.com/blog/itil-5-whats-coming.html), [Rixmind](https://rixmind.com/itil-5-what-changed-and-why-it-matters/))*

**Implicación para el diseño Gen Next:** El **Shift-Left** que ITIL 4 desarrollaba en el módulo CDS (Create, Deliver and Support) permanece vigente como principio operativo — sus tres habilitadores (autoservicio, gestión del conocimiento y automatización) ahora se enmarcan explícitamente dentro del 6C AI Capability Model, particularmente en las dimensiones de Clarification y Coordination.

### 2.3 HDI: El Marco de Certificación y Métricas

El **HDI Support Center Standard** (v5.0) es la base de certificación más estructurada para centros de soporte de TI, con 8 categorías y 71 ítems auditados ([HDI Standard v5.0](https://www.thinkhdi.com/~/media/HDICorp/Files/Standards/HDI-SC-Standard-v-5-0.pdf)).

**Estructura del Estándar HDI:**

| Enablers (Habilitadores) | Results (Resultados) |
|---|---|
| 1.0 Leadership | 6.0 People Satisfaction Results |
| 2.0 Strategy and Policy | 7.0 Customer Satisfaction Results |
| 3.0 People Management | 8.0 Performance Results |
| 4.0 Resources | |
| 5.0 Process and Procedure | |

**Los 4 Niveles de Madurez HDI:**

| Nivel | Enablers | Results |
|---|---|---|
| 1 | Just Started — reconoce el valor, inicia planes | Measured — datos recolectados y reportados |
| 2 | Some Progress — evidencia de que la actividad se realiza | Comparison to Goals — datos comparados contra meta |
| 3 | Considerable Progress — realizado consistentemente | Trending to Goals — tendencia positiva en 6 meses |
| 4 | Fully Achieved/Optimized — implementación universal, mejora continua | Consistently Meeting Goals — meta alcanzada 9/12 meses |

*(Fuente: [HDI Standard v5.0](https://www.thinkhdi.com/~/media/HDICorp/Files/Standards/HDI-SC-Standard-v-5-0.pdf))*

**Modelo de Tiers HDI (Shift-Left):**

| Tier | Función |
|---|---|
| **Tier 0** | Autoayuda; self-service; self-healing — costo: USD 2 por ticket |
| **Tier 1** | Service Desk; primer contacto vía teléfono/chat — costo: USD 22 |
| **Tier 2** | Soporte técnico avanzado; expertise especializado — costo: USD 69 |
| **Tier 3** | "Élite técnica"; arquitectos; punto final antes de vendors — costo: USD 104 |

*(Fuentes: [KnowledgeHut](https://www.knowledgehut.com/blog/it-service-management/it-support-levels), [Giva](https://www.givainc.com/blog/shift-left-analysis-how-to-guide-maximize-it-service-management-itsm-efficiency/))*

### 2.4 Forrester, Everest Group e ISG

**Forrester Wave: Enterprise Service Management Platforms, Q4 2025:**

| Categoría | Vendors |
|---|---|
| **Leaders** | ServiceNow, BMC Helix, Atlassian |
| **Strong Performers** | Freshworks, HCLSoftware, Ivanti, ManageEngine, Matrix42, OpenText, Serviceware |
| **Contenders** | IFS, SolarWinds, SymphonyAI, TOPdesk, USU |

Los temas clave de Forrester: **agentic AI, ITOM, AIOps y observability**. Los Líderes se distinguen por "ayudar a las empresas a transformar las prácticas de gestión de servicios, no solo a mejorar los procesos existentes" ([Spotlight AR](https://research.oz.spotlightar.com/reports/forrester-wave-enterprise-service-management-platforms-q4-2025/leaders)).

**Everest Group PEAK Matrix for ITSM Specialist Services 2025** (publicado junio 2025, 10 vendors evaluados): Las tendencias identificadas son GenAI, AIOps, hyperautomation, predictive analytics y entrega "experience-centric" con modelos de implementación rápida y servicios modulares ([Everest Group](https://www.everestgrp.com/peak-matrix/it-service-management-itsm-specialist-services-peak-matrix-assessment.html)).

**ISG Provider Lens Future of Work Services:** Reconoce en el segmento "Next-gen Service Desk" a Unisys y Lenovo como Leaders en 2025 ([Unisys/ISG](https://www.unisys.com/siteassets/collateral/analyst-report/ar-isg-fow-quad-report-us-102025.pdf)).

**Tamaño del Mercado Global:**

| Fuente | Tamaño 2024 | Proyección | CAGR |
|---|---|---|---|
| Growth Market Reports | USD 7.8B | USD 17.4B (2033) | 9.3% |
| Apps Run The World (software ITSM) | USD 11.4B | — | 14.8% (interanual) |
| Business Research Insights | USD 3.7B | USD 18B (2035) | 17.2% |

*(Fuentes: [Growth Market Reports](https://growthmarketreports.com/report/it-service-desk-market), [Apps Run The World](https://www.appsruntheworld.com/top-10-it-service-management-software-vendors-and-market-forecast/))*

---

### Visualización: Mercado Global ITSM

![Mercado Global ITSM — Tamaño y Proyección por fuente analítica](https://d2z0o16i8xm8ak.cloudfront.net/d93eac35-3c61-4da0-96a8-ed5148a1ce99/fd048496-6b11-47be-ab25-9f5f18194dae/svg1_mercado_global.png?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiaHR0cHM6Ly9kMnowbzE2aTh4bThhay5jbG91ZGZyb250Lm5ldC9kOTNlYWMzNS0zYzYxLTRkYTAtOTZhOC1lZDUxNDhhMWNlOTkvZmQwNDg0OTYtNmIxMS00N2JlLWFiMjUtOWY1ZjE4MTk0ZGFlL3N2ZzFfbWVyY2Fkb19nbG9iYWwucG5nPyoiLCJDb25kaXRpb24iOnsiRGF0ZUxlc3NUaGFuIjp7IkFXUzpFcG9jaFRpbWUiOjE3ODQ2NTU0NDZ9fX1dfQ__&Signature=oJgA~32E-AfTzMf5r4-tZJS0n0P7SNExduH5Ihyi3ZwRx2McI3rE1jDfnHLLEU4FGQ5o8QVN--MrCbL~bj9Vv66RnpfUDmqajNoO9c2eH-E-at3YweMmckrZijiUGNYxtY54eQr-qVkoGyzwLzWyfQ3dFktH6jX8vaWPNz4mJ0yE6dwgVDkUgfFglRsWINzZtLq1~7AlIzQJ~rFhL7edelt2CIcHPNbbNZKUBf4wrFlUseNa9fwMRc56X69VR0~SNRomMcWkOfV4rVyFvaS~818ymKIdQzyvqj8AZWdZV~TEZrrpfSAETTXX6DPiIylyfvQyeLDZy550OKhXeexLaQ__&Key-Pair-Id=K1BF7XGXAIMYNX)

---



---

## 3. Cómo los 12 Grandes Proveedores Posicionan sus Mesas

### 3.1 Tabla Comparativa

| Empresa | Nombre Comercial | IA / Automatización | Diferenciador Único |
|---|---|---|---|
| **Accenture** | Intelligent Service Center / myWizard® | GenAI, agentic AI, agentes virtuales (hasta 85% de llamadas), self-healing | 86% reducción costo/contacto; modelo human+machine basado en desempeño |
| **IBM** | IBM Consulting AIOps / watsonx Orchestrate | GenAI, ML, watsonx, IBM Concert, zero-touch operations | No mesa empaquetada — ecosistema de TI autónoma (AIOps + watsonx) |
| **Kyndryl** | Interactive AI for Service Desk | ASR + NLP + HAU (Interactions LLC); resuelve 70% por canales digitales | Concierge IT con video seguro y AR; 2M contactos/mes, 650+ clientes |
| **Deloitte** | Next Gen Service Desk | Deep learning, detección anomalías, GenAIOps, OperateEdge™ | Metodología O2I (Operate to Innovate); sin plataforma propietaria |
| **Capgemini** | AI-Powered Service Desk | Agentes virtuales, PRiSM GenAI, remediación autónoma | "Composable Service Desk" (asignación dinámica IA/humano en tiempo real) |
| **Cognizant** | WorkNext AI-powered Service Desk | NLP, NLU, chatbot Bold360ai, knowledge on demand | Single door; visión "zero-touch service desk 2030" |
| **HCLTech** | GenAI-powered Digital Service Desk / AI Force | CVA, GenAI, agent assist, self-heal, 150+ idiomas | Modelo Sense→Think→Act→Engage; AI Force.Ops |
| **Infosys** | ITIL Intelligent Service Desk / ESM Café | IA cognitiva, automatización cognitiva, RPA, 90% contención digital | ESM Café sobre ServiceNow; 47 centros, 3M+ usuarios, 75-80% FCR |
| **TCS** | DeskHelp / Cognix™ / ignio | Modelo IPSC, autoaprendizaje, ignio (auto-healing cognitivo), GenAI Copilot | Machine First™; ignio como plataforma de autohealing galardonada |
| **NTT DATA** | NextGen Service Desk (Nucleus) | GenAI, agentic AI, Nucleus Virtual Agent, previene 65% de incidentes | Liderazgo en XLA; 87% FCR; 23M+ tickets/año |
| **DXC** | DXC Service Desk / UPtime | GenAI conversacional, agent co-pilot, UPtime Platform + Espressive Barista | Métricas más completas: 93% FCR, 58% menos costo/contacto, 49% menos MTTR |
| **Wipro** | LiVE Workspace™ OneDesk / HOLMES | AIOps, HOLMES, auto-reparación proactiva, Azure OpenAI | 5 torres de servicio; self-heal antes de que el usuario note el problema |

*(Fuentes: páginas oficiales de cada empresa — ver análisis detallado en sección 3.2)*

### 3.2 Patrones de Mercado y Tendencias

**5 patrones comunes entre los 12 proveedores:**

1. **Convergencia AI-first:** Todos han rebautizado su mesa como "AI-powered" o "GenAI-powered". Accenture y NTT DATA ya hablan de **agentic AI** — agentes que deciden y actúan autónomamente ([Accenture](https://www.accenture.com/content/dam/accenture/final/accenture-com/document-4/Accenture-Federal-Services-Intelligent-Service-Center.pdf)) ([NTT DATA](https://us.nttdata.com/en/services/digital-workplace-services/workplace-omnichannel-user-support)).

2. **Migración SLA → XLA:** NTT DATA hace de las "operaciones basadas en XLA" su bandera principal; Capgemini comercializa "Experience Metrics (XLAs)" como diferenciador ([NTT DATA](https://www.nttdata.com/en-ca/services/digital-workplace)) ([Capgemini](https://www.capgemini.com/solutions/ai-powered-service-desk-by-capgemini/)).

3. **Shift de "resolver rápido" a "resolver antes":** NTT DATA previene "hasta el 65% de incidentes antes de que ocurran"; Wipro auto-repara antes de que el usuario lo note ([NTT DATA](https://us.nttdata.com/en/services/digital-workplace-services/workplace-omnichannel-user-support)) ([Wipro](https://www.wipro.com/infrastructure/-live-workspace/)).

4. **Modelo phygital (físico + digital):** DXC, Kyndryl y Wipro coinciden en tech bars, kioscos, máquinas expendedoras de IT y smart lockers junto con los canales digitales ([DXC](https://dxc.com/solutions/modern-workplace/digital-support-services/service-desk)).

5. **De tickets a outcomes:** TCS propone precios outcome-based habilitados por GenAI; HCLTech pasa de "gestionar esfuerzo a orquestar outcomes" ([TCS](https://www.tcs.com/insights/blogs/generative-ai-outcome-based-pricing-models-service-desk)).

**3 estrategias de plataforma observadas:**
- (a) **Plataforma propietaria** como pilar: myWizard (Accenture), UPtime (DXC), HOLMES (Wipro), ignio/Cognix (TCS), Nucleus (NTT DATA), AI Force (HCLTech), PRiSM (Capgemini), IBM Consulting Advantage
- (b) **ISV especializado:** Bold360ai/LogMeIn (Cognizant), Espressive Barista (DXC), Interactions LLC (Kyndryl)
- (c) **ServiceNow como capa ITSM universal:** mencionado por DXC, Deloitte, Infosys, NTT DATA, HCLTech, IBM

---

## 4. Plataformas ITSM Líderes: Capacidades de IA y Automatización

### 4.1 Tabla Comparativa de las 6 Plataformas

| Plataforma | Posicionamiento | IA Nativa | Gartner MQ AI-ITSM | Precio Referencial |
|---|---|---|---|---|
| **ServiceNow** | Enterprise — líder absoluto (44.4% cuota entre top 10, [Apps Run The World](https://www.appsruntheworld.com/top-10-it-service-management-software-vendors-and-market-forecast/)) | Now Assist, AI Agents, Moveworks, AI Control Tower | **Único Líder 2025** | Tiers Foundation/Advanced/Prime |
| **BMC Helix** | Enterprise alta madurez + AIOps | HelixGPT con modelos de dominio | **Visionario 2025** | No público |
| **Ivanti Neurons** | Enterprise end-to-end + self-healing | Ivanti Neurons AI; 14 prácticas ITIL 4 + PinkVERIFY | Líder último MQ ITSM Tools (2023) | Premium / Enterprise Premium |
| **Atlassian JSM** | High-velocity / DevOps | Atlassian Intelligence + Rovo agents | **Nuevo ingreso 2025** | Desde ~$19/agente/mes |
| **Freshworks Freshservice** | Mid-market / consumer-grade | Freddy AI / Freddy Copilot | **Niche Player 2024–2025** | $19–$119/agente + $29 Freddy |
| **ManageEngine ServiceDesk Plus** | SMB / asset-centric | Zia + GenAI incluidos sin costo extra | **Niche Player 2025** (primer ingreso) | $13–$67/técnico/mes |

*(Fuentes: [Apps Run The World](https://www.appsruntheworld.com/top-10-it-service-management-software-vendors-and-market-forecast/), [ServiceNow](https://www.servicenow.com/products/itsm/pricing.html), [Synta](https://www.synta.pro/post/artificial-intelligence-in-itsm-key-takeaways-from-the-gartner-magic-quadrant-2024-2025))*


---

### Posicionamiento de Plataformas ITSM

![Posicionamiento Competitivo — Cuota de mercado y Gartner MQ 2025](https://d2z0o16i8xm8ak.cloudfront.net/d93eac35-3c61-4da0-96a8-ed5148a1ce99/e064ffeb-1124-4eba-b4f6-27b84d99dd8c/svg6_competidores.png?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiaHR0cHM6Ly9kMnowbzE2aTh4bThhay5jbG91ZGZyb250Lm5ldC9kOTNlYWMzNS0zYzYxLTRkYTAtOTZhOC1lZDUxNDhhMWNlOTkvZTA2NGZmZWItMTEyNC00ZWJhLWI0ZjYtMjdiODRkOTlkZDhjL3N2ZzZfY29tcGV0aWRvcmVzLnBuZz8qIiwiQ29uZGl0aW9uIjp7IkRhdGVMZXNzVGhhbiI6eyJBV1M6RXBvY2hUaW1lIjoxNzg0NjU1NDQ2fX19XX0_&Signature=lZUzMWQxUEgH-~tlhXIBol1DNPJeXoW725PBakpjt0JKG~kRfNjmJil7i5LLb0hBG9cAo6z-75oj9IyU4lDNoEisA-7mP8tzqhD1cz3HBLnkTlj0xNra44LnMvmOeNkURaJR7Qn~~W0XmdGb4TGtoXqsT6Lb~6Bjbm4Mqzju8ZFcOeIjDtDRJGKTFskU99vI7tMC2OOCljmmk6SchyoncawXR4g4ZwZltmtnSUIzi2iEgroOPRM2JC0hqCZdZD~jJ-G~xZNqN-JqOm895UVbwmLODRbiRV~SRFJ9bS9kXWERZ4t~eq4JnhD8v6~U1UOiVGouQou3q3BcBnFYPwxlzQ__&Key-Pair-Id=K1BF7XGXAIMYNX)

---



### 4.2 ServiceNow: El Estándar de Referencia

ServiceNow tiene el 44.4% de cuota entre los top 10 proveedores del mercado ITSM en 2024 y es el único Líder en el MQ de AI-ITSM 2025 ([Apps Run The World](https://www.appsruntheworld.com/top-10-it-service-management-software-vendors-and-market-forecast/)) ([DataLunix](https://www.datalunix.com/post/freshservice-magic-quadrant)). Su arquitectura de IA está organizada en tres niveles progresivos:

- **Foundation:** Agentes y skills de IA para soporte basado en tareas
- **Advanced:** Flujos agénticos que automatizan procesos complejos  
- **Prime:** AI Specialists que gestionan flujos de forma autónoma; incluye "L1 Service Desk AI Specialist" y "AI Agent for Digital End-User Experience (DEX)"

Su plataforma AIOps (**Predictive AIOps**) combina Event Management, Metric Intelligence y Health Log Analytics (HLA). HLA usa aprendizaje no supervisado para "predecir incidentes antes de que causen interrupciones" y ha permitido a clientes prevenir entre el **25% y el 35% de las interrupciones críticas P1** ([ServiceNow community](https://www.servicenow.com/community/itom-blog/servicenow-s-aiops-and-gartner-s-event-intelligence-solutions-a/ba-p/3208116)).

---

## 5. Benchmarks de Madurez y Métricas de la Industria

Estos benchmarks son el insumo crítico para el Framework de Assessment: permiten clasificar objetivamente cualquier mesa en su nivel de madurez.

| Métrica | Promedio Industria | World-Class / Best-in-Class | Fuente |
|---|---|---|---|
| **FCR (First Contact Resolution)** | 74% | ≥80% | [HDI/MetricNet](https://www.thinkhdi.com/~/media/HDICorp/Files/Library-Archive/Insider%20Articles/First%20Contact%20Resolution.pdf) *(SQM da 71%; HDI confirma 74%)* |
| **MTTR (Mean Time to Resolution)** | 8.85 horas | <4 horas (bueno) / <1 hora (world-class) | [MetricNet/HDI](https://www.thinkhdi.com/~/media/HDICorp/Files/Library-Archive/Insider%20Articles/mean-time-to-resolve.pdf) |
| **CSAT** | 73–86% (varía por período) | ≥90% | [HDI metrics](https://www.thinkhdi.com/library/supportworld/2023/metrics-matter-for-it-support/) / [HelpDeskFocus](https://www.helpdeskfocus.com/help-desk-metrics.html) |
| **AHT (Average Handle Time)** | 6–8 min (voz) | <7 min (voz world-class) | [IrisAgent](https://irisagent.com/customer-support-metrics/) / [HDI metrics](https://www.thinkhdi.com/library/supportworld/2023/metrics-matter-for-it-support/) |
| **Costo por ticket N0** | USD 2 | — | [Giva](https://www.givainc.com/blog/shift-left-analysis-how-to-guide-maximize-it-service-management-itsm-efficiency/) |
| **Costo por ticket N1** | USD 22–35 | USD 15–18 | [Kwestra](https://kwestra.com/insights/itsm-automation-roi/) |
| **Costo por ticket N3** | USD 104 | — | [Giva](https://www.givainc.com/blog/shift-left-analysis-how-to-guide-maximize-it-service-management-itsm-efficiency/) |
| **Deflection / Ticket deflection rate** | 23% | 40–60% (maduro) / 80–90% (casos líderes) | [servicedeskagents](https://servicedeskagents.com/deflection-rates/) / [Kwestra](https://kwestra.com/insights/itsm-automation-roi/) |
| **Impacto GenAI en tiempo de respuesta** | -26.6% (Freshservice); -17.8% (SolarWinds) | — | [Freshservice benchmark](https://freshservice.com/assets/resources/freshservice/freshservice-it-service-management-benchmark-report-2024.pdf) *(el -26.6% es mejora en first response time, no en MTTR)* |
| **Impacto KCS+IA en FCR** | +5–7 puntos | — | [SDI](https://www.servicedeskinstitute.com/resources/itsm-statistics-facts-and-trends-for-2024/) |
| **Impacto IA en CSAT** | +15–22 pts cuando espera < 5 min | — | [Stealth Agents](https://stealthagents.com/research/ai-it-helpdesk-automation-statistics-2026) |


---

### Visualización: Benchmarks Industria

![Benchmarks Industria — FCR, MTTR, Deflection, Impacto GenAI](https://d2z0o16i8xm8ak.cloudfront.net/d93eac35-3c61-4da0-96a8-ed5148a1ce99/5961b363-b8bc-437f-8074-c7663610bfd1/svg4_benchmarks.png?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiaHR0cHM6Ly9kMnowbzE2aTh4bThhay5jbG91ZGZyb250Lm5ldC9kOTNlYWMzNS0zYzYxLTRkYTAtOTZhOC1lZDUxNDhhMWNlOTkvNTk2MWIzNjMtYjhiYy00MzdmLTgwNzQtYzc2NjM2MTBiZmQxL3N2ZzRfYmVuY2htYXJrcy5wbmc~KiIsIkNvbmRpdGlvbiI6eyJEYXRlTGVzc1RoYW4iOnsiQVdTOkVwb2NoVGltZSI6MTc4NDY1NTQ0Nn19fV19&Signature=B0SRyNxAz3jSoZctxxWJk~EGtLOOyV~7BbVpouhV5hXtdwh5eNfDqMxETUrZ-VONf80cZcBysg9uX43WlsIVyup6AckaWLkIlOIL5wZ9KqRoA0pBk-~g5aCsKkVClYUwPl9BbXuCGQs7zznMAY2xO9YPBA1jtviOR1Ok3fch1GWUOAaBiQRVrbbnQifrBgYkGJDoklH1LHk5fctI4RyFwkVgBIeaXufkoiLD8FNxiOdsQsYrmbl02K5OsZN56dk4E4ITMe3r1nOytS28iOoosPfMgvp1yh9gp5s~nlMlWYDCTgtKXiZfVWBm0s-xUKWovQr9GEOf1cGkKyVRDd~k8Q__&Key-Pair-Id=K1BF7XGXAIMYNX)

---

### 5.1 SLA vs. XLA: La Nueva Dualidad de Medición


### SLA vs. XLA — Comparativa Visual y 4 Capas de Reporte

![SLA vs. XLA — Comparativa y 4 capas de reporte ejecutivo](https://d2z0o16i8xm8ak.cloudfront.net/d93eac35-3c61-4da0-96a8-ed5148a1ce99/a3ec1ac8-586a-4b64-a4c7-b84284b3c388/svg7_sla_xla.png?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiaHR0cHM6Ly9kMnowbzE2aTh4bThhay5jbG91ZGZyb250Lm5ldC9kOTNlYWMzNS0zYzYxLTRkYTAtOTZhOC1lZDUxNDhhMWNlOTkvYTNlYzFhYzgtNTg2YS00YjY0LWE0YzctYjg0Mjg0YjNjMzg4L3N2Zzdfc2xhX3hsYS5wbmc~KiIsIkNvbmRpdGlvbiI6eyJEYXRlTGVzc1RoYW4iOnsiQVdTOkVwb2NoVGltZSI6MTc4NDY1NTQ0Nn19fV19&Signature=polvzt47byB0nZupNmt~k7lLChcSzhk~GlHv1YEYesSPGUTbljNInS1SdE4SXJlmDXcRmqF2sOeZ9xp8WsQYpADa6W8WJYgWSRNHkEexbzwMkXf~S8PNYs44-PxYAVOu86iKGPDGVD71aEOQMgIVEzO4ZjbtlFOEjZAi2Omy4vh8C2zxu0Akf6WkfHVYhaZJ-b-jfzbyA4C0o9ai7gIObPeH6xPdS7QUAu9rpDFRx6v86u2Oj4vqT3Cf3KJzYM3ScuODv-523G4rqkaNzKHIug7ZveKNPjZavOMmWZRMQyMTeHyN6StFBRirw1wuvqMb5nymXfQ7XRkG-q6vS~tcHA__&Key-Pair-Id=K1BF7XGXAIMYNX)

---



### 5.2 XLA en la Práctica: Del Hype a la Madurez (2025-2026)

El primer reporte global del **XLA Institute, "State of XLA 2025"**, presentado el 12 de junio de 2025, marca la transición de las XLA desde el discurso experimental hacia la práctica escalable: **casi el 70% de las empresas encuestadas planea implementar XLAs en 2026** (el XLA Institute usa la expresión "casi 70%"; algunas referencias redondearon a 68%), y su adopción se expande rápidamente más allá de los departamentos de TI tradicionales hacia salud, RR.HH. y finanzas — con Brasil emergiendo como uno de los mercados líderes en gestión de experiencia ([EIN Presswire](https://www.einpresswire.com/article/823090394/xla-institute-releases-groundbreaking-state-of-xla-2025-report?code=9Hv3x5D-vwZo-peK)) ([Emerce](https://www.emerce.nl/wire/xla-institute-publiceert-state-xla-2025-rapport)).

El reporte introduce el **Dynamic Experience Management Framework (DEMF)**, que define dos ejes de madurez: madurez de capacidad y madurez de creación de valor acumulativo ("accretive value creation"). Entre sus hallazgos: las organizaciones exitosas construyen su gestión de experiencia alrededor de personas (personas-based), la Digital Employee Experience (DEX) y las XLA convergen para sostener tanto a empleados como resultados de negocio, y las XLA desplazan el foco de la resolución reactiva de problemas hacia la habilitación proactiva del éxito del usuario ([LinkedIn — Alan Nance, XLA Institute](https://www.linkedin.com/posts/alannance_get-your-copy-of-the-state-of-xla-2025-published-activity-7340670233575079936-XZ3Q)).

**El dashboard de 4 capas para reporte ejecutivo SLA/XLA**, propuesto por SMC Consulting, organiza las métricas de la siguiente manera:

| Capa | Métricas incluidas | Propósito |
|---|---|---|
| **1. Confiabilidad operacional** | Disponibilidad, cumplimiento de SLA, MTTR, incidentes mayores, tasa de éxito de cambios | Confirma si los servicios de TI son estables y predecibles |
| **2. Eficiencia del service desk** | Volumen de tickets, FCR, backlog, costo por ticket, adopción de autoservicio | Muestra si el soporte es eficiente y escalable |
| **3. Experiencia de usuario** | Satisfacción, effort score, sentimiento, experiencia por canal, experiencia del journey | Muestra si los usuarios tienen una experiencia positiva y de baja fricción |
| **4. Impacto de negocio** | Pérdida de productividad, impacto por unidad de negocio, exposición a riesgo, beneficios de mejora, evitación de costos, ROI | Conecta el desempeño de ITSM con el valor de negocio |

*(Fuente: [SMC Consulting](https://www.smcconsulting.be/news/sla-vs-xla-itsm-reporting))*

**El proceso de 8 pasos para la transición de SLA a XLA:**

1. Auditar las métricas actuales de SLA e ITSM: identificar qué se mide, quién usa cada reporte y qué decisión soporta cada métrica
2. Comparar el desempeño operacional con la satisfacción: buscar resultados de SLA en verde con baja satisfacción o alto esfuerzo
3. Definir las experiencias más importantes: comenzar por journeys como onboarding, solicitud de ayuda, solicitud de accesos, trabajo remoto y recuperación de incidentes mayores
4. Seleccionar medidas de XLA significativas: satisfacción, esfuerzo, tiempo a la productividad, adopción, sentimiento y confiabilidad percibida
5. Agregar mecanismos de feedback: encuestas cortas, encuestas de journey y análisis de texto libre
6. Integrar el reporte de experiencia al dashboard de KPI de ITSM, mostrando XLA junto a SLA
7. Alinear el reporte ejecutivo de ITSM con los resultados de negocio: liderar con salud del servicio, experiencia de usuario, riesgo e impacto de negocio
8. Revisar y refinar las métricas regularmente: retirar KPIs de bajo valor y ajustar umbrales conforme madura el modelo

*(Fuente: [SMC Consulting](https://www.smcconsulting.be/news/sla-vs-xla-itsm-reporting))*

**Herramientas del mercado:** Entre las plataformas especializadas en la medición de XLA y experiencia digital destacan **Nexthink**, que promueve explícitamente el tránsito "de SLA a XLA" mediante puntuaciones basadas en el sentimiento del usuario final y la salud del lugar de trabajo digital ([Nexthink](https://nexthink.com/resource/from-sla-to-xla-rethinking-end-user-kpis)), y **HappySignals**, ambas orientadas a conectar indicadores de experiencia, operacionales y técnicos en un único stack de medición.

---

## 6. Modelo de Madurez Propio: Mesa Gen Next

Con base en la evidencia de Gartner, ITIL (Version 5), HDI, Forrester y el análisis de los 12 grandes proveedores, se propone el siguiente **Modelo de Madurez para la Mesa de Servicios Gen Next**. Este modelo sintetiza los marcos de referencia de la industria y agrega dimensiones propias derivadas del análisis comparativo.

### 6.1 Los 5 Niveles de Madurez

| Nivel | Nombre | Descripción | Indicadores Clave |
|---|---|---|---|
| **Nivel 1** | **Reactivo** | La mesa responde a eventos cuando los usuarios los reportan. Sin proactividad, sin automatización significativa, sin gobierno formal. | FCR <65%; MTTR >12h; CSAT <70%; costo/ticket N1 >$40; deflection <10%; sin N0; sin catálogo formal |
| **Nivel 2** | **Estandarizado** | Procesos ITIL definidos. Catálogo de servicios. SLA formales. Base de conocimiento básica. CMDB en construcción. Medición de métricas operativas. | FCR 65–74%; MTTR 8–12h; CSAT 70–80%; catálogo publicado; SLA definidos; KPI reportados mensualmente |
| **Nivel 3** | **Proactivo** | Shift-left habilitado. N0 funcional. Automatización de tareas repetitivas. Gestión de problemas activa. Knowledge Management estructurado (KCS). Modelo de gobierno operativo. | FCR ≥75%; MTTR 4–8h; deflection 20–35%; autoservicio activo; KCS implementado; gobierno del servicio formal |
| **Nivel 4** | **Predictivo** | IA integrada. AIOps con detección de anomalías y correlación de incidentes. GenAI para agentes. XLA medidos junto a SLA. DEX monitoreado. Observabilidad activa. | FCR ≥80%; MTTR <4h; deflection 35–55%; CSAT ≥88%; XLA medidos; prevención de hasta 30% de P1 |
| **Nivel 5** | **Autónomo** | Agentes de IA que resuelven de extremo a extremo. Operación autónoma de infraestructura. Knowledge Hub con IA generativa. Remediación proactiva. Modelo económico basado en outcomes. | FCR ≥85%; MTTR <2h; deflection ≥55%; CSAT ≥92%; >50% incidentes resueltos sin agente humano; costo/ticket N0 dominante |


---

### Modelo de Madurez — Escalera Visual

![Modelo de Madurez Gen Next — 5 Niveles (escalera visual)](https://d2z0o16i8xm8ak.cloudfront.net/d93eac35-3c61-4da0-96a8-ed5148a1ce99/112f5b50-2a31-4452-8e67-0955a86dcb27/svg3_madurez.png?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiaHR0cHM6Ly9kMnowbzE2aTh4bThhay5jbG91ZGZyb250Lm5ldC9kOTNlYWMzNS0zYzYxLTRkYTAtOTZhOC1lZDUxNDhhMWNlOTkvMTEyZjViNTAtMmEzMS00NDUyLThlNjctMDk1NWE4NmRjYjI3L3N2ZzNfbWFkdXJlei5wbmc~KiIsIkNvbmRpdGlvbiI6eyJEYXRlTGVzc1RoYW4iOnsiQVdTOkVwb2NoVGltZSI6MTc4NDY1NTQ0Nn19fV19&Signature=kBmWT7MAOzy7Kg8xq7OJlBiKa9nLnzljUyNwa~AnunUDOUROJAlHgDPRKKi4efAKvYHbfTkDsNedH6aNC1k6WL7~54OhRa5M3TISHgQwciGPoU877WkQpaoRKypUp9NDHtO7WuPrPaPZvz-RuMF7tlj9b1Qi3afKmjlapM4nRg~wCViOLteeHFAsUkanmixx5uODlUD9ARizVx0pi1j37ebfu2TDYrMHqVHkf6xqQSE2tHF5~PvIMt1g6cPNdqLW9rHYzkEl5CNpqc9H66q7I9~x42y~x28Dt4tjWJNNciKXkJLHsW-0h5JCrOQ0xc1EPJIQpl~Ir-X1~1G-em0u6A__&Key-Pair-Id=K1BF7XGXAIMYNX)

---



### 6.2 Las 14 Dimensiones de Evaluación

El modelo Gen Next evalúa la madurez de una mesa en **14 dimensiones**, agrupadas en 4 ejes:

**Eje A — Modelo Operativo**
1. Estructura de niveles (N0–N3)
2. Modelo de gobierno del servicio
3. Catálogo de servicios
4. Modelo económico y costos

**Eje B — Inteligencia y Automatización**
5. Inteligencia Artificial (virtual agents, GenAI, agentic AI)
6. Automatización (workflows, self-healing, RPA)
7. AIOps y Observabilidad
8. Knowledge Hub (KCS + IA)

**Eje C — Experiencia y Medición**
9. Autoservicio (N0 / shift-left)
10. Métricas SLA + XLA
11. Digital Employee Experience (DEX)
12. Gestión de la Calidad (QA)

**Eje D — Evolución y Gobierno**
13. Roadmap de evolución continua
14. Modelo de transición y caracterización AS-IS

---

## 7. Framework de Assessment: Preguntas de Caracterización

Este framework permite clasificar cualquier mesa en los 5 niveles del modelo de madurez a través de preguntas estructuradas por dimensión.

### Eje A — Modelo Operativo

**A1. Estructura de Niveles**
- ¿La mesa tiene definidos formalmente los niveles de soporte (N1, N2, N3)?
- ¿Existe un Nivel 0 (N0) de autoservicio operativo con usuarios activos?
- ¿Los tickets se escalan con criterios definidos y RACI claro?
- ¿Cuál es el % de tickets resueltos en N1 sin escalar?

**A2. Modelo de Gobierno**
- ¿Existe un modelo de gobierno formal con comités, roles y responsabilidades definidas?
- ¿Se realizan revisiones periódicas de desempeño (service reviews) con el cliente?
- ¿Existe un proceso de mejora continua documentado y ejecutado?
- ¿Hay un owner del servicio con autoridad sobre cambios y prioridades?

**A3. Catálogo de Servicios**
- ¿La mesa tiene un catálogo de servicios publicado y accesible al usuario?
- ¿El catálogo diferencia entre servicios de soporte y servicios de solicitud?
- ¿Los tiempos de entrega (OLAs/SLAs) están definidos por ítem de catálogo?
- ¿El catálogo se actualiza periódicamente?

**A4. Modelo Económico**
- ¿Se conoce el costo por ticket por nivel (N0, N1, N2, N3)?
- ¿Existe un modelo de pricing del servicio (por usuario, por ticket, por outcome)?
- ¿Se mide el ROI de la automatización y la IA?
- ¿El modelo económico incentiva la deflección y el shift-left?

### Eje B — Inteligencia y Automatización

**B5. Inteligencia Artificial**
- ¿La mesa tiene un virtual agent o chatbot operativo con usuarios activos?
- ¿El virtual agent resuelve solicitudes de extremo a extremo o solo responde preguntas?
- ¿Se usa GenAI para asistir a los agentes (summarization, suggest resolution, draft response)?
- ¿Existe algún agente de IA autónomo (agentic AI) que tome decisiones sin aprobación humana?
- ¿La IA está conectada al Knowledge Hub como fuente de verdad?

**B6. Automatización**
- ¿Qué % de tickets se resuelven con cero intervención humana?
- ¿Existe automatización de tareas repetitivas (reset de contraseñas, aprovisionamiento, etc.)?
- ¿La mesa tiene capacidades de self-healing (auto-remediación de endpoints o infraestructura)?
- ¿Se usan workflows automatizados para gestión de solicitudes?
- ¿Existe RPA integrado con el service desk?

**B7. AIOps y Observabilidad**
- ¿La mesa está conectada a herramientas de monitoreo y observabilidad?
- ¿Existe correlación automática de alertas de infraestructura con incidentes del service desk?
- ¿La mesa puede detectar incidentes antes de que los usuarios los reporten?
- ¿Se usa análisis de logs, métricas y trazas para detección predictiva?
- ¿Cuál es el % de incidentes P1 prevenidos antes de impactar al usuario?

**B8. Knowledge Hub**
- ¿Existe una base de conocimiento activa con artículos vinculados a incidentes?
- ¿La creación de artículos sigue la metodología KCS?
- ¿La IA genera, valida o sugiere artículos de conocimiento automáticamente?
- ¿Cuál es el % de tickets vinculados a artículos de conocimiento?
- ¿Los usuarios pueden acceder al Knowledge Hub desde el portal de autoservicio?

### Eje C — Experiencia y Medición

**C9. Autoservicio (N0 / Shift-Left)**
- ¿La mesa tiene un portal de autoservicio con un catálogo navegable?
- ¿Los usuarios pueden resolver solicitudes comunes sin contactar a un agente?
- ¿Cuál es la tasa de deflección actual (% de contactos resueltos sin agente)?
- ¿El portal está integrado con el virtual agent para una experiencia conversacional?

**C10. Métricas SLA + XLA**
- ¿La mesa mide FCR, MTTR, CSAT y AHT de forma regular?
- ¿Los SLAs están definidos por tipo de ticket y criticidad?
- ¿Se miden XLAs (experiencia del empleado) además de SLAs operativos?
- ¿Los reportes se comparten proactivamente con los clientes en tiempo real?

**C11. Digital Employee Experience (DEX)**
- ¿Se mide la satisfacción del empleado con el servicio de TI de forma continua?
- ¿Existe monitoreo del rendimiento del endpoint desde la perspectiva del usuario?
- ¿Se correlaciona la experiencia del dispositivo con los tickets del service desk?
- ¿La mesa actúa sobre señales de DEX antes de que el usuario reporte un problema?

**C12. Gestión de Calidad**
- ¿Existe un proceso formal de QA de las interacciones del service desk?
- ¿Se auditan llamadas, chats o tickets con criterios definidos?
- ¿Las métricas de calidad se usan para planes de mejora de los agentes?

### Eje D — Evolución y Gobierno

**D13. Roadmap de Evolución**
- ¿La mesa tiene un roadmap de evolución formal con hitos y responsables?
- ¿El roadmap está alineado con la estrategia de TI de la organización?
- ¿Se revisa y actualiza el roadmap al menos anualmente?
- ¿Existe un backlog de mejoras priorizado?

**D14. Modelo de Transición**
- ¿Existe documentación del estado actual (AS-IS) de la mesa?
- ¿Se han identificado las brechas entre el estado actual y el estado deseado?
- ¿Existe un plan de transición con fases, costos y criterios de éxito?
- ¿Se ha definido un modelo de hypercare post-transición?

---

## 8. Cómo se Diferencia una Mesa Gen Next

Con base en el análisis comparativo del mercado, la oferta **Mesa de Servicios Gen Next** se diferencia en 6 dimensiones críticas:

| Dimensión | Mesa Tradicional (Nivel 1–2) | Mesa Gen Next (Nivel 4–5) |
|---|---|---|
| **Modelo operativo** | Reactivo; N1/N2/N3 con escalado manual | N0–N5; shift-left inteligente; escalado automático por IA |
| **Inteligencia** | Scripts de troubleshooting; FAQ estáticas | Virtual agent con GenAI; agentes autónomos; KCS+IA |
| **Automatización** | Workflows básicos; algunas automatizaciones | Self-healing, auto-remediación, >40% deflección |
| **Observabilidad** | Monitoreo de alertas; reacción a incidentes | AIOps predictivo; prevención de P1; correlación de causas raíz |
| **Medición de valor** | SLA de cumplimiento | SLA + XLA + DEX + impacto económico |
| **Evolución** | Estático; cambios reactivos | Roadmap vivo; evolución continua; backlog de mejoras |


---

### Agentic AI: Estado Real de Adopción 2025–2026

![Agentic AI — Estado de adopción 2025-2026 y casos de éxito](https://d2z0o16i8xm8ak.cloudfront.net/d93eac35-3c61-4da0-96a8-ed5148a1ce99/955a3847-9ef4-43e5-9040-5ca93869731c/svg8_agentic_ai.png?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiaHR0cHM6Ly9kMnowbzE2aTh4bThhay5jbG91ZGZyb250Lm5ldC9kOTNlYWMzNS0zYzYxLTRkYTAtOTZhOC1lZDUxNDhhMWNlOTkvOTU1YTM4NDctOWVmNC00M2U1LTkwNDAtNWNhOTM4Njk3MzFjL3N2ZzhfYWdlbnRpY19haS5wbmc~KiIsIkNvbmRpdGlvbiI6eyJEYXRlTGVzc1RoYW4iOnsiQVdTOkVwb2NoVGltZSI6MTc4NDY1NTQ0Nn19fV19&Signature=XU-7KC9dLFvpDjbBEzKIylvteuZnVm9-aHEQGvYowUQi8gSY4IB3qmMbWXc4RohIbReHlebAX6Sop1~PNh7OOgllCGZfOBeXWjHyhmPh0u5gR3h8-tEX1muQ~WyvmWVk75n6BotOpfChb45Wyk20cx7nSZEouIgKXNhAyZTBNNSvxny1QbzPvwLMPLo~WsZQnIFVIE2zC4zXAy8HtmRy30KN3QhPTZcsQdJPBcS3w2LOMUfdPRSfD5hA2xb1EfoXRSqhQtNZwgIzoUw97ZeOwrIjACJa18PXg9LKa6vfJ~09VOXN~dVX0LU-EFnKJBW8RMO-B0eRkH2hXKxlBuVtOg__&Key-Pair-Id=K1BF7XGXAIMYNX)

---


---

## 9. Tendencias Estratégicas 2024–2026

Las siguientes tendencias son las más relevantes para el diseño del portafolio Gen Next:

1. **GenAI como table stakes:** Los proveedores que no tienen GenAI quedan fuera de conversación. El impacto es medible: -26.6% en **tiempo de respuesta** (first response time) y +34.6% en **resoluciones más rápidas** ([Freshservice benchmark](https://freshservice.com/assets/resources/freshservice/freshservice-it-service-management-benchmark-report-2024.pdf)).

2. **Agentic AI como ventaja competitiva:** La distinción crítica: las herramientas anteriores respondían a *prompts*; los sistemas agénticos persiguen objetivos, mantienen memoria y ejecutan flujos multipaso ([Ivanti](https://www.ivanti.com/en-gb/blog/agentic-ai-it-service-autonomy)).

3. **KCS como prerrequisito para la IA:** "Los datos validados y demand-driven previenen alucinaciones y construyen confianza del usuario. KCS es un sistema operativo tanto para agentes humanos como de IA" ([Consortium for Service Innovation](https://www.serviceinnovation.org/kcs/)).

4. **Shift-left con datos:** El costo pasa de USD 104 (N3) a USD 2 (N0). Cada punto de deflección genera un ahorro cuantificable ([Giva](https://www.givainc.com/blog/shift-left-analysis-how-to-guide-maximize-it-service-management-itsm-efficiency/)).

5. **De SLA a outcomes:** TCS propone precios basados en outcomes; la industria migra de "gestionar esfuerzo" a "orquestar resultados" ([TCS](https://www.tcs.com/insights/blogs/generative-ai-outcome-based-pricing-models-service-desk)).

6. **Observabilidad como diferenciador:** La mesa que detecta y resuelve antes del reporte del usuario se vuelve invisible para el negocio — en el mejor sentido del término ([ServiceNow whitepaper](https://www.servicenow.com/content/dam/servicenow-assets/public/en-us/doc-type/resource-center/white-paper/the-essentials-of-predictive-aiops-and-visibility.pdf)).

7. **Agentic AI: del experimento a producción (con matices).** El año 2025-2026 confirma que la IA agéntica dejó de ser un experimento de laboratorio, pero la brecha entre adopción y madurez real sigue siendo amplia:

   | Indicador | Cifra | Fuente |
   |---|---|---|
   | Empresas con agentes de IA ya desplegados en alguna forma | 51% | [Brilo AI (vía G2/OneReach.ai)](https://www.brilo.ai/resources/agentic-ai-statistics) |
   | Empresas en producción plena (vs. experimentación) | 11% (frente a 79% aún en experimentación) | [Brilo AI (vía Digital Applied)](https://www.brilo.ai/resources/agentic-ai-statistics) |
   | Proyectos de IA agéntica cancelados hacia fin de 2027 | >40%, por costos, gobernanza o valor de negocio poco claro | [Gartner, vía Brilo AI](https://www.brilo.ai/resources/agentic-ai-statistics) |
   | Barreras principales para producción de IA agéntica | Seguridad/privacidad/cumplimiento (52%); complejidad técnica de gestión a escala (51%); falta de personal capacitado (44%) | [Dynatrace — Pulse of Agentic AI 2026](https://www.dynatrace.com/news/press-release/pulse-of-agentic-ai-2026/) |
   | Proyectos en producción para casos de uso limitados / adopción amplia por departamento / integración madura enterprise-wide | 50% / 44% / 23% | [Dynatrace — Pulse of Agentic AI 2026](https://www.dynatrace.com/news/press-release/pulse-of-agentic-ai-2026/) |

   Casos documentados de adopción en producción confirman el potencial cuando la implementación es madura: **Robinhood** desplegó agentes de IA sobre ServiceNow logrando un **70% de deflección de casos entre IT, HR y Legal, con 2.200+ horas de esfuerzo manual eliminadas cada mes** y 94% de satisfacción de empleados ([SaaS Intelligence / ServiceNow](https://saasintelligence.substack.com/p/servicenow-just-made-ai-free-and)); **Honeywell** logró una **reducción del ~80-85% en el volumen de tickets** entrantes tras introducir un copiloto de IA (Moveworks) para su help desk ([Moveworks AI Help Desk](https://www.moveworks.com/us/en/solutions/ai-help-desk)); y **Salesforce**, usando su propia plataforma Agentforce, resolvió de forma autónoma el **84% de 380.000 interacciones de soporte** en 90 días, con solo 2% de escalamiento a humanos ([Cloud Science Labs](https://www.cloudsciencelabs.com/blog/agentforce-roi-how-to-measure-the-business-impact-of-salesforce-ai-agents)) ([Salesforce Newsroom](https://www.salesforce.com/news/stories/agentforce-customer-support-lessons-learned/)).

   Los benchmarks de mercado para service desks con IA agéntica muestran mejoras sustanciales sobre el modelo tradicional: **FCR de 75-85% frente a 40-55% en desks tradicionales**, **reducción de MTTR de 60-70%**, y **costo por interacción de USD 3-8 frente a USD 15-25** en modelos gestionados por humanos ([CallSphere](https://callsphere.ai/blog/agentic-ai-service-desk-autonomous-it-ticket-resolution-2026)).

   Sin embargo, la gobernanza sigue siendo el eslabón más débil: solo una fracción de las organizaciones reporta contar con **gobernanza madura** de IA agéntica, y la mayoría **sigue verificando decisiones críticas con supervisión humana** — ServiceNow, por ejemplo, documenta explícitamente que su "agentic workforce" requiere "gobernanza fuerte, responsabilidades claramente definidas, seguimiento de desempeño y supervisión de gerentes humanos" como condición para escalar ([ServiceNow Newsroom](https://newsroom.servicenow.com/press-releases/details/2025/ServiceNow-Extends-End-to-End-AI-Agent-Orchestration-With-Agentic-Workforce-Management/default.aspx)).

8. **Pricing hacia outcomes: el modelo económico cambia.** La evolución del pricing en service desk documentada por TCS muestra una progresión clara de cuatro fases: **FTE-based** (finales de los 90s/inicios de los 2000, pago por disponibilidad de recursos sin incentivos de desempeño) → **ticket-based** (pago por esfuerzo real, pero con estructuras de tarifas complejas por tipo de ticket) → **modelo híbrido** (combinación de tarifa fija por usuario/aplicación y pricing por ticket, a fines de los 2010) → **outcome-based** (alineado con KPIs y SLAs definidos por el cliente, vinculado directamente a resultados de negocio como mejor servicio al cliente y mayor uptime) ([TCS](https://www.tcs.com/insights/blogs/generative-ai-outcome-based-pricing-models-service-desk)).

   La GenAI habilita este modelo mediante forecasting de demanda, facturación en tiempo real vinculada al consumo real, detección de anomalías en billing, y clasificación automática de complejidad de tickets para calibrar el pricing ([TCS](https://www.tcs.com/insights/blogs/generative-ai-outcome-based-pricing-models-service-desk)).

   **Benchmarks de ROI en automatización ITSM:** el caso defensible de IA en ITSM logra un **payback de 4 a 9 meses**, considerando presupuestar entre 30-50% por encima de la cotización del proveedor y un costo operativo continuo de 20-30% del costo de construcción por año ([Kwestra](https://kwestra.com/insights/itsm-automation-roi)). En paralelo, el mercado más amplio de proyectos de IA agéntica muestra que **la mayoría de proyectos enfrenta dificultades para demostrar ROI en el corto plazo. La industria de servicios de TI está migrando hacia contratos outcome-based de forma acelerada: TCS y Gartner documentan esta **migración gradual hacia modelos outcome-based**, y los modelos de **shared savings** —donde el proveedor y el cliente comparten entre 15% y 25% del ahorro generado por la automatización— ganan tracción como mecanismo de transición entre el pricing tradicional y el outcome puro ([Economic Times](https://economictimes.indiatimes.com/tech/information-tech/it-scrambles-for-benchmarks-as-clients-eye-outcome-based-deals/articleshow/124199042.cms)).

   La fórmula conceptual que sintetiza este modelo es simple pero exige datos maduros para calibrarse: **Costo del Servicio = Outcomes Logrados × Precio por Unidad de Outcome**, donde el "outcome" puede definirse como tickets resueltos con SLA cumplido, puntos de deflección alcanzados, o mejora medible en CSAT/XLA — desplazando el riesgo comercial del cliente hacia una responsabilidad compartida con el proveedor.

---

## 10. Conclusiones Estratégicas

El mercado converge hacia una realidad simple: **la mesa de servicio reactiva ya es indefendible comercialmente**. Los 12 grandes proveedores, las 6 plataformas ITSM líderes y los analistas de referencia (Gartner, Forrester, Everest, ISG) apuntan en la misma dirección: la mesa que no tiene IA, automatización y observabilidad está perdiendo en costo, en experiencia y en retención de clientes.

La oportunidad del proyecto **Mesa de Servicios Gen Next** es real y está bien fundada en evidencia:

- Gartner comoditizó las plataformas ITSM y trasladó el cuadrante a la IA — la diferenciación está en el framework de inteligencia y gobierno, no en el software base.
- Los grandes proveedores venden "AI-first" pero pocos tienen un **framework de assessment** que permita al cliente medir su madurez y entender dónde está parado.
- El modelo de madurez de 5 niveles propuesto en este documento, combinado con las 14 dimensiones de evaluación, ofrece un instrumento de caracterización que ninguno de los 12 grandes tiene publicado en formato de oferta comercial.
- Los benchmarks de FCR, MTTR, CSAT, deflección y costo por ticket son los criterios objetivos que permiten demostrar el valor diferencial de una Mesa Gen Next en cualquier conversación de preventa.
- La llegada de ITIL (Version 5) con su 6C AI Capability Model y el marco DPSM confirma que la gobernanza de IA ya no es opcional en el diseño de una mesa de servicios madura — es, junto con las XLA y el pricing outcome-based, uno de los tres pilares regulatorios y comerciales que definirán la próxima generación de contratos de servicio.

El siguiente paso natural — el **Assessment AS-IS** del roadmap de julio — tiene ahora una base de evidencia sólida, un modelo de madurez propio y un set de preguntas de caracterización listas para ser aplicadas.

Para el mercado colombiano y latinoamericano en particular, la oportunidad tiene una ventana temporal concreta: Colombia lidera la velocidad de crecimiento de servicios de TI en Sudamérica, el sector financiero ya opera con adopción de IA por encima del 80% en establecimientos de crédito, y el segmento de servicios ITSM (13.82% CAGR) crece más rápido que el de soluciones licenciadas — lo cual favorece directamente una oferta de consultoría y assessment como la que este estudio fundamenta, en un mercado donde Aranda Software es, hasta la fecha, el único competidor local de relevancia identificado frente a la oleada de plataformas globales que están expandiendo presencia formal en la región.

---

## 11. Mercado ITSM en Colombia y Latinoamérica

### 11.1 Tamaño de Mercado: Latam, Sudamérica y Colombia

| Alcance geográfico | Tamaño actual | Proyección | CAGR | Fuente |
|---|---|---|---|---|
| **América Latina (ITSM)** | USD 1.8 mil millones (2024) | USD 2.5 mil millones (2028) | 12% anual | [InvGate](https://blog.invgate.com/es/mercado-de-itsm-en-latam) |
| **Sudamérica (ITSM)** | USD 0.52 mil millones (2025) | USD 1.26 mil millones (2031) | 16.00% (2026-2031) | [Mordor Intelligence — South America ITSM Market](https://www.mordorintelligence.com/industry-reports/south-america-information-technology-service-management-itsm-market) |
| **Colombia (ITSM)** | USD 108.5 millones (2026) | USD 209.70 millones (2031) | 14.08% | [Mordor Intelligence — Colombia ITSM Market](https://www.mordorintelligence.com/industry-reports/colombia-information-technology-service-management-itsm-market) |
| **Colombia (IT Services, categoría amplia)** | — | — | 9.8% — el más rápido de Sudamérica | [Mordor Intelligence — South America ITSM Market](https://www.mordorintelligence.com/industry-reports/south-america-information-technology-service-management-itsm-market) |

El reporte de Mordor Intelligence sobre Sudamérica identifica a Colombia como un mercado secundario relevante en múltiples factores de crecimiento: digitalización empresarial en banca, retail y telecomunicaciones (junto a Brasil y Argentina); necesidad de experiencias de servicio en español y portugués; interés creciente en modelos de entrega centralizada de servicios para operaciones distribuidas; y expansión de modelos de soporte de TI tercerizado entre firmas medianas ([Mordor Intelligence — South America ITSM Market](https://www.mordorintelligence.com/industry-reports/south-america-information-technology-service-management-itsm-market)). El mismo reporte destaca que **"Colombia está recibiendo impulso desde la facturación electrónica, la actividad 5G y la presencia multinacional en Bogotá, lo que está elevando el interés en plataformas de servicio estructuradas"**.


---

### Oportunidad de Mercado: Colombia y Latinoamérica

![Oportunidad de Mercado — Colombia y Latinoamérica ITSM](https://d2z0o16i8xm8ak.cloudfront.net/d93eac35-3c61-4da0-96a8-ed5148a1ce99/c30880f8-19c2-4f0b-b5e9-c64b42cc6d05/svg9_colombia_latam.png?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiaHR0cHM6Ly9kMnowbzE2aTh4bThhay5jbG91ZGZyb250Lm5ldC9kOTNlYWMzNS0zYzYxLTRkYTAtOTZhOC1lZDUxNDhhMWNlOTkvYzMwODgwZjgtMTljMi00ZjBiLWI1ZTktYzY0YjQyY2M2ZDA1L3N2ZzlfY29sb21iaWFfbGF0YW0ucG5nPyoiLCJDb25kaXRpb24iOnsiRGF0ZUxlc3NUaGFuIjp7IkFXUzpFcG9jaFRpbWUiOjE3ODQ2NTU0NDZ9fX1dfQ__&Signature=XieN~TBohKykA6LQ4QB0~cdFJZ8nXKCLBpecQ7QJj~c9Eu3HS5w47y-VFZWANZ524c62PSLeZ9p3nL0KAuwbGhIgpLhEDv58~xLzDc2C0Ymi~68FkPoXab9SaoDDS4s7qNVw9fdQ0YZQ5y2fFS2X63xpQDG5Im4t~tS3w~cIZ7JT1c8zQ9MLEob0F60F3elFjeD2wkTG3bTlFrtXWaGYRZqXLTlxQi3azTS3e2cVIDhLAxCp7uRlrj2LoP6AJ3t4n2~WbLNhU-P~of3TDpIEdElRW0gEhR2lv20aK~QcRqxAGP2Cqg96XY9VuPgsbCCTkMR1ZReCH2~yqFq-3iXoHw__&Key-Pair-Id=K1BF7XGXAIMYNX)

---



### 11.2 Colombia ITSM: Composición del Mercado

| Segmento | Dato 2025/2026 | Detalle |
|---|---|---|
| **Cloud** | 63.45% de cuota | Modelo de despliegue dominante en el mercado colombiano |
| **Service Desk e Incident Management** | 27.09% de cuota | Mayor categoría funcional dentro del ITSM colombiano |
| **Knowledge Management** | 12.90% CAGR proyectado a 2031 | La categoría funcional de mayor crecimiento relativo |
| **Soluciones (software licenciado)** | 61.40% de cuota (2025) | Sigue siendo la mayor porción del mercado en términos absolutos |
| **Servicios (consultoría, implementación, gestión)** | 13.82% CAGR proyectado a 2031 | Crece más rápido que las soluciones — la oportunidad estructural para una oferta de servicios profesionales |

*(Fuente: [Mordor Intelligence — Colombia ITSM Market](https://www.mordorintelligence.com/industry-reports/colombia-information-technology-service-management-itsm-market))*

### 11.3 Competencia Local y Expansión de Plataformas Globales

**Competidores locales:** **Aranda Software** es, según Mordor Intelligence, el actor local más relevante del mercado colombiano de ITSM, combinando raíces locales con certificaciones formales de proceso: renovó en agosto de 2025 su certificación **PinkVerify** para 11 procesos ITSM, incorporando capacidades de automatización avanzada y prácticas asistidas por IA alineadas con los estándares globales de ITIL ([Mordor Intelligence — Colombia ITSM Market](https://www.mordorintelligence.com/industry-reports/colombia-information-technology-service-management-itsm-market)). **InvGate**, de origen argentino, también tiene presencia relevante en la región, con reconocimiento de Gartner como proveedor representativo en su Market Guide y presencia en más de 50 países ([InvGate](https://blog.invgate.com/es/mercado-de-itsm-en-latam)).

**Expansión de plataformas globales en la región:**

- **BMC Helix** estableció una entidad legal formal en Brasil en octubre de 2025, señal de inversión directa creciente de los grandes vendors globales en Sudamérica.
- **Ivanti** lanzó su producto Bpod en Sudamérica en junio de 2026, ampliando su huella comercial en la región.
- **ManageEngine** está duplicando su headcount en Brasil como parte de su estrategia de expansión regional.

*(Contexto de mercado, [Mordor Intelligence — South America ITSM Market](https://www.mordorintelligence.com/industry-reports/south-america-information-technology-service-management-itsm-market) y [Mordor Intelligence — Colombia ITSM Market](https://www.mordorintelligence.com/industry-reports/colombia-information-technology-service-management-itsm-market))*

Otros vendors globales con presencia activa en el mercado colombiano incluyen ServiceNow, Atlassian, Freshworks y ManageEngine, listados por Mordor Intelligence como líderes de la industria en Colombia, junto con perfiles de compañía adicionales como Zoho, Microsoft, Broadcom, OpenText, SolarWinds, SysAid, EasyVista, TeamDynamix, Halo Service Solutions, TOPdesk, Serviceaide, Alemba y Efecte ([Mordor Intelligence — Colombia ITSM Market](https://www.mordorintelligence.com/industry-reports/colombia-information-technology-service-management-itsm-market)).

### 11.4 Regulación Financiera Colombiana Relevante para ITSM

El sector financiero colombiano, regulado por la **Superintendencia Financiera de Colombia (SFC)**, impone requisitos que impactan directamente el diseño de mesas de servicio y operaciones de TI en bancos, aseguradoras y otras entidades vigiladas:

- **Circular Externa 007 (SFC):** Establece medidas mínimas para la administración del riesgo de ciberseguridad, exigiendo a las entidades vigiladas contar con un **Security Information and Event Management (SIEM)** para correlación de eventos, pruebas periódicas de planes de continuidad del negocio que simulen ciberataques, reporte de incidentes de ciberseguridad a la SFC y a las autoridades del modelo nacional de gestión de incidentes cibernéticos (con periodicidad de reporte de gestión al menos semestral), y procedimientos formales de respuesta y recuperación ante incidentes ([Circular 007 SFC, vía Scribd](https://es.scribd.com/document/478859956/Circular-007-SuperFinanciera)) ([Fundación Microfinanzas BBVA](https://www.fundacionmicrofinanzasbbva.org/revistaprogreso/instrucciones-entidades-vigiladas-ciberseguridad/)).

- **Open Finance — plazo regulatorio:** El régimen de transición para los estándares mínimos del sistema de finanzas abiertas ha sido ampliado sucesivamente por la SFC: la Circular Externa 009 de 2025 extendió el plazo hasta febrero de 2026, y la Circular Externa 001 de 2026 (emitida el 3 de febrero) lo amplió nuevamente hasta el **8 de agosto de 2026**, dando a las entidades vigiladas un margen adicional para completar las modificaciones técnicas en sus sistemas de información ([Holland & Knight](https://www.hklaw.com/en/insights/publications/2026/02/sfc-amplia-el-plazo-para-que-entidades-en-colombia-se-ajusten)) ([El Ecosistema Startup](https://ecosistemastartup.com/open-finance-colombia-2026-5-acciones-para-tu-fintech/)).

- **Adopción de IA en el sector financiero:** Según la propia SFC, en 2025 el **81% de los establecimientos de crédito colombianos ya utilizaba inteligencia artificial** en sus procesos, y el uso de canales digitales (Internet y aplicaciones móviles) pasó del **35.7% al 66.6% de las operaciones del sistema financiero entre 2021 y 2025** ([Superintendencia Financiera de Colombia](https://www.superfinanciera.gov.co/publicaciones/10116043/sistema-financiero-acelera-implementacion-de-canales-digitales/)).

Estas obligaciones regulatorias —SIEM, continuidad operativa, reporte de incidentes cibernéticos y cumplimiento de Open Finance— crean una demanda estructural de capacidades de observabilidad, gestión de incidentes de alta madurez y gobernanza de IA que una Mesa de Servicios Gen Next, alineada al modelo de madurez y al 6C AI Capability Model de ITIL (Version 5), está en posición de atender directamente.

### 11.5 Adopción de Agentic AI en Servicios Financieros y Seguros

Los datos de adopción de IA agéntica por industria muestran que los sectores regulados de BFSI (Banca, Servicios Financieros y Seguros) están entre los más activos, aunque todavía por debajo de sectores tecnológicos puros:

| Sector | Adopción Enterprise | Adopción Mid-Market | Adopción SMB | Promedio de Industria |
|---|---|---|---|---|
| **Servicios Financieros** | 29% | 22% | 13% | 22% |
| **Seguros** | 28% | 20% | 15% | 18% |

*(Fuente: [First Page Sage — Agentic AI Adoption Statistics 2026](https://firstpagesage.com/reports/agentic-ai-adoption-statistics/))*

Esta adopción, combinada con el 81% de penetración de IA general en establecimientos de crédito colombianos reportado por la SFC, sugiere que el sector financiero colombiano —a diferencia de otros verticales de la región— ya cuenta con la madurez digital y regulatoria necesaria para adoptar mesas de servicio de próxima generación con componentes agénticos, siempre que estas cumplan con los requisitos de gobernanza, trazabilidad y reporte de incidentes exigidos por la SFC.

### 11.6 Oportunidad para una Oferta de Professional Services (PS) en Colombia

El cruce de evidencia recolectada en esta sección configura una oportunidad de mercado concreta:

- **Colombia lidera la velocidad de crecimiento de IT Services en Sudamérica** (9.8% CAGR, el más alto de la región), lo cual valida una entrada temprana de una oferta diferenciada de mesa de servicios Gen Next ([Mordor Intelligence — South America ITSM Market](https://www.mordorintelligence.com/industry-reports/south-america-information-technology-service-management-itsm-market)).
- **La adopción de IA en banca colombiana ya es alta** (81% de establecimientos de crédito), lo que reduce la fricción de venta de soluciones con componentes de IA agéntica y AIOps en el sector financiero, uno de los verticales más exigentes en gobernanza ([SFC](https://www.superfinanciera.gov.co/publicaciones/10116043/sistema-financiero-acelera-implementacion-de-canales-digitales/)).
- **El mercado de servicios (13.82% CAGR) crece más rápido que el de soluciones licenciadas (61.4% de cuota pero menor crecimiento relativo)** en Colombia, lo que confirma que la demanda se está desplazando desde la compra de software hacia la contratación de consultoría, implementación y operación gestionada — exactamente el terreno donde compite una oferta de Assessment y Mesa Gen Next ([Mordor Intelligence — Colombia ITSM Market](https://www.mordorintelligence.com/industry-reports/colombia-information-technology-service-management-itsm-market)).
- **Aranda Software es, hasta la fecha, el único competidor local de relevancia identificado** con certificación formal (PinkVerify) y capacidades de IA — el resto del panorama competitivo está compuesto por plataformas globales (ServiceNow, Atlassian, BMC Helix, Ivanti, ManageEngine, Freshworks) que compiten principalmente como proveedores de software, no como integradores de assessment y transformación de madurez ([Mordor Intelligence — Colombia ITSM Market](https://www.mordorintelligence.com/industry-reports/colombia-information-technology-service-management-itsm-market)).
- La combinación de regulación exigente (Circular 007, Open Finance), presión de adopción de IA y un mercado de servicios en expansión acelerada crea una ventana comercial concreta para posicionar el Framework de Assessment y el Modelo de Madurez de 5 niveles descritos en este estudio como la oferta diferenciada frente a competidores que aún no publican metodologías de caracterización propias.

---

*Documento elaborado con base en fuentes primarias consultadas en julio de 2026: Gartner, PeopleCert/ITIL, HDI, Forrester, Everest Group, ISG, XLA Institute, Dynatrace, Mordor Intelligence, InvGate, Superintendencia Financiera de Colombia, y páginas oficiales de Accenture, IBM, Kyndryl, Deloitte, Capgemini, Cognizant, HCLTech, Infosys, TCS, NTT DATA, DXC y Wipro, así como ServiceNow, BMC, Ivanti, Atlassian, Freshworks, ManageEngine, Aranda Software, Salesforce y Robinhood.*