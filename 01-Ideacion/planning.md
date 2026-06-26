# Plan de diseño del servicio · Mesa de Servicios de Nueva Generación con IA
**PersonalSoft · Estrategia CTO / SICTO · Borrador para validación interna**

---

## Visión general del plan

El diseño del servicio se estructura en tres grandes fases: **Ideación**, **Ingeniería del servicio** y **Producción**. Cada fase tiene entregables concretos tanto para equipos de delivery como para comerciales.

<svg width="100%" viewBox="0 0 680 120" xmlns="http://www.w3.org/2000/svg">
<defs>
<marker id="arr" viewBox="0 0 10 10" refX="8" refY="5" markerWidth="6" markerHeight="6" orient="auto-start-reverse">
<path d="M2 1L8 5L2 9" fill="none" stroke="context-stroke" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</marker>
</defs>
<rect x="20" y="20" width="180" height="80" rx="8" fill="#E6F1FB" stroke="#85B7EB" stroke-width="0.5"/>
<text x="110" y="52" text-anchor="middle" font-size="13" font-weight="500" fill="#0C447C" font-family="sans-serif">Fase 1</text>
<text x="110" y="70" text-anchor="middle" font-size="12" font-weight="500" fill="#0C447C" font-family="sans-serif">Ideación</text>
<text x="110" y="88" text-anchor="middle" font-size="10" fill="#185FA5" font-family="sans-serif">Conceptualizar y validar</text>
<line x1="200" y1="60" x2="240" y2="60" stroke="#B4B2A9" stroke-width="1" marker-end="url(#arr)"/>
<rect x="240" y="20" width="200" height="80" rx="8" fill="#EEEDFE" stroke="#AFA9EC" stroke-width="0.5"/>
<text x="340" y="52" text-anchor="middle" font-size="13" font-weight="500" fill="#3C3489" font-family="sans-serif">Fase 2</text>
<text x="340" y="70" text-anchor="middle" font-size="12" font-weight="500" fill="#3C3489" font-family="sans-serif">Ingeniería del servicio</text>
<text x="340" y="88" text-anchor="middle" font-size="10" fill="#534AB7" font-family="sans-serif">Diseñar y construir artefactos</text>
<line x1="440" y1="60" x2="480" y2="60" stroke="#B4B2A9" stroke-width="1" marker-end="url(#arr)"/>
<rect x="480" y="20" width="180" height="80" rx="8" fill="#E1F5EE" stroke="#1D9E75" stroke-width="0.5"/>
<text x="570" y="52" text-anchor="middle" font-size="13" font-weight="500" fill="#085041" font-family="sans-serif">Fase 3</text>
<text x="570" y="70" text-anchor="middle" font-size="12" font-weight="500" fill="#085041" font-family="sans-serif">Producción</text>
<text x="570" y="88" text-anchor="middle" font-size="10" fill="#0F6E56" font-family="sans-serif">Lanzar, operar y evolucionar</text>
</svg>

---

## Fase 1 · Ideación

**Objetivo:** Definir qué es el servicio, para quién es, cómo se diferencia y bajo qué condiciones se puede vender y operar.

**Duración estimada:** 3–4 semanas

### 1.1 Caracterización del servicio

Definir con precisión qué es y qué no es la Mesa de Servicios de Nueva Generación.

| Artefacto | Descripción | Responsable |
|---|---|---|
| Ficha de caracterización del servicio | Nombre, propósito, value proposition, sectores objetivo, diferenciadores | CTO / SICTO |
| Definición de sabores del servicio | Dedicado, compartido, Express (Alfa) | CTO + Comercial |
| Mapa de alcance (qué incluye / qué no) | Límites del servicio por nivel y tipo de cliente | CTO |
| Benchmark de mercado | Cómo lo hacen SURA, Bancolombia, competencia | SICTO |

### 1.2 Niveles de servicio (Service Levels)

| Artefacto | Descripción | Responsable |
|---|---|---|
| Definición de niveles N0, N1, N2, N3 | Funciones, tipos de casos, perfiles, lenguajes | CTO |
| Matriz de escalamiento | Criterios y condiciones para escalar entre niveles | CTO + Delivery |
| Diferenciación Mesa de Ayuda vs Mesa de Soporte | Tabla comparativa para uso comercial e interno | SICTO |
| Criterios de criticidad | Clasificación de tickets por impacto y urgencia | CTO |

### 1.3 Modelo de roles (RACI inicial)

| Artefacto | Descripción | Responsable |
|---|---|---|
| Mapa de roles del servicio | Gerente de mesa, líder técnico, analista N1, especialista N2, desarrollador N3, especialista IA | CTO |
| RACI por etapa del servicio | Quién hace, aprueba, consulta e informa en cada momento | CTO + Delivery |
| Definición de perfiles de contratación | Skills, seniority, stack técnico por nivel | A&S + CTO |

### 1.4 Arquitectura agéntica (IA)

| Artefacto | Descripción | Responsable |
|---|---|---|
| Mapa de agentes de IA | Orquestador + agentes especializados (triaje, diagnóstico, desarrollo, testing, AIOps, conocimiento) | CTO |
| Principios de gobierno de IA | Human-in-the-loop, ISO 42000, trazabilidad, gestión de riesgos | CTO |
| Definición de capacidades IA por nivel | Qué hace la IA en N0, N1, N2, N3 | CTO + SICTO |

### 1.5 Estrategia comercial inicial

| Artefacto | Descripción | Responsable |
|---|---|---|
| Propuesta de valor (pitch de una página) | Para uso comercial: qué es, qué resuelve, qué diferencia | Comercial + CTO |
| Identificación de clientes piloto | SURA, Bancolombia, XM, Centro América | Comercial |
| Modelo de transición de clientes actuales | Cómo migrar de staff augmentation al nuevo servicio | CTO + Comercial |

---

## Fase 2 · Ingeniería del servicio

**Objetivo:** Diseñar, documentar y construir todos los artefactos que hacen operable y vendible el servicio.

**Duración estimada:** 6–8 semanas

### 2.1 Catálogo de servicios

| Artefacto | Descripción | Responsable |
|---|---|---|
| Catálogo de servicios v1 | Módulos del servicio, descripción, entregables, SLA orientativo | CTO + Comercial |
| Ficha de cada módulo | Service Desk, Gestión de conocimiento, AIOps, Gestión de incidentes, Reporting | CTO |
| Matriz de inclusión / exclusión por sabor | Qué está incluido en dedicado vs compartido vs Express | CTO + Comercial |

### 2.2 Modelo de estimación y calculadora

| Artefacto | Descripción | Responsable |
|---|---|---|
| Calculadora del servicio | Modelo en Excel/Sheets con los 9 criterios de estimación | CTO + Financiera |
| Parámetros base | Línea base, % GAP tiempo muerto por FTE, horas laborales, monetización por ticket | CTO + Financiera |
| Plantilla de preventa | Documento de recolección de información del cliente para estimar | Comercial + CTO |
| Modelo de pricing por sabor | Precio por FTE, por ticket, por nivel | Comercial + Financiera |

### 2.3 Procesos del servicio

| Artefacto | Descripción | Responsable |
|---|---|---|
| Proceso de intake y triaje | Flujo desde que llega el ticket hasta que se asigna | CTO |
| Proceso de escalamiento | Criterios y pasos para escalar N1→N2→N3 | CTO + Delivery |
| Proceso de cierre y validación | Confirmación con el usuario, registro en KB, actualización SLA | Delivery |
| Proceso de gestión de conocimiento | Cómo se crea, valida y publica en la base de conocimiento | CTO |
| Proceso de reporting mensual | Qué se mide, cómo se presenta, con qué frecuencia | CTO + Delivery |
| Proceso de mejora continua | Retrospectivas, análisis de causa raíz, ajustes al servicio | Delivery |

### 2.4 SLA y KPIs

| Artefacto | Descripción | Responsable |
|---|---|---|
| Marco de SLA estándar | Tiempos de respuesta y resolución por nivel y prioridad | CTO |
| Plantilla de SLA por cliente | Documento negociable con el cliente | Comercial + CTO |
| Dashboard de KPIs | Tiempo de respuesta, resolución, CSAT, tickets por nivel, % automatización | CTO + Delivery |
| Modelo de penalidades | Qué pasa si no se cumple el SLA pactado | Comercial + Financiera |

### 2.5 Herramientas

| Artefacto | Descripción | Responsable |
|---|---|---|
| Evaluación de herramientas de tickets | Comparativo: herramienta del cliente vs herramienta estándar PS | CTO |
| Definición de herramienta estándar PS | La herramienta propia de PS como respaldo y estándar mínimo | CTO |
| Arquitectura de base de conocimiento | Estructura del KEDB, niveles de acceso, integración con IA | CTO |
| Integración con agentes de IA | Cómo se conecta la herramienta con el motor de IA | CTO |

### 2.6 Artefactos de venta (Comercial)

| Artefacto | Descripción | Responsable |
|---|---|---|
| Deck de venta del servicio | Presentación para clientes: qué es, cómo funciona, casos de éxito | Comercial + CTO |
| One-pager del servicio | Resumen de una página para dejar en reuniones | Comercial |
| Propuesta comercial tipo (SOW) | Plantilla de Statement of Work para la mesa de servicios | Comercial + Legal |
| FAQ de ventas | Preguntas frecuentes que el comercial debe poder responder | Comercial + CTO |
| Comparativo competitivo | Cómo se diferencia PS de otros proveedores de mesa de servicios | Comercial |

### 2.7 Artefactos de delivery

| Artefacto | Descripción | Responsable |
|---|---|---|
| Playbook de operación | Manual de cómo operar la mesa día a día | CTO + Delivery |
| Plantilla de plan de transición | Cómo arrancar con un cliente nuevo (onboarding) | Delivery |
| Checklist de montaje del modelo | Lista de recursos para operar: personas, HW, SW, capacitaciones | Delivery |
| Plantilla de entregable mensual | Formato del reporte mensual al cliente | Delivery |
| Plantilla de victorias tempranas | Reporte de avances cada 15 días | Delivery |
| Guía de gestión de escalamientos | Cómo manejar un incidente crítico paso a paso | Delivery |

---

## Fase 3 · Producción

**Objetivo:** Lanzar el servicio, operar los primeros clientes, medir y evolucionar.

**Duración estimada:** Continua desde julio 2025

### 3.1 Habilitación y capacitación

| Artefacto | Descripción | Responsable |
|---|---|---|
| Plan de capacitación a comerciales | Cómo vender la mesa, preguntas frecuentes, casos de uso | CTO + Comercial |
| Plan de inducción al equipo de delivery | Qué es el servicio, cómo opera, qué se espera de cada rol | Delivery |
| Guía de herramientas | Cómo usar la herramienta de tickets, la base de conocimiento y los agentes IA | CTO |
| Material de entrenamiento técnico por nivel | Contenido específico para N1, N2 y N3 | CTO |
| Plan de certificación interna | Criterios para validar que el equipo está listo para operar | CTO + A&S |

### 3.2 Lanzamiento (versión Alfa)

| Artefacto | Descripción | Responsable |
|---|---|---|
| Plan de lanzamiento Alfa (1 julio) | Cronograma, cliente piloto, equipo asignado, criterios de éxito | CTO |
| Criterios de aceptación del piloto | Qué tiene que pasar para considerar el piloto exitoso | CTO + Comercial |
| Plan de comunicación interna | Cómo se comunica el lanzamiento a todo PersonalSoft | Comercial |
| Acuerdo legal con cliente piloto | Contrato o adenda que formaliza el nuevo modelo de servicio | Legal + Comercial |

### 3.3 Operación y evolución

| Artefacto | Descripción | Responsable |
|---|---|---|
| Ritual de seguimiento semanal | Reunión interna de revisión del servicio (operación, incidentes, mejoras) | Delivery |
| Ritual de revisión mensual con cliente | Presentación del entregable mensual, KPIs, acuerdos | Delivery + Comercial |
| Proceso de discovery de nuevos servicios | Cómo identificar oportunidades de servicios adicionales dentro del cliente | Comercial |
| Modelo de madurez del servicio | Cómo el servicio evoluciona de Alfa → Beta → Producción completa | CTO |
| Roadmap del servicio | Qué capacidades y mejoras se incorporan en el tiempo | CTO |

---

## Resumen de artefactos por destinatario

<svg width="100%" viewBox="0 0 680 200" xmlns="http://www.w3.org/2000/svg">
<rect x="20" y="10" width="195" height="180" rx="8" fill="#E6F1FB" stroke="#85B7EB" stroke-width="0.5"/>
<text x="117" y="32" text-anchor="middle" font-size="12" font-weight="500" fill="#0C447C" font-family="sans-serif">Comercial</text>
<line x1="28" y1="40" x2="207" y2="40" stroke="#85B7EB" stroke-width="0.5"/>
<text x="117" y="58" text-anchor="middle" font-size="10" fill="#185FA5" font-family="sans-serif">Deck de venta</text>
<text x="117" y="74" text-anchor="middle" font-size="10" fill="#185FA5" font-family="sans-serif">One-pager</text>
<text x="117" y="90" text-anchor="middle" font-size="10" fill="#185FA5" font-family="sans-serif">SOW / Propuesta tipo</text>
<text x="117" y="106" text-anchor="middle" font-size="10" fill="#185FA5" font-family="sans-serif">Calculadora de estimación</text>
<text x="117" y="122" text-anchor="middle" font-size="10" fill="#185FA5" font-family="sans-serif">FAQ de ventas</text>
<text x="117" y="138" text-anchor="middle" font-size="10" fill="#185FA5" font-family="sans-serif">Comparativo competitivo</text>
<text x="117" y="154" text-anchor="middle" font-size="10" fill="#185FA5" font-family="sans-serif">Plantilla SLA por cliente</text>
<text x="117" y="170" text-anchor="middle" font-size="10" fill="#185FA5" font-family="sans-serif">Plan de comunicación</text>

<rect x="243" y="10" width="195" height="180" rx="8" fill="#EEEDFE" stroke="#AFA9EC" stroke-width="0.5"/>
<text x="340" y="32" text-anchor="middle" font-size="12" font-weight="500" fill="#3C3489" font-family="sans-serif">Delivery</text>
<line x1="251" y1="40" x2="430" y2="40" stroke="#AFA9EC" stroke-width="0.5"/>
<text x="340" y="58" text-anchor="middle" font-size="10" fill="#534AB7" font-family="sans-serif">Playbook de operación</text>
<text x="340" y="74" text-anchor="middle" font-size="10" fill="#534AB7" font-family="sans-serif">Plan de transición</text>
<text x="340" y="90" text-anchor="middle" font-size="10" fill="#534AB7" font-family="sans-serif">Checklist de montaje</text>
<text x="340" y="106" text-anchor="middle" font-size="10" fill="#534AB7" font-family="sans-serif">Entregable mensual</text>
<text x="340" y="122" text-anchor="middle" font-size="10" fill="#534AB7" font-family="sans-serif">Victorias tempranas</text>
<text x="340" y="138" text-anchor="middle" font-size="10" fill="#534AB7" font-family="sans-serif">Guía de escalamientos</text>
<text x="340" y="154" text-anchor="middle" font-size="10" fill="#534AB7" font-family="sans-serif">Plan de inducción</text>
<text x="340" y="170" text-anchor="middle" font-size="10" fill="#534AB7" font-family="sans-serif">Ritual semanal / mensual</text>

<rect x="466" y="10" width="195" height="180" rx="8" fill="#E1F5EE" stroke="#1D9E75" stroke-width="0.5"/>
<text x="563" y="32" text-anchor="middle" font-size="12" font-weight="500" fill="#085041" font-family="sans-serif">CTO / SICTO</text>
<line x1="474" y1="40" x2="653" y2="40" stroke="#1D9E75" stroke-width="0.5"/>
<text x="563" y="58" text-anchor="middle" font-size="10" fill="#0F6E56" font-family="sans-serif">Caracterización del servicio</text>
<text x="563" y="74" text-anchor="middle" font-size="10" fill="#0F6E56" font-family="sans-serif">Definición de niveles</text>
<text x="563" y="90" text-anchor="middle" font-size="10" fill="#0F6E56" font-family="sans-serif">RACI completo</text>
<text x="563" y="106" text-anchor="middle" font-size="10" fill="#0F6E56" font-family="sans-serif">Mapa de agentes IA</text>
<text x="563" y="122" text-anchor="middle" font-size="10" fill="#0F6E56" font-family="sans-serif">Catálogo de servicios</text>
<text x="563" y="138" text-anchor="middle" font-size="10" fill="#0F6E56" font-family="sans-serif">Marco de SLA y KPIs</text>
<text x="563" y="154" text-anchor="middle" font-size="10" fill="#0F6E56" font-family="sans-serif">Arquitectura herramientas</text>
<text x="563" y="170" text-anchor="middle" font-size="10" fill="#0F6E56" font-family="sans-serif">Roadmap del servicio</text>
</svg>

---

## Priorización para arrancar (versión Alfa · 1 julio)

Lo mínimo que debe estar listo antes del lanzamiento:

| Prioridad | Artefacto | Estado |
|---|---|---|
| 🔴 Crítico | Caracterización y niveles del servicio | Por construir |
| 🔴 Crítico | RACI y roles | Por construir |
| 🔴 Crítico | Calculadora de estimación | Por construir |
| 🔴 Crítico | Plantilla SOW / propuesta tipo | Por construir |
| 🔴 Crítico | Plan de transición para cliente piloto | Por construir |
| 🟡 Importante | Catálogo de servicios v1 | Por construir |
| 🟡 Importante | Deck de venta | Por construir |
| 🟡 Importante | Marco de SLA estándar | Por construir |
| 🟡 Importante | Plan de capacitación a comerciales | Por construir |
| 🟢 Puede esperar | Dashboard de KPIs | Fase posterior |
| 🟢 Puede esperar | Modelo de madurez del servicio | Fase posterior |
| 🟢 Puede esperar | Integración completa agentes IA | Fase posterior |

---

## Próximas decisiones requeridas

Antes de avanzar en la ingeniería del servicio, el equipo CTO / SICTO debe resolver:

1. **¿Qué cliente piloto arranca el 1 de julio?** — SURA Tren 2, Bancolombia o uno nuevo
2. **¿Cuál es la herramienta estándar de PS?** — Definir cuál es el respaldo si el cliente no tiene
3. **¿Incluimos infraestructura en N3 o queda fuera del alcance?**
4. **¿Quién es el Gerente de Mesa de Servicios?** — Rol crítico para arrancar
5. **¿El modelo de IA va desde el día 1 o se incorpora progresivamente?**
6. **¿Cómo se cobra? ¿Por FTE, por ticket o modelo mixto?**
