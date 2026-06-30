# Modelo de Madurez de Mesas de Servicio
**PersonalSoft · Basado en ITIL v5 · Borrador para validación CTO/SICTO**

---

## 1. Propósito del modelo

Este modelo permite evaluar el nivel de madurez actual de cualquier mesa de servicio operada (propia o de cliente), con el fin de identificar brechas, priorizar inversión y diseñar el plan de evolución hacia la Mesa de Servicios de Nueva Generación con IA.

Aplica de forma agnóstica a cualquier mesa, independiente de la industria o del cliente.

---

## 2. Marco de referencia: ITIL v5

ITIL v5 organiza el conocimiento en cuatro grandes esquemas de calificación. Este modelo de madurez evalúa la mesa de servicio según qué tan desarrollada está la organización en cada uno de estos cuatro frentes:

<svg width="100%" viewBox="0 0 700 260" xmlns="http://www.w3.org/2000/svg">
<rect x="20" y="20" width="660" height="50" rx="8" fill="#26215C" stroke="#534AB7" stroke-width="0.5"/>
<text x="350" y="50" text-anchor="middle" font-size="13" font-weight="500" fill="#CECBF6" font-family="sans-serif">ITIL Master · Reconocimiento de dominio integral del marco</text>

<rect x="20" y="90" width="660" height="60" rx="8" fill="#EEEDFE" stroke="#AFA9EC" stroke-width="0.5"/>
<text x="350" y="106" text-anchor="middle" font-size="11" font-weight="500" fill="#3C3489" font-family="sans-serif">ML Transformation</text>
<text x="158" y="128" text-anchor="middle" font-size="10" fill="#534AB7" font-family="sans-serif">ITIL Service</text>
<text x="350" y="128" text-anchor="middle" font-size="10" fill="#534AB7" font-family="sans-serif">ITIL Experience</text>
<text x="540" y="128" text-anchor="middle" font-size="10" fill="#534AB7" font-family="sans-serif">ITIL Strategy</text>
<text x="158" y="144" text-anchor="middle" font-size="9" fill="#7F77DD" font-family="sans-serif">Diseño y entrega del servicio</text>
<text x="350" y="144" text-anchor="middle" font-size="9" fill="#7F77DD" font-family="sans-serif">Experiencia del cliente y usuario</text>
<text x="540" y="144" text-anchor="middle" font-size="9" fill="#7F77DD" font-family="sans-serif">Visión y dirección estratégica</text>

<rect x="20" y="170" width="660" height="60" rx="8" fill="#E1F5EE" stroke="#1D9E75" stroke-width="0.5"/>
<text x="350" y="186" text-anchor="middle" font-size="11" font-weight="500" fill="#085041" font-family="sans-serif">ITIL Foundation · Base obligatoria para todo el esquema</text>
<text x="200" y="206" text-anchor="middle" font-size="10" fill="#0F6E56" font-family="sans-serif">Monitor, Support and Fulfill</text>
<text x="350" y="206" text-anchor="middle" font-size="10" fill="#0F6E56" font-family="sans-serif">Plan, Implement and Control</text>
<text x="520" y="206" text-anchor="middle" font-size="10" fill="#0F6E56" font-family="sans-serif">Collaborate, Assure and Improve</text>
<text x="350" y="222" text-anchor="middle" font-size="9" fill="#1D9E75" font-family="sans-serif">Núcleo operativo: gestión de incidentes, peticiones, problemas y conocimiento</text>
</svg>

### 2.1 Los cuatro frentes evaluables

| Frente ITIL v5 | Qué evalúa en la mesa de servicio |
|---|---|
| **ITIL Foundation** | Conocimiento y aplicación básica de los conceptos de gestión de servicios |
| **Monitor, Support and Fulfill** | Capacidad operativa de la mesa: cómo monitorea, soporta y resuelve solicitudes |
| **ITIL Service** | Calidad del diseño y entrega del servicio: catálogo, SLA, niveles, transición |
| **ITIL Experience** | Experiencia real del cliente y del usuario final con la mesa |

> Nota: el esquema también incluye Plan/Implement/Control, Collaborate/Assure/Improve y Strategy, que se incorporan en una segunda iteración del modelo conforme la mesa madure más allá del nivel operativo básico.

---

## 3. Niveles de madurez

El modelo usa una escala de 5 niveles, alineada con la lógica de CMMI pero adaptada al lenguaje de gestión de servicios de ITIL.

<svg width="100%" viewBox="0 0 700 320" xmlns="http://www.w3.org/2000/svg">
<defs>
<marker id="arr" viewBox="0 0 10 10" refX="8" refY="5" markerWidth="6" markerHeight="6" orient="auto-start-reverse">
<path d="M2 1L8 5L2 9" fill="none" stroke="context-stroke" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</marker>
</defs>

<rect x="20" y="270" width="660" height="40" rx="6" fill="#FAECE7" stroke="#D85A30" stroke-width="0.5"/>
<text x="55" y="294" font-size="13" font-weight="500" fill="#712B13" font-family="sans-serif">1</text>
<text x="90" y="288" font-size="11" font-weight="500" fill="#712B13" font-family="sans-serif">Inicial</text>
<text x="90" y="302" font-size="9" fill="#993C1D" font-family="sans-serif">Proceso impredecible, poco control, reactivo total</text>

<rect x="20" y="220" width="660" height="40" rx="6" fill="#FAEEDA" stroke="#EF9F27" stroke-width="0.5"/>
<text x="55" y="244" font-size="13" font-weight="500" fill="#633806" font-family="sans-serif">2</text>
<text x="90" y="238" font-size="11" font-weight="500" fill="#633806" font-family="sans-serif">Administrado</text>
<text x="90" y="252" font-size="9" fill="#854F0B" font-family="sans-serif">Proceso por mesa, documentación parcial, sin estandarizar entre mesas</text>

<rect x="20" y="170" width="660" height="40" rx="6" fill="#E6F1FB" stroke="#378ADD" stroke-width="0.5"/>
<text x="55" y="194" font-size="13" font-weight="500" fill="#0C447C" font-family="sans-serif">3</text>
<text x="90" y="188" font-size="11" font-weight="500" fill="#0C447C" font-family="sans-serif">Definido</text>
<text x="90" y="202" font-size="9" fill="#185FA5" font-family="sans-serif">Estandarización entre mesas, procesos documentados y consistentes</text>

<rect x="20" y="120" width="660" height="40" rx="6" fill="#EEEDFE" stroke="#7F77DD" stroke-width="0.5"/>
<text x="55" y="144" font-size="13" font-weight="500" fill="#3C3489" font-family="sans-serif">4</text>
<text x="90" y="138" font-size="11" font-weight="500" fill="#3C3489" font-family="sans-serif">Administrado cuantitativamente</text>
<text x="90" y="152" font-size="9" fill="#534AB7" font-family="sans-serif">Procesos medibles, predecibles, basados en datos (KPIs reales, no empíricos)</text>

<rect x="20" y="70" width="660" height="40" rx="6" fill="#E1F5EE" stroke="#1D9E75" stroke-width="0.5"/>
<text x="55" y="94" font-size="13" font-weight="500" fill="#085041" font-family="sans-serif">5</text>
<text x="90" y="88" font-size="11" font-weight="500" fill="#085041" font-family="sans-serif">Optimizado</text>
<text x="90" y="102" font-size="9" fill="#0F6E56" font-family="sans-serif">Mejora continua activa, IA y automatización integradas, anticipación</text>

<line x1="50" y1="62" x2="50" y2="40" stroke="#888780" stroke-width="1" marker-end="url(#arr)"/>
<text x="350" y="30" text-anchor="middle" font-size="11" font-weight="500" fill="#5F5E5A" font-family="sans-serif">Dirección de evolución del servicio</text>
</svg>

### 3.1 Descripción de cada nivel

**Nivel 1 · Inicial**
La mesa opera de forma reactiva y sin estándar. No hay documentación consistente, las soluciones dependen del conocimiento individual de cada persona, y no existe trazabilidad de lo que pasó con cada caso. Es el punto de partida típico de una mesa heredada de un modelo de staff augmentation sin gobierno.

**Nivel 2 · Administrado**
Existen procesos, pero viven a nivel de cada mesa individual, no de la organización. Hay algo de documentación, pero no está estandarizada entre clientes. Las decisiones siguen siendo en buena parte empíricas.

**Nivel 3 · Definido**
Los procesos están documentados, son consistentes y se replican entre mesas distintas. Existe un catálogo de servicios claro, roles definidos, RACI explícito y una metodología común — aunque la ejecución todavía dependa de la disciplina del equipo.

**Nivel 4 · Administrado cuantitativamente**
La mesa se gestiona con datos: SLA medidos de verdad (no solo pactados), KPIs con metas, tendencias analizadas. Las decisiones de mejora se toman con evidencia, no por percepción.

**Nivel 5 · Optimizado**
La mesa incorpora IA y automatización de forma activa: clasificación automática, sugerencia de soluciones, monitoreo predictivo. El foco pasa de resolver a anticipar. Es el nivel al que apunta la Mesa de Servicios de Nueva Generación.

---

## 4. Prácticas evaluadas

Basado en lo que el equipo ya identificó como relevante (Foundation, Monitor/Support/Fulfill, Service, Experience), el modelo evalúa 10 prácticas concretas, agrupadas por frente ITIL:

| # | Práctica | Frente ITIL v5 |
|---|---|---|
| 1 | Gestión de incidentes | Monitor, Support and Fulfill |
| 2 | Gestión de solicitudes / peticiones | Monitor, Support and Fulfill |
| 3 | Gestión de problemas (causa raíz) | Monitor, Support and Fulfill |
| 4 | Gestión del conocimiento | Monitor, Support and Fulfill |
| 5 | Catálogo de servicios | ITIL Service |
| 6 | Niveles de servicio (SLA) | ITIL Service |
| 7 | Transición y onboarding de servicios | ITIL Service |
| 8 | Satisfacción y experiencia del cliente | ITIL Experience |
| 9 | Capacidad y dimensionamiento del equipo | Foundation |
| 10 | Herramientas y automatización | Foundation |

---

## 5. Instrumento de evaluación

Para cada práctica se evalúa con una rúbrica de 5 niveles. El evaluador marca el nivel que mejor describe el estado actual de la mesa, basado en evidencia (no en percepción).

### 5.1 Práctica 1 · Gestión de incidentes

| Nivel | Descripción observable |
|---|---|
| 1 · Inicial | Los incidentes se resuelven sin registro formal ni categorización consistente |
| 2 · Administrado | Se registran en una herramienta, pero la categorización es inconsistente entre agentes |
| 3 · Definido | Existe un proceso documentado de registro, categorización y escalamiento (N1→N2→N3) |
| 4 · Cuantitativo | Se mide tiempo de resolución por categoría y nivel, con metas claras |
| 5 · Optimizado | Clasificación automática con IA, sugerencia de solución antes de escalar |

### 5.2 Práctica 2 · Gestión de solicitudes / peticiones

| Nivel | Descripción observable |
|---|---|
| 1 · Inicial | No hay diferencia entre incidente y solicitud; todo se trata igual |
| 2 · Administrado | Se distingue solicitud de incidente, pero el flujo es manual en su totalidad |
| 3 · Definido | Existe catálogo de solicitudes estándar con tiempos de cumplimiento definidos |
| 4 · Cuantitativo | Se mide el cumplimiento de solicitudes contra el SLA pactado, con reportes periódicos |
| 5 · Optimizado | Portal de autoservicio (N0) resuelve solicitudes frecuentes sin intervención humana |

### 5.3 Práctica 3 · Gestión de problemas (causa raíz)

| Nivel | Descripción observable |
|---|---|
| 1 · Inicial | No se investiga causa raíz; cada incidente se resuelve de forma aislada |
| 2 · Administrado | Se investiga causa raíz de forma esporádica, sin proceso formal |
| 3 · Definido | Existe proceso documentado de análisis de causa raíz para incidentes recurrentes |
| 4 · Cuantitativo | Se mide la reducción de tickets recurrentes tras resolver la causa raíz |
| 5 · Optimizado | IA detecta patrones de causa raíz de forma proactiva, antes de que se acumulen tickets |

### 5.4 Práctica 4 · Gestión del conocimiento

| Nivel | Descripción observable |
|---|---|
| 1 · Inicial | El conocimiento vive solo en la cabeza de las personas, no hay documentación |
| 2 · Administrado | Hay documentación dispersa (notas, correos), sin repositorio central |
| 3 · Definido | Existe una base de conocimiento (KEDB) estructurada y mantenida |
| 4 · Cuantitativo | Se mide el uso de la base de conocimiento y su impacto en tiempo de resolución |
| 5 · Optimizado | La base de conocimiento se alimenta automáticamente con IA y sugiere soluciones en N0/N1 |

### 5.5 Práctica 5 · Catálogo de servicios

| Nivel | Descripción observable |
|---|---|
| 1 · Inicial | No existe catálogo formal; el alcance del servicio se entiende de forma verbal |
| 2 · Administrado | Existe un catálogo básico, pero desactualizado o incompleto |
| 3 · Definido | Catálogo formal, actualizado, con descripción clara de cada servicio incluido |
| 4 · Cuantitativo | Se mide el uso de cada servicio del catálogo y su rentabilidad |
| 5 · Optimizado | El catálogo se ajusta dinámicamente según demanda real y datos de uso |

### 5.6 Práctica 6 · Niveles de servicio (SLA)

| Nivel | Descripción observable |
|---|---|
| 1 · Inicial | No hay SLA definidos, o existen pero no se miden |
| 2 · Administrado | Hay SLA pactados con el cliente, pero la medición es manual e inconsistente |
| 3 · Definido | SLA documentados, medidos de forma sistemática, con reporte periódico al cliente |
| 4 · Cuantitativo | Se analiza tendencia de cumplimiento de SLA y se ajustan metas con datos |
| 5 · Optimizado | Alertas predictivas anticipan incumplimientos de SLA antes de que ocurran |

### 5.7 Práctica 7 · Transición y onboarding de servicios

| Nivel | Descripción observable |
|---|---|
| 1 · Inicial | No hay proceso de transición; el arranque con cada cliente es improvisado |
| 2 · Administrado | Hay pasos básicos de transición, pero no documentados ni replicables |
| 3 · Definido | Existe un playbook de transición estándar (inducción, documentación, acuerdos) |
| 4 · Cuantitativo | Se mide el tiempo de transición y la calidad del arranque (tickets en primeros 30 días) |
| 5 · Optimizado | La transición se acelera con plantillas inteligentes y checklists automatizados |

### 5.8 Práctica 8 · Satisfacción y experiencia del cliente

| Nivel | Descripción observable |
|---|---|
| 1 · Inicial | No se mide satisfacción; se asume que "todo está bien" si no hay quejas |
| 2 · Administrado | Se hacen encuestas esporádicas, sin proceso sistemático |
| 3 · Definido | Encuesta de satisfacción (CSAT) por ticket o periódica, con seguimiento |
| 4 · Cuantitativo | Se correlaciona CSAT con otros indicadores (tiempo de resolución, reincidencia) |
| 5 · Optimizado | La experiencia se monitorea en tiempo real y se ajusta el servicio proactivamente |

### 5.9 Práctica 9 · Capacidad y dimensionamiento del equipo

| Nivel | Descripción observable |
|---|---|
| 1 · Inicial | El equipo se dimensiona de forma intuitiva, sin datos de carga real |
| 2 · Administrado | Hay algún criterio de dimensionamiento, pero no se revisa con el tiempo |
| 3 · Definido | Existe una calculadora o modelo de estimación basado en volumen histórico de tickets |
| 4 · Cuantitativo | Se mide el % de tiempo muerto (GAP) por persona y se ajusta la capacidad con datos |
| 5 · Optimizado | El dimensionamiento se ajusta dinámicamente según demanda predicha por IA |

### 5.10 Práctica 10 · Herramientas y automatización

| Nivel | Descripción observable |
|---|---|
| 1 · Inicial | Herramientas dispersas (correo, Excel, chats), sin integración |
| 2 · Administrado | Hay una herramienta de tickets, pero subutilizada (solo registro, sin automatización) |
| 3 · Definido | Herramienta de tickets integrada con flujos de escalamiento y notificación automática |
| 4 · Cuantitativo | Se mide el % de automatización del flujo y su impacto en tiempos | 
| 5 · Optimizado | Agentes de IA conectados a la herramienta: clasificación, sugerencia y resolución automática |

---

## 6. Plantilla de aplicación por mesa

Para cada mesa evaluada, se registra:

| Campo | Contenido |
|---|---|
| Nombre de la mesa | (Ej. Mesa de Cotizadores, Mesa de Torre de Control...) |
| Cliente / cuenta | (Identificador interno de la cuenta) |
| Fecha de evaluación | DD/MM/AAAA |
| Evaluador | Nombre de quien realiza la valoración |
| Nivel por práctica (1–5) | Tabla con las 10 prácticas y el nivel asignado a cada una |
| Nivel de madurez global | Promedio o nivel mínimo entre las 10 prácticas (definir criterio de agregación) |
| Evidencias | Qué se observó para sustentar cada nivel asignado |
| Brechas identificadas | Lista de gaps priorizados |
| Recomendación de evolución | Próximo nivel objetivo y qué se requiere para alcanzarlo |

### 6.1 Ejemplo de tabla de resultados (formato sugerido)

| Práctica | Nivel actual | Nivel objetivo (6 meses) | Brecha principal |
|---|---|---|---|
| 1. Gestión de incidentes | 2 | 4 | Falta categorización consistente y medición de tiempos |
| 2. Gestión de solicitudes | 2 | 3 | No hay catálogo de solicitudes estándar |
| 3. Gestión de problemas | 1 | 3 | No se investiga causa raíz de forma sistemática |
| 4. Gestión del conocimiento | 2 | 4 | Conocimiento disperso, sin KEDB estructurado |
| 5. Catálogo de servicios | 2 | 3 | Catálogo desactualizado |
| 6. SLA | 2 | 4 | Medición manual e inconsistente |
| 7. Transición / onboarding | 1 | 3 | No hay playbook replicable |
| 8. Satisfacción del cliente | 1 | 3 | No se mide CSAT de forma sistemática |
| 9. Capacidad del equipo | 2 | 4 | Dimensionamiento intuitivo, sin datos de GAP |
| 10. Herramientas y automatización | 2 | 5 | Sin integración de IA en el flujo |

---

## 7. Cómo se usa este modelo

1. **Levantamiento inicial:** se aplica el instrumento a cada mesa actual del cliente (ej. SURA: Cotizadores, Venta Canal Digital, Torre de Control; Bancolombia: GIOTI; XM: Paquete 3; Medicarte: Historia clínica médica)
2. **Consolidación:** se construye un mapa de calor con el nivel de cada mesa por práctica, para ver dónde están las brechas más grandes a nivel de portafolio
3. **Priorización:** se identifican las prácticas con mayor brecha y mayor impacto en el negocio del cliente
4. **Plan de evolución:** se diseña una hoja de ruta de transición por mesa, alineada con el modelo de transición de clientes (Fase 4 del plan general del servicio)
5. **Reevaluación periódica:** se repite la valoración cada 6 meses para medir avance real

---

## 8. Próximos pasos sugeridos

1. Validar las 10 prácticas y la rúbrica con el equipo CTO/SICTO
2. Definir el criterio de agregación del nivel global (promedio simple, nivel mínimo, ponderado por criticidad)
3. Aplicar el instrumento como piloto en una mesa conocida (ej. una de las mesas de SURA) para calibrar la rúbrica
4. Construir el mapa de calor consolidado de todas las mesas actuales
5. Conectar este modelo de madurez con el Service Blueprint y el rediseño estandarizado (TO-BE) del servicio
