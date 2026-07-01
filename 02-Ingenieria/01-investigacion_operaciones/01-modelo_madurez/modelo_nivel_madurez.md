# Modelo de Madurez de Mesas de Servicio · v1.0
**PersonalSoft · ITIL v5 · 4 Dimensiones · 17 Prácticas Operativas + 4 de Negocio · Escala N0–N5**

---

## 1. Propósito del modelo

Este modelo tiene un doble uso: **diagnosticar** el estado real de cualquier mesa de servicio (propia o de un cliente), y servir como **herramienta comercial** para mostrarle al cliente dónde está parado hoy y qué gana al evolucionar hacia la Mesa de Servicios de Nueva Generación con IA.

El modelo está construido sobre **ITIL v5 (2026)** — el marco más adoptado globalmente para gestión de servicios de TI, actualizado para incorporar gobierno de IA, gestión de productos digitales y experiencia como métrica central. Tiene cuatro capas:

- **Clasificador inicial** — determina si la mesa es de Ayuda o de Soporte, y si tiene N0 activo
- **Escala N0–N5** — seis niveles de madurez desde autoservicio puro hasta optimización con IA
- **17 prácticas operativas** — organizadas por las 4 dimensiones reales de ITIL v5
- **4 indicadores de negocio** — evalúan si la mesa es exitosa como negocio para PS, no solo como operación
- **Capa sectorial** — profundización regulatoria para banca (SFC/SOX) y salud (Supersalud/Habeas Data)

---

## 2. Clasificador inicial

Antes de evaluar las prácticas, se determina el tipo de mesa. Esto define el nivel mínimo esperado y el perfil de evaluación.

| Aspecto | Mesa de Ayuda | Mesa de Soporte |
|---|---|---|
| Nivel de servicio | Básico (N1) | Avanzado (N2 y N3) |
| Tipo de atención | Reactiva | Reactiva y proactiva |
| Complejidad | Baja | Media y alta |
| Perfil del equipo | Junior · Atención al usuario | Técnico especializado / Senior |
| Enfoque | Usuario final | Tecnología y continuidad |
| ¿Incluye causa raíz? | No | Sí |
| ¿KPIs de desempeño? | Básicos | Completos con tendencias |
| ¿Change Enablement formal? | No | Sí, con trazabilidad |
| Roles típicos | Analista de soporte | Coordinador · Líder técnico · Desarrollador |
| **Nivel mínimo esperado** | **N2 · Administrado** | **N3 · Definido** |

**Pregunta adicional:** ¿La mesa tiene N0 · Autoservicio activo? (Sí / No / En construcción)
N0 = portal de autoservicio + KEDB accesible al usuario + IA generativa activa. Sin N0, el servicio arranca en N1.

---

## 3. La escala de madurez: N0 a N5

### Tabla resumen

| Nivel | Nombre | Qué caracteriza | Riesgo de quedarse aquí |
|---|---|---|---|
| N0 | Autoservicio | Portal + KEDB + IA. El usuario resuelve solo | KEDB desactualizada = frustración, no ahorro |
| N1 | Inicial | Reactivo total. Depende de personas | Bus factor: si se va la persona, se va el conocimiento |
| N2 | Administrado | Procesos por mesa, sin estandarizar | No escala: cada mesa reinventa el proceso |
| N3 | Definido | Estandarización entre mesas | Sin datos, no se demuestra que el servicio mejora |
| N4 | Cuantitativo | Gestión basada en datos | Alto costo en horas-persona sin automatizar |
| N5 | Optimizado | IA activa, mejora continua | Sin gobierno de IA, la automatización falla a escala |

### N0 · Autoservicio
El usuario resuelve por sí mismo sin abrir un ticket ni contactar a nadie. Existe un portal con KEDB actualizada y una IA generativa que responde preguntas frecuentes. N0 reduce la carga de N1 en solicitudes y consultas repetitivas. Es el primer diferenciador de la Mesa de Nueva Generación.

**Riesgo principal:** si la base de conocimiento no está actualizada o la IA no tiene suficiente contexto, el usuario abandona y escala igual — N0 mal implementado es peor que no tenerlo.

### N1 · Inicial
La mesa funciona pero depende de personas específicas. No hay documentación, los criterios cambian según quién atiende. Incidentes y solicitudes se mezclan sin distinción.

**Riesgo principal:** bus factor crítico. Si se va la persona que "sabe", el servicio se degrada de inmediato.

### N2 · Administrado
Existen procesos pero viven dentro de cada mesa de forma aislada. La herramienta de tickets se usa solo como bitácora. Los reportes se arman manualmente.

**Riesgo principal:** no escala. Cada nuevo cliente exige reinventar el proceso desde cero.

### N3 · Definido
Los procesos están documentados y se replican entre mesas. Existe catálogo de servicios, RACI explícito y metodología común. Es el primer nivel donde se puede hablar de servicio estandarizado.

**Riesgo principal:** sin datos, no se puede demostrar objetivamente que el servicio mejora con el tiempo.

### N4 · Administrado cuantitativamente
La mesa se gestiona con datos reales. Los ANS se miden sistemáticamente. Hay tendencias analizadas y decisiones basadas en evidencia.

**Riesgo principal:** sin automatización, mantener este nivel de medición consume muchas horas-persona.

### N5 · Optimizado
La mesa incorpora IA y automatización en el flujo diario. El foco pasa de "resolver rápido" a "anticipar antes de que el cliente note el problema".

**Riesgo principal:** sin gobierno de IA (human-in-the-loop, ISO 42001), la automatización puede fallar a escala en lugar de dar valor.

---

## 4. Las 17 prácticas operativas organizadas por las 4 dimensiones de ITIL v5

> **Nota sobre ITIL v5:** La versión 5 (lanzada en junio de 2026) mantiene las 34 prácticas de ITIL 4 reorganizadas en dos grupos: 22 de Product and Service Management y 12 de General Management. Las 4 dimensiones se preservan. Este modelo selecciona las 17 prácticas más relevantes para evaluación de mesas de servicio y las organiza según las dimensiones ITIL v5.

---

### Dimensión 1 · Organizaciones y Personas
*Gobierno, roles y cultura del equipo*

#### 1.1 Gobierno de roles (RACI) · Feedback operativo
> Identificada en las mesas actuales de PS: la ausencia de roles claros genera decisiones arbitrarias y escalamientos mal dirigidos.

| Nivel | Descripción |
|---|---|
| N0 | No aplica como práctica independiente en N0 |
| N1 · Inicial | Héroes aislados. Cualquiera hace cualquier cosa según disponibilidad |
| N2 · Administrado | Roles informales conocidos por el equipo, sin documentación ni RACI |
| N3 · Definido | RACI documentado: Coordinador de Servicio, Líder Técnico de Equipo, Especialista / Desarrollador |
| N4 · Cuantitativo | Desempeño medido por rol, RACI ajustado con datos reales de carga |
| N5 · Optimizado | IA sugiere reasignación de tickets según carga, especialidad y disponibilidad en tiempo real |

#### 1.2 Capacidad y dimensionamiento del equipo · ITIL Foundation

| Nivel | Descripción |
|---|---|
| N0 | No aplica como práctica independiente en N0 |
| N1 · Inicial | Cálculo a ojo, sin datos de carga real. Frecuentemente sub o sobre dimensionado |
| N2 · Administrado | Criterio estático que no se revisa aunque la realidad del cliente cambie |
| N3 · Definido | Calculadora FTE basada en volumen histórico real de tickets, incluyendo % GAP administrativo |
| N4 · Cuantitativo | Se mide % de tiempo muerto (GAP) por persona y se ajusta la capacidad con datos |
| N5 · Optimizado | Dimensionamiento dinámico: IA anticipa picos de demanda antes de que ocurran |

---

### Dimensión 2 · Información y Tecnología
*Herramientas, automatización y datos*

#### 2.1 Herramientas y automatización · ITIL Foundation

| Nivel | Descripción |
|---|---|
| N0 | No aplica como práctica independiente en N0 |
| N1 · Inicial | Dispersas: correo, Excel, chats personales sin ninguna integración |
| N2 · Administrado | Herramienta de tickets pero usada solo como bitácora, sin automatización |
| N3 · Definido | Flujos integrados: escalamiento y notificación automática, menos trabajo manual del agente |
| N4 · Cuantitativo | Se mide % de automatización del flujo y su impacto en tiempos de resolución |
| N5 · Optimizado | Agentes de IA conectados: clasifican, sugieren y en algunos casos resuelven tickets automáticamente |

#### 2.2 Gestión del conocimiento (KEDB) · Monitor, Support and Fulfill

| Nivel | Descripción |
|---|---|
| N0 | KEDB activa y accesible al usuario final. Es la base del autoservicio — sin KEDB actualizada no hay N0 real |
| N1 · Inicial | En la cabeza de personas clave. Bus factor crítico |
| N2 · Administrado | Notas aisladas en correos y chats. Nadie sabe dónde buscar la respuesta correcta |
| N3 · Definido | KEDB centralizada, estructurada y con dueño responsable de mantenerla actualizada |
| N4 · Cuantitativo | Uso correlacionado con reducción del tiempo de resolución. Retorno de inversión medible |
| N5 · Optimizado | La KEDB se alimenta automáticamente con cada ticket resuelto. IA sugiere solución antes de que el humano busque |

#### 2.3 Gestión de integraciones y entorno de aplicaciones · Feedback operativo
> Las mesas atienden ecosistemas completos (Canal Asesor, Sura Masivos, Digital Venta, ERPs, historias clínicas). No saber cómo están integrados los sistemas es causa raíz de muchos incidentes mal resueltos o escalados innecesariamente.

| Nivel | Descripción |
|---|---|
| N0 | No aplica como práctica independiente en N0 |
| N1 · Inicial | Sin documentar. Conocimiento informal en pocas personas |
| N2 · Administrado | Lista básica de sistemas sin arquitectura ni dependencias documentadas |
| N3 · Definido | Mapa de integraciones: sistemas, APIs, dependencias y owner técnico de cada integración |
| N4 · Cuantitativo | Alertas configuradas por criticidad de API afectada. Priorización basada en impacto real medido |
| N5 · Optimizado | Monitoreo AIOps: detecta caídas de integración antes de que el usuario las reporte |

#### 2.4 Monitoreo y gestión de eventos · Monitor, Support and Fulfill
> **Nueva práctica incorporada desde revisión ITIL v5.** El módulo oficial Monitor, Support and Fulfill cubre explícitamente Monitoring and Event Management como práctica independiente del Service Desk.

| Nivel | Descripción |
|---|---|
| N0 | No aplica como práctica independiente en N0 |
| N1 · Inicial | Sin monitoreo. Los problemas los reporta el usuario final — siempre después del impacto |
| N2 · Administrado | Monitoreo básico manual. Alertas configuradas pero revisadas de forma inconsistente |
| N3 · Definido | Monitoreo sistemático con umbrales definidos y alertas automáticas al equipo de soporte |
| N4 · Cuantitativo | Correlación de eventos: se analizan patrones para detectar problemas antes de que se acumulen tickets |
| N5 · Optimizado | AIOps: predicción de eventos y resolución proactiva antes de que el incidente impacte al usuario |

---

### Dimensión 3 · Socios y Proveedores
*Niveles de servicio, contratos y límites del alcance*

#### 3.1 Service Desk — punto único de contacto · Monitor, Support and Fulfill
> **Nueva práctica incorporada desde revisión ITIL v5.** Service Desk es una de las 5 prácticas del módulo Monitor, Support and Fulfill. En ITIL v5 se define como "la práctica de proporcionar el punto de entrada y único punto de contacto con el proveedor de servicios para todos los usuarios". No tenerla evaluada explícitamente era una omisión importante — es la práctica que define la mesa misma.

| Nivel | Descripción |
|---|---|
| N0 | No aplica. N0 es el nivel anterior a la mesa — el usuario resuelve sin llegar al Service Desk |
| N1 · Inicial | Sin punto único de contacto. Los usuarios contactan por cualquier canal sin orden ni priorización |
| N2 · Administrado | La mesa existe pero sin roles claros ni procesos formales. Funciona por la voluntad del equipo |
| N3 · Definido | Punto único de contacto definido: canales oficiales, horarios, roles y escalamiento documentado |
| N4 · Cuantitativo | Mesa medida como unidad de negocio: ANS cumplidos, CSAT por ticket, costo/ticket calculado |
| N5 · Optimizado | Mesa orquestada por IA: N0 deflecta, N1 clasifica, N2/N3 solo reciben casos complejos |

#### 3.2 Catálogo de servicios y límites del alcance · ITIL Service

| Nivel | Descripción |
|---|---|
| N0 | No aplica como práctica independiente en N0 |
| N1 · Inicial | Informal, solo verbal. El alcance vive en la cabeza del equipo comercial |
| N2 · Administrado | Firmado y olvidado: desactualizado apenas se firmó el contrato |
| N3 · Definido | Catálogo vivo: el equipo lo conoce y lo usa como referencia real de qué entra y qué no |
| N4 · Cuantitativo | Costeo por servicio: se identifica rentabilidad de cada módulo del catálogo |
| N5 · Optimizado | Ajuste dinámico según demanda real y datos de uso del catálogo |

#### 3.3 SLA / ANS + XLA por prioridad · ITIL Service
> **XLA (Experience Level Agreement)** es una incorporación formal de ITIL v5. Mide la experiencia percibida del usuario, no solo los tiempos técnicos. Un servicio puede cumplir el ANS (tiempo de respuesta) pero fallar el XLA (satisfacción real del usuario). ITIL v5 adopta los XLA como práctica estándar.

| Nivel | Descripción |
|---|---|
| N0 | No aplica. Sin ticket, sin ANS medible |
| N1 · Inicial | No medidos o aspiracionales. Existen pero nunca se midieron desde que se firmaron |
| N2 · Administrado | Medición manual e inconsistente, solo cuando el cliente reclama |
| N3 · Definido | ANS por prioridad: Crítico <1h · Alto <4h · Medio <8h · Bajo <24h. XLA definido por tipo de servicio. Reporte mensual |
| N4 · Cuantitativo | Análisis de tendencia de ANS + XLA correlacionado con experiencia real del usuario |
| N5 · Optimizado | Alertas predictivas: el sistema avisa que un ANS o XLA está en riesgo ANTES de que se incumpla |

**Tiempos de referencia ANS por prioridad (desde N3):**

| Prioridad | Criterio | Tiempo respuesta | Tiempo resolución |
|---|---|---|---|
| Crítico | PDN — afecta continuidad del negocio | < 1 hora | < 4 horas |
| Alto | Afecta múltiples usuarios o proceso crítico | < 4 horas | < 8 horas |
| Medio | Afecta un usuario, tiene workaround | < 8 horas | < 24 horas |
| Bajo | Consulta, solicitud o mejora sin urgencia | < 24 horas | < 72 horas |

#### 3.4 Disponibilidad y cobertura horaria · Feedback operativo

| Nivel | Descripción |
|---|---|
| N0 | N0 activo = cobertura 24x7 automática para solicitudes frecuentes. Sin N0, el servicio tiene horario limitado |
| N1 · Inicial | Best effort: el equipo responde cuando puede, sin compromiso formal de disponibilidad |
| N2 · Administrado | Horario conocido por el equipo pero no pactado contractualmente con el cliente |
| N3 · Definido | Horario definido y pactado (ej. L-V 7:30AM–5PM). GAP administrativo negociado |
| N4 · Cuantitativo | Cumplimiento real de cobertura medido y reportado al cliente con datos |
| N5 · Optimizado | N0/N1 gestionado por IA fuera de horario: 24x7 efectivo sin costo de guardia humana permanente |

---

### Dimensión 4 · Flujos de Valor y Procesos
*Soporte, incidentes, cambios, transición y experiencia del cliente*

#### 4.1 Gestión de incidentes · Monitor, Support and Fulfill

| Nivel | Descripción |
|---|---|
| N0 | No aplica como práctica independiente en N0 |
| N1 · Inicial | Reactivo / apagar incendios. Sin trazabilidad de qué pasó ni por qué |
| N2 · Administrado | Registro básico, categorización inconsistente entre agentes |
| N3 · Definido | Proceso estándar de registro, triaje y escalamiento N1→N2→N3 documentado |
| N4 · Cuantitativo | Tiempos medidos por categoría y nivel con metas claras y reporte de tendencias |
| N5 · Optimizado | Auto-resolución IA: clasifica y sugiere, escala solo cuando la confianza del modelo es baja |

#### 4.2 Gestión de solicitudes · Monitor, Support and Fulfill

| Nivel | Descripción |
|---|---|
| N0 · Autoservicio | El portal resuelve solicitudes frecuentes sin que el usuario abra un ticket ni contacte a nadie |
| N1 · Inicial | Mezcladas con incidentes, sin distinción ni priorización lógica |
| N2 · Administrado | Flujo completamente manual de principio a fin |
| N3 · Definido | Catálogo de solicitudes estándar con tiempos de cumplimiento definidos por tipo |
| N4 · Cuantitativo | ANS medido en tiempo real por tipo de solicitud, con reporte de cumplimiento |
| N5 · Optimizado | Portal N0 expandido con IA: resuelve y aprende de cada interacción automáticamente |

#### 4.3 Gestión de problemas (causa raíz) · Monitor, Support and Fulfill

| Nivel | Descripción |
|---|---|
| N0 | No aplica como práctica independiente en N0 |
| N1 · Inicial | No existe. Cada incidente se resuelve aislado como si fuera la primera vez |
| N2 · Administrado | A voluntad del analista, sin proceso formal institucionalizado |
| N3 · Definido | Análisis formal activado cuando un tipo de incidente se repite más de X veces |
| N4 · Cuantitativo | Se mide reducción de tickets recurrentes tras resolver causa raíz. Retorno medible |
| N5 · Optimizado | IA detecta patrones ocultos proactivamente, antes del umbral de alerta humana |

#### 4.4 Gestión del cambio (Change Enablement) · ITIL Service
> **Nueva práctica incorporada desde revisión ITIL v5.** Change Enablement es una de las prácticas del módulo Plan, Implement and Control de ITIL v5. Era relevante en las mesas actuales (control SOX en banca, segregación de funciones, cambios en producción) pero no estaba como práctica evaluable explícita. Ahora aplica a todas las mesas, no solo a banca.

| Nivel | Descripción |
|---|---|
| N0 | No aplica como práctica independiente en N0 |
| N1 · Inicial | Cambios en producción sin control ni trazabilidad. Cualquiera puede modificar cualquier cosa |
| N2 · Administrado | Registro básico de cambios, sin aprobación formal ni segregación de funciones |
| N3 · Definido | Proceso documentado: quién solicita, quién aprueba y quién despliega están claramente separados |
| N4 · Cuantitativo | Se mide el impacto de cambios en incidentes (cambios que generaron incidentes) y se ajusta el proceso |
| N5 · Optimizado | Cambios evaluados automáticamente por IA según riesgo calculado. Solo los de alto riesgo requieren aprobación humana |

#### 4.5 Transición y onboarding · ITIL Service

| Nivel | Descripción |
|---|---|
| N0 | No aplica como práctica independiente en N0 |
| N1 · Inicial | Improvisada. Se reinventa el proceso con cada cliente nuevo |
| N2 · Administrado | Pasos sueltos, no documentados ni replicables por otra persona del equipo |
| N3 · Definido | Playbook exacto: inducción, documentación, acuerdos, KEDB inicial |
| N4 · Cuantitativo | Métrica 30 días: calidad del arranque medida con datos reales (tickets en primeros 30 días vs. mes 4) |
| N5 · Optimizado | Plantillas IA aceleran la transición. Carga automática de documentación y configuración |

#### 4.6 Mejora continua del servicio · Collaborate, Assure and Improve
> **Nueva práctica incorporada desde revisión ITIL v5.** Mejora Continua es una de las prácticas del módulo Collaborate, Assure and Improve de ITIL v5. Estaba implícita en el nivel N5 pero no como práctica evaluable con su propia rúbrica. Su ausencia significaba que podíamos tener una mesa "optimizada" sin un proceso formal de mejora institucionalizado.

| Nivel | Descripción |
|---|---|
| N0 | No aplica como práctica independiente en N0 |
| N1 · Inicial | Sin proceso de mejora. Solo se reacciona ante crisis. Las lecciones aprendidas no se documentan |
| N2 · Administrado | Mejoras identificadas pero sin priorización ni seguimiento formal. Dependen de la iniciativa individual |
| N3 · Definido | Backlog de mejoras activo: priorizado con owner responsable y fecha de revisión comprometida |
| N4 · Cuantitativo | Mejoras medidas antes y después con datos reales. Se demuestra el retorno de cada iniciativa |
| N5 · Optimizado | IA detecta oportunidades de mejora a partir de patrones de operación. Mejora continua automatizada |

#### 4.7 Experiencia del cliente (CX / NPS / CSAT / XLA) · ITIL Experience

| Nivel | Descripción |
|---|---|
| N0 | Satisfacción medida por tasa de resolución autónoma: % de usuarios que resolvieron sin escalar a N1 |
| N1 · Inicial | Cero quejas = todo OK. No hay mecanismo real de medición de satisfacción |
| N2 · Administrado | Encuesta anual esporádica sin seguimiento a resultados |
| N3 · Definido | CSAT continuo por ticket + XLA definido por tipo de servicio con seguimiento a resultados negativos |
| N4 · Cuantitativo | Cruce operacional: CSAT/XLA correlacionado con tiempos de resolución, reincidencia y NPS |
| N5 · Optimizado | CX en tiempo real: el servicio se ajusta proactivamente antes de que la insatisfacción se formalice |

---

## 5. Dimensión de negocio

Una mesa puede estar en N4 operativamente y ser poco rentable o estar en riesgo de perder al cliente. Esta dimensión evalúa el éxito de la mesa como negocio para PS.

| Indicador | N1 | N3 | N5 |
|---|---|---|---|
| Salud financiera | Pérdida oculta: margen desconocido | Margen por FTE identificado y monitoreado | Upselling automático: IA detecta oportunidades |
| Retención y cuenta | Riesgo de churn no detectado | Plan de cuenta activo, renovación gestionada | Expansión automática: modelo detecta señales |
| NPS / CSAT / XLA | Cliente silencioso | CSAT + XLA sistemáticos, NPS periódico | Predicción de churn antes de la queja |
| Eficiencia de costo | Costo/ticket alto e invisible | Costo/ticket calculado vs. línea base | Automatización escala sola, costo marginal baja |

> **Una mesa exitosa cumple ambas dimensiones:** madura operativamente (N0–N5 en las 17 prácticas) y rentable / valiosa para PS y el cliente.

---

## 6. Capa sectorial: Banca

Complementa las 17 prácticas con criterios bajo supervisión de la **Superintendencia Financiera de Colombia (SFC)**.

| Práctica sectorial | Nivel mínimo | Qué evalúa |
|---|---|---|
| Continuidad de negocio (BCP/DRP) | N3 | ¿Planes de continuidad probados con simulacros ejecutados? |
| Trazabilidad de cambios (SOX) | N3 | ¿Todo cambio en producción tiene aprobación y trazabilidad completa? |
| Gestión de incidentes de seguridad | N3 | ¿Proceso diferenciado para fraude o vulnerabilidades de seguridad? |
| Reportabilidad regulatoria | N4 | ¿La mesa genera evidencia auditable ante un requerimiento de la SFC? |
| Segregación de funciones | N3 | ¿Quien atiende, aprueba y despliega están claramente separados? |
| Disponibilidad de canales críticos | N4 | ¿Se mide y reporta disponibilidad de canales transaccionales? |

**Argumento de venta:** "Hoy su mesa opera sin trazabilidad completa de cambios. Eso es exposición regulatoria ante la SFC. Con N3 en adelante, cada cambio queda documentado y auditable — reduce su riesgo regulatorio, no solo mejora el soporte técnico."

---

## 7. Capa sectorial: Salud (EPS)

Complementa las 17 prácticas con criterios bajo **Supersalud** y la Ley 1581 de 2012 (Habeas Data en salud).

| Práctica sectorial | Nivel mínimo | Qué evalúa |
|---|---|---|
| Protección de datos sensibles de salud | N3 | ¿Acceso a historia clínica controlado y auditado individualmente? |
| Continuidad de servicios asistenciales | N3 | ¿Protocolos diferenciados para incidentes que afectan atención al paciente? |
| Trazabilidad clínica | N3 | ¿Todo cambio en historia clínica queda registrado y es auditable? |
| Incidentes con impacto asistencial | N3 | ¿Clasificación diferenciada entre ticket administrativo y uno que afecta un paciente? |
| Interoperabilidad | N3 | ¿Los sistemas cumplen estándares RIPS / PISIS del Ministerio de Salud? |

**Argumento de venta:** "Un problema de autorización de un procedimiento urgente puede esperar en la misma fila que un reseteo de contraseña. Con N3, los incidentes asistenciales se priorizan automáticamente — protege la continuidad asistencial y reduce el riesgo ante Supersalud."

---

## 8. Lo que incorporó esta versión vs. versiones anteriores

Esta es la primera versión numerada (v1.0) del modelo. Integra todo el trabajo iterativo previo más las siguientes incorporaciones basadas en la revisión de la documentación oficial de ITIL v5 (2026):

| Incorporación | Por qué se agregó |
|---|---|
| **Service Desk como práctica evaluable (D3)** | Es una de las 5 prácticas oficiales del módulo Monitor, Support and Fulfill de ITIL v5. No tenerla era una omisión — es la práctica que define la mesa misma |
| **Monitoreo y gestión de eventos (D2)** | Práctica oficial ITIL v5. Detectar antes de que el usuario reporte es la diferencia entre N4 y N5 |
| **Gestión del cambio / Change Enablement (D4)** | Práctica del módulo Plan, Implement and Control de ITIL v5. Aplica a todas las mesas (no solo banca) |
| **Mejora continua del servicio (D4)** | Práctica del módulo Collaborate, Assure and Improve de ITIL v5. Sin este backlog formal, N5 no es sostenible |
| **XLA (Experience Level Agreement)** | ITIL v5 adopta formalmente los XLA como estándar. Integrado en la práctica 3.3 (ANS+XLA) y en 4.7 (CX) |
| **N0 como nivel propio** | ITIL v5 posiciona el autoservicio como nivel de servicio, no como característica opcional |
| **Dimensión de negocio** | Fuera del alcance de ITIL pero necesaria para evaluar si la mesa es exitosa para PS como negocio |

---

## 9. Aplicación comercial

### 9.1 Flujo de uso en conversación de venta

1. **Clasificar** — ¿Mesa de Ayuda o de Soporte? ¿Tiene N0 activo?
2. **Evaluar** — Aplicar el instrumento Excel a las mesas del cliente (17 prácticas + negocio, escala N0–N5)
3. **Diagnosticar** — Identificar prácticas por debajo del mínimo esperado (marcadas en rojo en el Excel)
4. **Visualizar** — Mostrar el Dashboard: radar por dimensión, barras comparativas entre mesas
5. **Presentar roadmap** — Qué cambia en el negocio del cliente en cada salto de nivel
6. **Conectar con valor** — Menos tickets recurrentes, menos riesgo regulatorio, mejor experiencia del usuario
7. **Activar capa sectorial** — Si aplica banca o salud, agregar criterios regulatorios como diferenciador

### 9.2 Conexión con el plan general del servicio

Este modelo es el insumo de entrada de la **Fase 4 (Transición de clientes actuales)**: antes de proponer la migración de una mesa al nuevo modelo de Mesa de Servicios de Nueva Generación con IA, se aplica esta evaluación para tener evidencia objetiva del punto de partida y construir el caso de negocio de la transición.

---

## 10. Próximos pasos

1. **Pilotar el clasificador** en las 8 mesas activas (4 SURA + 4 Bancolombia) — definir si cada una es de Ayuda o de Soporte y si tienen N0 activo
2. **Aplicar el instrumento Excel v1.0** en cada mesa para obtener el perfil de madurez inicial
3. **Validar los tiempos de ANS** por prioridad (Crítico/Alto/Medio/Bajo) con el equipo de delivery de cada cuenta
4. **Validar Change Enablement y Mejora continua** con los líderes técnicos de cada mesa — son las prácticas más nuevas y pueden requerir calibración
5. **Construir el slide deck comercial** con los resultados del Dashboard para presentar a las cuentas
6. **Definir el estándar de mercado esperado** por tipo de mesa y sector como referencia comparativa
7. **Integrar con Fase 4** del plan de diseño: diagnóstico de madurez como condición de entrada para la propuesta de transición
8. **Explorar capa sectorial para Centro América** (Curasao y otros) con sus particularidades regulatorias propias
