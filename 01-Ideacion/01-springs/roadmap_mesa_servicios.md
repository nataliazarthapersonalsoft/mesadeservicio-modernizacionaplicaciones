# Plan de diseño del servicio · Mesa de Servicios de Nueva Generación con IA
**PersonalSoft · Estrategia CTO / SICTO · Borrador para validación interna**

---

## Visión general del plan

El diseño del servicio se estructura en cuatro fases ejecutables en 3 meses, más una fase continua de transición de clientes actuales.

<svg width="100%" viewBox="0 0 680 140" xmlns="http://www.w3.org/2000/svg">
<defs>
<marker id="arr" viewBox="0 0 10 10" refX="8" refY="5" markerWidth="6" markerHeight="6" orient="auto-start-reverse">
<path d="M2 1L8 5L2 9" fill="none" stroke="context-stroke" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</marker>
</defs>
<rect x="10" y="20" width="140" height="90" rx="8" fill="#E6F1FB" stroke="#85B7EB" stroke-width="0.5"/>
<text x="80" y="44" text-anchor="middle" font-size="11" font-weight="500" fill="#0C447C" font-family="sans-serif">Fase 1</text>
<text x="80" y="60" text-anchor="middle" font-size="11" font-weight="500" fill="#0C447C" font-family="sans-serif">Ideación</text>
<text x="80" y="76" text-anchor="middle" font-size="9" fill="#185FA5" font-family="sans-serif">Semanas 1–3</text>
<text x="80" y="92" text-anchor="middle" font-size="9" fill="#185FA5" font-family="sans-serif">Conceptualizar</text>
<text x="80" y="106" text-anchor="middle" font-size="9" fill="#185FA5" font-family="sans-serif">y validar</text>
<line x1="150" y1="65" x2="172" y2="65" stroke="#B4B2A9" stroke-width="1" marker-end="url(#arr)"/>
<rect x="172" y="20" width="140" height="90" rx="8" fill="#EEEDFE" stroke="#AFA9EC" stroke-width="0.5"/>
<text x="242" y="44" text-anchor="middle" font-size="11" font-weight="500" fill="#3C3489" font-family="sans-serif">Fase 2</text>
<text x="242" y="60" text-anchor="middle" font-size="11" font-weight="500" fill="#3C3489" font-family="sans-serif">Ingeniería</text>
<text x="242" y="76" text-anchor="middle" font-size="9" fill="#534AB7" font-family="sans-serif">Semanas 4–8</text>
<text x="242" y="92" text-anchor="middle" font-size="9" fill="#534AB7" font-family="sans-serif">Diseñar y construir</text>
<text x="242" y="106" text-anchor="middle" font-size="9" fill="#534AB7" font-family="sans-serif">artefactos</text>
<line x1="312" y1="65" x2="334" y2="65" stroke="#B4B2A9" stroke-width="1" marker-end="url(#arr)"/>
<rect x="334" y="20" width="140" height="90" rx="8" fill="#E1F5EE" stroke="#1D9E75" stroke-width="0.5"/>
<text x="404" y="44" text-anchor="middle" font-size="11" font-weight="500" fill="#085041" font-family="sans-serif">Fase 3</text>
<text x="404" y="60" text-anchor="middle" font-size="11" font-weight="500" fill="#085041" font-family="sans-serif">Producción</text>
<text x="404" y="76" text-anchor="middle" font-size="9" fill="#0F6E56" font-family="sans-serif">Semanas 9–12</text>
<text x="404" y="92" text-anchor="middle" font-size="9" fill="#0F6E56" font-family="sans-serif">Lanzar · Alfa</text>
<text x="404" y="106" text-anchor="middle" font-size="9" fill="#0F6E56" font-family="sans-serif">y operar</text>
<line x1="474" y1="65" x2="496" y2="65" stroke="#D85A30" stroke-width="1" stroke-dasharray="4 2" marker-end="url(#arr)"/>
<rect x="496" y="20" width="174" height="90" rx="8" fill="#FAECE7" stroke="#F0997B" stroke-width="0.5" stroke-dasharray="4 2"/>
<text x="583" y="44" text-anchor="middle" font-size="11" font-weight="500" fill="#712B13" font-family="sans-serif">Fase 4</text>
<text x="583" y="60" text-anchor="middle" font-size="11" font-weight="500" fill="#712B13" font-family="sans-serif">Transición clientes</text>
<text x="583" y="76" text-anchor="middle" font-size="9" fill="#993C1D" font-family="sans-serif">Desde mes 2 · continua</text>
<text x="583" y="92" text-anchor="middle" font-size="9" fill="#993C1D" font-family="sans-serif">Migrar de staffing</text>
<text x="583" y="106" text-anchor="middle" font-size="9" fill="#993C1D" font-family="sans-serif">al nuevo modelo</text>
</svg>

---

## Glosario de términos clave

Antes de entrar al plan, definimos los términos técnicos que aparecen a lo largo del documento:

| Término | Qué significa en este contexto |
|---|---|
| **Triaje** (del francés *triage*) | Clasificación y priorización de un ticket en el momento en que llega: qué tan urgente es, a qué nivel va (N1, N2 o N3) y quién lo atiende primero |
| **N0, N1, N2, N3** | Niveles de atención del servicio: N0 = autoservicio sin humano, N1 = primer contacto humano, N2 = técnico especializado, N3 = experto de back-end |
| **SLA** (Service Level Agreement) | Acuerdo de niveles de servicio: los tiempos máximos pactados con el cliente para responder y resolver cada tipo de ticket |
| **KPI** (Key Performance Indicator) | Indicador clave de desempeño: la métrica que usamos para saber si el servicio está funcionando bien |
| **RACI** | Matriz de responsabilidades: quién hace (Responsible), quién aprueba (Accountable), quién es consultado (Consulted) y quién es informado (Informed) |
| **KEDB** (Known Error Database) | Base de datos de errores conocidos: repositorio de problemas frecuentes y sus soluciones, para que el equipo no tenga que reinventar la rueda |
| **AIOps** | Uso de inteligencia artificial para operar sistemas de TI: monitoreo predictivo, detección de anomalías, correlación de alertas antes de que se conviertan en incidentes |
| **Orquestador** | El agente de IA central que recibe el ticket, decide qué agentes activar y coordina la respuesta de todos |
| **Staffing / Staff augmentation** | Modelo anterior: PersonalSoft pone personas dentro del cliente, bajo metodología del cliente. El nuevo modelo es un servicio gestionado con metodología PS |
| **SOW** (Statement of Work) | Documento de alcance de trabajo: contrato operativo que define qué hace PS, bajo qué condiciones y a qué costo |
| **Slide deck** | Presentación en diapositivas (PowerPoint / Google Slides) para uso comercial o de capacitación |
| **Onboarding** | Proceso de arranque con un cliente nuevo: inducción, configuración de herramientas, transferencia de conocimiento |
| **Discovery** | Proceso de exploración dentro de un cliente para identificar nuevas oportunidades de servicio |

---

## Fase 1 · Ideación
**Semanas 1–3 · Objetivo:** Definir qué es el servicio, para quién es, cómo se diferencia y bajo qué condiciones se puede vender y operar.

### 1.1 Caracterización del servicio

> Definir con precisión qué es y qué no es la Mesa de Servicios de Nueva Generación, incluyendo sus características diferenciadoras frente a un modelo tradicional de staff augmentation.

| Artefacto | Descripción | Responsable |
|---|---|---|
| Ficha de caracterización del servicio | Nombre, propósito, value proposition, sectores objetivo, diferenciadores | CTO / SICTO |
| Detalle de características del servicio | IA integrada, base de conocimiento activa, reporting automático, herramienta estándar PS, modelo agnóstico por industria | CTO |
| Definición de sabores del servicio | Dedicado (100% al cliente), Compartido (capacidad entre varios clientes), Express / Alfa (piloto rápido) | CTO + Comercial |
| Mapa de alcance | Qué incluye el servicio, qué no incluye, qué se cobra aparte | CTO |
| Benchmark de mercado | Cómo lo hacen SURA, Bancolombia, competencia regional | SICTO |

### 1.2 Niveles de servicio

> Definir los cuatro niveles de atención del servicio con sus funciones, tipos de casos, perfiles técnicos y lenguajes/herramientas requeridos.

| Artefacto | Descripción | Responsable |
|---|---|---|
| Definición de niveles N0, N1, N2, N3 | Funciones, tipos de casos, perfiles, lenguajes por nivel | CTO |
| Matriz de escalamiento | Criterios y condiciones para pasar un ticket de un nivel al siguiente | CTO + Delivery |
| Diferenciación Mesa de Ayuda vs Mesa de Soporte | Tabla comparativa: nivel básico (reactivo) vs avanzado (reactivo y proactivo) | SICTO |
| Criterios de criticidad | Clasificación de tickets por impacto en el negocio y urgencia | CTO |

### 1.3 Roles y RACI inicial

> Definir quién hace qué dentro del servicio, tanto del lado de PersonalSoft como del lado del cliente.

| Artefacto | Descripción | Responsable |
|---|---|---|
| Mapa de roles del servicio | Gerente de mesa, líder técnico, analista N1, especialista N2, desarrollador N3, especialista IA | CTO |
| RACI por etapa del servicio | Quién hace, aprueba, consulta e informa en cada momento del ciclo | CTO + Delivery |
| Definición de perfiles de contratación | Skills, seniority y stack técnico requerido por nivel | A&S + CTO |

### 1.4 Arquitectura de IA y agentes

> Definir cómo la inteligencia artificial se integra al servicio: qué hace cada agente, cómo se coordinan y bajo qué principios de gobierno operan.

| Artefacto | Descripción | Responsable |
|---|---|---|
| Mapa de agentes de IA | Orquestador (clasificador y coordinador central) + agentes especializados: clasificación (triaje), diagnóstico, desarrollo, pruebas, monitoreo predictivo (AIOps), gestión de conocimiento | CTO |
| Principios de gobierno de IA | Human-in-the-loop (siempre hay un humano que supervisa), ISO 42000, trazabilidad de decisiones, gestión de riesgos | CTO |
| Capacidades IA por nivel | Qué hace la IA en N0 (respuesta automática), N1 (sugerencia de solución), N2 (análisis de causa raíz), N3 (asistencia en código) | CTO + SICTO |

### 1.5 Marco legal y contractual inicial

> Definir los aspectos legales que requiere el servicio para ser vendido y operado correctamente.

| Artefacto | Descripción | Responsable |
|---|---|---|
| Revisión del modelo contractual actual | ¿El contrato actual de staffing soporta el nuevo modelo o se necesita uno nuevo? | Legal + Comercial |
| Definición de acuerdos de confidencialidad (NDA) | Protección de información del cliente dentro de la mesa de servicios | Legal |
| Marco de protección de datos | Cómo se maneja la información del cliente en las herramientas y agentes de IA (especialmente en banca y seguros con regulación estricta) | Legal + CTO |
| Cláusulas de SLA y penalidades | Qué compromisos legales asume PS si no cumple los tiempos pactados | Legal + Comercial |
| Propiedad de la base de conocimiento | ¿A quién pertenece el conocimiento construido durante el servicio: al cliente o a PS? | Legal + CTO |
| Revisión de cumplimiento regulatorio por sector | Qué normas aplican en banca (SFC, Basilea) y seguros (regulación local) que impactan la operación de la mesa | Legal + CTO |

---

## Fase 2 · Ingeniería del servicio
**Semanas 4–8 · Objetivo:** Diseñar, documentar y construir todos los artefactos que hacen operable y vendible el servicio.

### 2.1 Catálogo de servicios

> El catálogo es el menú del servicio: qué módulos existen, qué incluye cada uno y bajo qué condiciones se entrega.

| Artefacto | Descripción | Responsable |
|---|---|---|
| Catálogo de servicios v1 | Módulos del servicio, descripción, entregables y SLA orientativo por módulo | CTO + Comercial |
| Ficha de cada módulo | Service Desk, Gestión de conocimiento, Monitoreo predictivo (AIOps), Gestión de incidentes, Reporting | CTO |
| Matriz de inclusión / exclusión por sabor | Qué está incluido en Dedicado vs Compartido vs Express (Alfa) | CTO + Comercial |

### 2.2 Modelo de estimación y calculadora

> Herramienta que permite calcular cuánto cuesta y cuántas personas se necesitan para operar la mesa de un cliente específico.

| Artefacto | Descripción | Responsable |
|---|---|---|
| Calculadora del servicio | Modelo en Excel / Sheets con los 9 criterios de estimación | CTO + Financiera |
| Parámetros base de la calculadora | Línea base histórica, % de tiempo muerto por persona (GAP), horas laborales reales, costo por ticket | CTO + Financiera |
| Plantilla de levantamiento de información | Documento que el comercial lleva al cliente para recoger los datos necesarios para estimar | Comercial + CTO |
| Modelo de pricing por sabor | Precio por persona (FTE), por ticket o modelo mixto, según el sabor del servicio | Comercial + Financiera |

### 2.3 Procesos del servicio

> Los procesos son el cómo: paso a paso de cómo opera la mesa desde que llega un ticket hasta que se cierra y se aprende de él.

| Artefacto | Descripción | Responsable |
|---|---|---|
| Proceso de clasificación y enrutamiento (triaje) | Flujo desde que llega el ticket hasta que se asigna al nivel correcto y a la persona correcta | CTO |
| Proceso de escalamiento | Criterios y pasos concretos para pasar un ticket de N1 a N2, y de N2 a N3 | CTO + Delivery |
| Proceso de cierre y validación | Confirmación con el usuario, registro en base de conocimiento, actualización del acuerdo de niveles de servicio | Delivery |
| Proceso de gestión de conocimiento | Cómo se crea, valida y publica un artículo en la base de conocimiento | CTO |
| Proceso de reporting mensual | Qué se mide, cómo se presenta, con qué frecuencia y quién lo aprueba | CTO + Delivery |
| Proceso de mejora continua | Retrospectivas, análisis de causa raíz, ajustes al servicio basados en datos | Delivery |

### 2.4 SLA y KPIs

> Los acuerdos de niveles de servicio (SLA) y los indicadores clave (KPI) son lo que permite medir si el servicio funciona bien y demostrárselo al cliente.

| Artefacto | Descripción | Responsable |
|---|---|---|
| Marco de SLA estándar | Tiempos máximos de respuesta y resolución por nivel de atención y prioridad del ticket | CTO |
| Plantilla de SLA por cliente | Documento negociable que se personaliza para cada cliente | Comercial + CTO |
| Dashboard de indicadores | Tiempo de respuesta, tiempo de resolución, satisfacción del cliente (CSAT), tickets por nivel, % de resolución automática con IA | CTO + Delivery |
| Modelo de penalidades | Qué sucede si PS no cumple el acuerdo de niveles de servicio pactado | Comercial + Legal |

### 2.5 Herramientas y plataforma

> Definir qué herramientas se usan para operar el servicio: para gestionar tickets, para construir la base de conocimiento y para conectar los agentes de IA.

| Artefacto | Descripción | Responsable |
|---|---|---|
| Evaluación de herramientas de tickets | Comparativo entre herramienta del cliente vs herramienta estándar PS (ServiceNow, Freshdesk, Jira Service Management, etc.) | CTO |
| Definición de herramienta estándar PS | La herramienta propia de PS que se usa cuando el cliente no tiene una definida | CTO |
| Arquitectura de base de conocimiento | Estructura del repositorio de errores conocidos (KEDB), niveles de acceso, integración con IA generativa | CTO |
| Integración de agentes de IA | Cómo se conecta la herramienta de tickets con el motor de IA para clasificación automática y sugerencia de soluciones | CTO |

### 2.6 Artefactos de venta (Comercial)

> Todo lo que el equipo comercial necesita para explicar, demostrar y cerrar el servicio con un cliente.

| Artefacto | Descripción | Responsable |
|---|---|---|
| Slide deck (presentación de venta) | Presentación en diapositivas para clientes: qué es el servicio, cómo funciona, qué lo diferencia, casos de referencia | Comercial + CTO |
| One-pager del servicio | Resumen de una sola página para dejar en reuniones o enviar por correo | Comercial |
| Propuesta comercial tipo (SOW) | Plantilla de documento de alcance de trabajo para la mesa de servicios | Comercial + Legal |
| FAQ de ventas | Preguntas frecuentes que el comercial debe poder responder sobre el servicio | Comercial + CTO |
| Comparativo competitivo | Cómo se diferencia PS de otros proveedores de mesa de servicios en el mercado | Comercial |
| Slide deck de capacitación a comerciales | Presentación interna para enseñarle al equipo comercial cómo vender el servicio | CTO + Comercial |

### 2.7 Artefactos de delivery

> Todo lo que el equipo que opera el servicio necesita para arrancar con un cliente, operarlo día a día y entregarlo con calidad.

| Artefacto | Descripción | Responsable |
|---|---|---|
| Playbook de operación | Manual completo de cómo operar la mesa día a día: procesos, herramientas, roles, escalamientos | CTO + Delivery |
| Plantilla de plan de arranque con cliente (onboarding) | Cómo arrancar con un cliente nuevo: qué se hace en la semana 1, 2, 3... | Delivery |
| Lista de chequeo de montaje del modelo | Lista de recursos necesarios para arrancar: personas, hardware, software, capacitaciones | Delivery |
| Plantilla de entregable mensual | Formato del reporte mensual que se le presenta al cliente con indicadores y novedades | Delivery |
| Plantilla de victorias tempranas | Reporte quincenal (cada 15 días) de avances concretos para el cliente | Delivery |
| Guía de gestión de escalamientos | Paso a paso de cómo manejar un incidente crítico: qué hacer, a quién llamar, qué comunicar | Delivery |

---

## Fase 3 · Producción (Versión Alfa)
**Semanas 9–12 · Objetivo:** Lanzar el servicio con el primer cliente, medir resultados y ajustar.

### 3.1 Habilitación y capacitación

> Preparar a las personas (comerciales, equipo de delivery, líderes) para vender y operar el servicio correctamente.

| Artefacto | Descripción | Responsable |
|---|---|---|
| Slide deck de habilitación comercial | Presentación para capacitar al equipo comercial: qué vender, cómo argumentarlo, cuánto vale | CTO + Comercial |
| Plan de inducción al equipo de delivery | Qué es el servicio, cómo opera, qué se espera de cada rol, herramientas que se usan | Delivery |
| Guía de herramientas | Cómo usar la herramienta de tickets, la base de conocimiento y los agentes de IA | CTO |
| Material de entrenamiento técnico por nivel | Contenido específico para analistas N1, especialistas N2 y desarrolladores N3 | CTO |
| Plan de certificación interna | Criterios para validar que el equipo está listo para operar antes de arrancar con el cliente | CTO + A&S |

### 3.2 Lanzamiento Alfa (1 julio)

> El momento de arrancar con el primer cliente piloto bajo el nuevo modelo de servicio.

| Artefacto | Descripción | Responsable |
|---|---|---|
| Plan de lanzamiento Alfa | Cronograma detallado, cliente piloto seleccionado, equipo asignado, criterios de éxito | CTO |
| Criterios de aceptación del piloto | Qué tiene que pasar (indicadores, tiempos, satisfacción) para considerar el piloto exitoso | CTO + Comercial |
| Acuerdo legal con cliente piloto | Contrato o adenda que formaliza el nuevo modelo de servicio con el cliente piloto | Legal + Comercial |
| Plan de comunicación interna | Cómo se comunica el lanzamiento del nuevo servicio a todo PersonalSoft | Comercial |

### 3.3 Operación y evolución continua

> Una vez lanzado el servicio, cómo se sostiene, mejora y crece en el tiempo.

| Artefacto | Descripción | Responsable |
|---|---|---|
| Ritual de seguimiento semanal | Reunión interna de revisión: operación, incidentes, bloqueos, mejoras | Delivery |
| Ritual de revisión mensual con cliente | Presentación del entregable mensual, indicadores, acuerdos para el siguiente mes | Delivery + Comercial |
| Proceso de identificación de nuevos servicios (discovery) | Cómo detectar oportunidades de servicios adicionales dentro del cliente (modernización, proyectos) | Comercial |
| Modelo de madurez del servicio | Cómo el servicio evoluciona de Alfa → Beta → Producción completa, con qué criterios se avanza | CTO |
| Roadmap del servicio | Qué capacidades y mejoras se incorporan en el tiempo: más IA, más automatización, nuevos niveles | CTO |

---

## Fase 4 · Transición de clientes actuales
**Desde mes 2 · Continua · Objetivo:** Migrar a los clientes que hoy operan bajo un modelo de staff augmentation al nuevo modelo de servicio gestionado.

> Esta fase corre en paralelo con las anteriores. No es un bloque separado en el tiempo — es una pista de trabajo que arranca en el mes 2 y continúa de forma progresiva cliente por cliente.

### 4.1 Diagnóstico de clientes actuales

| Artefacto | Descripción | Responsable |
|---|---|---|
| Mapa de clientes actuales con mesa | Inventario de todos los clientes que hoy tienen mesa: SURA, Bancolombia, XM, Centro América y otros | Comercial + Delivery |
| Ficha de diagnóstico por cliente | Cómo opera hoy cada mesa: herramienta, equipo, volumen de tickets, SLA actuales, nivel de madurez | Delivery |
| Clasificación por madurez | Qué tan listo está cada cliente para migrar: listo, en proceso, requiere trabajo previo | CTO + Comercial |

### 4.2 Modelo de transición

| Artefacto | Descripción | Responsable |
|---|---|---|
| Plantilla de plan de transición por cliente | Qué cambia, qué se mantiene, qué se agrega, cronograma de migración | Delivery + CTO |
| Guía de conversación con el cliente | Cómo presentarle al cliente el cambio de modelo sin que lo vea como un riesgo | Comercial |
| Propuesta de valor de la transición | Por qué le conviene al cliente migrar: más calidad, más visibilidad, IA incluida, mismo costo o mejor | Comercial + CTO |
| Acuerdo legal de transición | Adenda al contrato actual que formaliza el cambio de modelo y los nuevos compromisos | Legal + Comercial |

### 4.3 Clientes prioritarios para transición

| Cliente | Estado actual | Acción inmediata | Responsable |
|---|---|---|---|
| SURA (Tren 2) | Mesa operando bajo staffing | Reunión con Virginia Durango y Lina Vargas — ver operación 30 min y levantar diagnóstico | Comercial + Delivery |
| Bancolombia (CoEs) | Mesa más madura — tienen metodología propia | Ir a recoger su metodología, aprender de ellos y proponer mejora con IA | Comercial + CTO |
| XM | Mesa en operación | Contactar a Maritza y Paula Soto para diagnóstico | Comercial |
| Centro América | Soporte y mantenimiento con Yamis | Modelo de capacidad compartida — proponer servicio compartido con SLA | Comercial |
| Clientes nuevos | Sin mesa activa | Usar versión Express (Alfa) como puerta de entrada | Comercial |

### 4.4 Aspectos legales de la transición

| Artefacto | Descripción | Responsable |
|---|---|---|
| Revisión de contratos vigentes | ¿El contrato actual permite cambiar el modelo operativo sin renegociar? | Legal |
| Adenda de transición de modelo | Documento que actualiza el contrato: de staffing a servicio gestionado con SLA | Legal + Comercial |
| Definición de propiedad del conocimiento acumulado | El conocimiento construido hasta hoy en la mesa del cliente, ¿a quién pertenece al migrar? | Legal + CTO |
| Cláusulas de continuidad del servicio | Garantías de que la transición no interrumpe la operación del cliente | Legal + Delivery |

---

## Resumen de artefactos por destinatario

<svg width="100%" viewBox="0 0 680 230" xmlns="http://www.w3.org/2000/svg">
<rect x="10" y="10" width="153" height="210" rx="8" fill="#E6F1FB" stroke="#85B7EB" stroke-width="0.5"/>
<text x="87" y="32" text-anchor="middle" font-size="12" font-weight="500" fill="#0C447C" font-family="sans-serif">Comercial</text>
<line x1="18" y1="40" x2="155" y2="40" stroke="#85B7EB" stroke-width="0.5"/>
<text x="87" y="58" text-anchor="middle" font-size="10" fill="#185FA5" font-family="sans-serif">Slide deck de venta</text>
<text x="87" y="74" text-anchor="middle" font-size="10" fill="#185FA5" font-family="sans-serif">One-pager</text>
<text x="87" y="90" text-anchor="middle" font-size="10" fill="#185FA5" font-family="sans-serif">SOW tipo</text>
<text x="87" y="106" text-anchor="middle" font-size="10" fill="#185FA5" font-family="sans-serif">Calculadora</text>
<text x="87" y="122" text-anchor="middle" font-size="10" fill="#185FA5" font-family="sans-serif">FAQ ventas</text>
<text x="87" y="138" text-anchor="middle" font-size="10" fill="#185FA5" font-family="sans-serif">Comparativo</text>
<text x="87" y="154" text-anchor="middle" font-size="10" fill="#185FA5" font-family="sans-serif">Plantilla SLA</text>
<text x="87" y="170" text-anchor="middle" font-size="10" fill="#185FA5" font-family="sans-serif">Propuesta transición</text>
<text x="87" y="186" text-anchor="middle" font-size="10" fill="#185FA5" font-family="sans-serif">Guía conversación</text>
<text x="87" y="202" text-anchor="middle" font-size="10" fill="#185FA5" font-family="sans-serif">cliente</text>

<rect x="175" y="10" width="153" height="210" rx="8" fill="#EEEDFE" stroke="#AFA9EC" stroke-width="0.5"/>
<text x="252" y="32" text-anchor="middle" font-size="12" font-weight="500" fill="#3C3489" font-family="sans-serif">Delivery</text>
<line x1="183" y1="40" x2="320" y2="40" stroke="#AFA9EC" stroke-width="0.5"/>
<text x="252" y="58" text-anchor="middle" font-size="10" fill="#534AB7" font-family="sans-serif">Playbook de operación</text>
<text x="252" y="74" text-anchor="middle" font-size="10" fill="#534AB7" font-family="sans-serif">Plan de onboarding</text>
<text x="252" y="90" text-anchor="middle" font-size="10" fill="#534AB7" font-family="sans-serif">Checklist de montaje</text>
<text x="252" y="106" text-anchor="middle" font-size="10" fill="#534AB7" font-family="sans-serif">Entregable mensual</text>
<text x="252" y="122" text-anchor="middle" font-size="10" fill="#534AB7" font-family="sans-serif">Victorias tempranas</text>
<text x="252" y="138" text-anchor="middle" font-size="10" fill="#534AB7" font-family="sans-serif">Guía escalamientos</text>
<text x="252" y="154" text-anchor="middle" font-size="10" fill="#534AB7" font-family="sans-serif">Plan de inducción</text>
<text x="252" y="170" text-anchor="middle" font-size="10" fill="#534AB7" font-family="sans-serif">Ritual semanal</text>
<text x="252" y="186" text-anchor="middle" font-size="10" fill="#534AB7" font-family="sans-serif">Plan transición</text>
<text x="252" y="202" text-anchor="middle" font-size="10" fill="#534AB7" font-family="sans-serif">por cliente</text>

<rect x="340" y="10" width="153" height="210" rx="8" fill="#E1F5EE" stroke="#1D9E75" stroke-width="0.5"/>
<text x="417" y="32" text-anchor="middle" font-size="12" font-weight="500" fill="#085041" font-family="sans-serif">CTO / SICTO</text>
<line x1="348" y1="40" x2="485" y2="40" stroke="#1D9E75" stroke-width="0.5"/>
<text x="417" y="58" text-anchor="middle" font-size="10" fill="#0F6E56" font-family="sans-serif">Caracterización</text>
<text x="417" y="74" text-anchor="middle" font-size="10" fill="#0F6E56" font-family="sans-serif">Definición de niveles</text>
<text x="417" y="90" text-anchor="middle" font-size="10" fill="#0F6E56" font-family="sans-serif">RACI completo</text>
<text x="417" y="106" text-anchor="middle" font-size="10" fill="#0F6E56" font-family="sans-serif">Mapa de agentes IA</text>
<text x="417" y="122" text-anchor="middle" font-size="10" fill="#0F6E56" font-family="sans-serif">Catálogo de servicios</text>
<text x="417" y="138" text-anchor="middle" font-size="10" fill="#0F6E56" font-family="sans-serif">Marco SLA y KPIs</text>
<text x="417" y="154" text-anchor="middle" font-size="10" fill="#0F6E56" font-family="sans-serif">Arquitectura plataforma</text>
<text x="417" y="170" text-anchor="middle" font-size="10" fill="#0F6E56" font-family="sans-serif">Roadmap del servicio</text>
<text x="417" y="186" text-anchor="middle" font-size="10" fill="#0F6E56" font-family="sans-serif">Gobierno de IA</text>
<text x="417" y="202" text-anchor="middle" font-size="10" fill="#0F6E56" font-family="sans-serif">Modelo de madurez</text>

<rect x="505" y="10" width="163" height="210" rx="8" fill="#FAEEDA" stroke="#EF9F27" stroke-width="0.5"/>
<text x="587" y="32" text-anchor="middle" font-size="12" font-weight="500" fill="#633806" font-family="sans-serif">Legal</text>
<line x1="513" y1="40" x2="660" y2="40" stroke="#EF9F27" stroke-width="0.5"/>
<text x="587" y="58" text-anchor="middle" font-size="10" fill="#854F0B" font-family="sans-serif">Revisión contratos</text>
<text x="587" y="74" text-anchor="middle" font-size="10" fill="#854F0B" font-family="sans-serif">NDA actualizado</text>
<text x="587" y="90" text-anchor="middle" font-size="10" fill="#854F0B" font-family="sans-serif">Marco protección datos</text>
<text x="587" y="106" text-anchor="middle" font-size="10" fill="#854F0B" font-family="sans-serif">Cláusulas SLA</text>
<text x="587" y="122" text-anchor="middle" font-size="10" fill="#854F0B" font-family="sans-serif">Propiedad conocimiento</text>
<text x="587" y="138" text-anchor="middle" font-size="10" fill="#854F0B" font-family="sans-serif">Cumplimiento regulatorio</text>
<text x="587" y="154" text-anchor="middle" font-size="10" fill="#854F0B" font-family="sans-serif">SOW tipo</text>
<text x="587" y="170" text-anchor="middle" font-size="10" fill="#854F0B" font-family="sans-serif">Adenda de transición</text>
<text x="587" y="186" text-anchor="middle" font-size="10" fill="#854F0B" font-family="sans-serif">Continuidad servicio</text>
<text x="587" y="202" text-anchor="middle" font-size="10" fill="#854F0B" font-family="sans-serif">Penalidades</text>
</svg>

---

## Priorización para arrancar (versión Alfa · 1 julio)

Lo mínimo que debe estar listo antes del lanzamiento:

| Prioridad | Artefacto | Fase | Responsable |
|---|---|---|---|
| 🔴 Crítico | Caracterización y niveles del servicio | 1 | CTO |
| 🔴 Crítico | RACI y roles | 1 | CTO |
| 🔴 Crítico | Marco legal: revisión contratos y NDA | 1 | Legal |
| 🔴 Crítico | Calculadora de estimación | 2 | CTO + Financiera |
| 🔴 Crítico | Plantilla SOW / propuesta tipo | 2 | Comercial + Legal |
| 🔴 Crítico | Plan de onboarding para cliente piloto | 2 | Delivery |
| 🔴 Crítico | Slide deck de venta | 2 | Comercial + CTO |
| 🟡 Importante | Catálogo de servicios v1 | 2 | CTO |
| 🟡 Importante | Marco de SLA estándar | 2 | CTO |
| 🟡 Importante | Slide deck de capacitación a comerciales | 2 | CTO + Comercial |
| 🟡 Importante | Playbook de operación v1 | 2 | Delivery |
| 🟡 Importante | Diagnóstico de clientes actuales | 4 | Comercial + Delivery |
| 🟢 Puede esperar | Dashboard de KPIs | 3 | CTO + Delivery |
| 🟢 Puede esperar | Integración completa agentes IA | 3 | CTO |
| 🟢 Puede esperar | Modelo de madurez del servicio | 3 | CTO |

---

## Decisiones requeridas antes de avanzar

El equipo CTO / SICTO debe resolver estas preguntas antes de pasar a la fase de ingeniería:

1. **¿Qué cliente arranca el piloto el 1 de julio?** — SURA Tren 2, Bancolombia u otro
2. **¿Cuál es la herramienta estándar de PS?** — Definir cuál usamos cuando el cliente no tiene
3. **¿El N3 incluye soporte de infraestructura física?** — Discos, equipos, servidores físicos: ¿dentro o fuera del alcance?
4. **¿Quién es el Gerente de Mesa de Servicios?** — Rol crítico para arrancar el piloto
5. **¿La IA va desde el día 1 o se incorpora progresivamente?** — Impacta el costo y la propuesta comercial
6. **¿Cómo se cobra?** — Por persona (FTE), por ticket, modelo mixto o por nivel de servicio
7. **¿El conocimiento construido en la mesa pertenece al cliente o a PS?** — Decisión legal y comercial crítica
