# Modelo de Madurez de Mesas de Servicio
**PersonalSoft · ITIL v5 · Escala N0–N5 · 4 dimensiones · 13 prácticas + negocio + capa sectorial**

---

## 1. Propósito del modelo

Este modelo tiene un doble uso: **diagnosticar** el estado real de cualquier mesa de servicio (propia o de un cliente), y servir como **herramienta comercial** para mostrarle al cliente dónde está parado hoy y qué gana al evolucionar.

El modelo tiene cuatro capas:

- **Clasificador inicial** — determina si la mesa es de Ayuda o de Soporte, y si tiene N0 activo
- **Escala N0–N5** — seis niveles de madurez desde autoservicio puro hasta optimización con IA
- **13 prácticas operativas** — organizadas por las 4 dimensiones reales de ITIL v5
- **Dimensión de negocio** — evalúa si la mesa es exitosa como negocio, no solo como operación
- **Capa sectorial** — profundización regulatoria para banca (SFC/SOX) y salud (Supersalud/Habeas Data)

### 1.1 Clasificador inicial

| Aspecto | Mesa de Ayuda | Mesa de Soporte |
|---|---|---|
| Nivel de servicio | Básico (N1) | Avanzado (N2 y N3) |
| Tipo de atención | Reactiva | Reactiva y proactiva |
| Complejidad | Baja | Media y alta |
| Perfil del equipo | Junior · Atención al usuario | Técnico especializado / Senior |
| Enfoque | Usuario final | Tecnología y continuidad |
| ¿Incluye causa raíz? | No | Sí |
| ¿KPIs de desempeño? | Básicos | Completos con tendencias |
| Roles típicos | Analista de soporte | Coordinador · Líder técnico · Desarrollador |
| **Nivel mínimo esperado** | **N2 · Administrado** | **N3 · Definido** |

**Pregunta adicional del clasificador:** ¿La mesa tiene N0 · Autoservicio activo?
Opciones: Sí / No / En construcción.
N0 = portal de autoservicio + KEDB + IA generativa activa. Sin N0, el servicio arranca en N1.

---

## 2. La escala de madurez: N0 a N5

La escala tiene seis niveles. N0 es nuevo respecto a versiones anteriores del modelo — representa el autoservicio puro, donde el usuario resuelve sin intervención humana ni técnica.

### N0 · Autoservicio

**Qué caracteriza este nivel**
El usuario resuelve por sí mismo sin abrir un ticket ni contactar a nadie. Existe un portal de autoservicio con una base de conocimiento (KEDB) actualizada y una IA generativa que responde preguntas frecuentes. La mesa opera, pero N0 reduce la carga de N1 en solicitudes y consultas repetitivas.

**Comportamientos típicos**
- Portal de autoservicio disponible 24x7
- Base de conocimiento accesible al usuario final (no solo al equipo interno)
- IA generativa responde preguntas frecuentes sin escalamiento
- El usuario resuelve sin abrir un ticket

**Qué experimenta el cliente**
Resuelve solo, sin esperar a que alguien lo atienda. Disponible en cualquier horario.

**Riesgo principal**
Si la base de conocimiento no está actualizada o la IA no tiene suficiente contexto, el usuario abandona y escala igual — N0 que no funciona es peor que no tenerlo porque genera frustración adicional.

---

### N1 · Inicial

**Qué caracteriza este nivel**
La mesa funciona pero depende de personas específicas. No hay documentación, los criterios cambian según quién atiende. El cliente percibe el servicio como impredecible.

**Comportamientos típicos**
- Tickets resueltos pero sin saber cuántos hay realmente
- Criterios de priorización cambian según quién atiende
- Sin lugar único para documentar soluciones
- Incidentes y solicitudes mezclados sin distinción
- Tiempo de resolución desconocido

**Qué experimenta el cliente**
Servicio impredecible: a veces rápido, a veces lento, sin explicación. No sabe si recibe lo que paga.

**Riesgo principal**
Bus factor crítico. Si se va la persona que "sabe", el servicio se degrada de inmediato.

---

### N2 · Administrado

**Qué caracteriza este nivel**
Existen procesos pero viven dentro de cada mesa de forma aislada. La herramienta de tickets se usa solo como bitácora. Los reportes se arman manualmente.

**Comportamientos típicos**
- Cada mesa tiene "su manera", distinta a la de al lado
- Herramienta de tickets usada solo como bitácora
- Reportes armados manualmente con alto esfuerzo
- Conocimiento se transmite de boca a boca
- SLA pactados pero medición manual e inconsistente

**Qué experimenta el cliente**
Nota regularidad pero no puede comparar. No sabe si su mesa es mejor o peor que el mercado.

**Riesgo principal**
No escala. Cada nuevo cliente exige reinventar el proceso desde cero.

---

### N3 · Definido

**Qué caracteriza este nivel**
Los procesos están documentados y se replican entre mesas. Existe catálogo de servicios, RACI explícito y metodología común. Es el primer nivel donde se puede hablar de servicio estandarizado.

**Comportamientos típicos**
- Catálogo de servicios formal y conocido por el equipo
- RACI documentado: Coordinador, Líder Técnico, Especialista / Desarrollador
- ANS por prioridad: Crítico <1h · Alto <4h · Medio <8h · Bajo <24h
- KEDB centralizada con dueño responsable
- Playbook de transición replicable entre clientes

**Qué experimenta el cliente**
Empieza a confiar. Puede anticipar tiempos y sabe exactamente qué incluye el contrato.

**Riesgo principal**
Sin datos, no se puede demostrar objetivamente que el servicio mejora con el tiempo.

---

### N4 · Administrado cuantitativamente

**Qué caracteriza este nivel**
La mesa se gestiona con datos reales. Los SLA/ANS no solo están pactados — se miden sistemáticamente. Hay tendencias analizadas y decisiones basadas en evidencia.

**Comportamientos típicos**
- Dashboard de KPIs actualizado con metas claras
- Análisis de causa raíz sistemático para incidentes recurrentes
- % GAP de tiempo muerto medido y ajustado
- Reportes mensuales con tendencias, no solo fotos del mes
- Costo por ticket calculado y monitorizado

**Qué experimenta el cliente**
Recibe evidencia objetiva. Puede decidir renovar o ampliar con datos reales, no con percepción subjetiva.

**Riesgo principal**
Sin automatización, mantener este nivel de medición consume muchas horas-persona.

---

### N5 · Optimizado

**Qué caracteriza este nivel**
La mesa incorpora IA y automatización en el flujo diario. El foco pasa de "resolver rápido" a "anticipar antes de que el cliente note el problema". Es el nivel al que apunta la Mesa de Servicios de Nueva Generación con IA.

**Comportamientos típicos**
- Clasificación automática de tickets sin intervención humana
- Sugerencia de solución antes de escalar (KEDB + IA)
- AIOps: monitoreo predictivo detecta anomalías antes del incidente
- El equipo humano se enfoca en lo que requiere juicio, no rutina
- Upselling detectado automáticamente por patrones de uso

**Qué experimenta el cliente**
El servicio se siente como socio activo, no como soporte. Mejora sin que el cliente lo pida.

**Riesgo principal**
Sin gobierno de IA (human-in-the-loop, ISO 42001), la automatización puede fallar a escala en lugar de dar valor.

---

### Tabla resumen de niveles

| Nivel | Nombre | Resumen | Riesgo principal |
|---|---|---|---|
| N0 | Autoservicio | Portal + KEDB + IA. Sin intervención humana | KEDB desactualizada = frustración, no ahorro |
| N1 | Inicial | Reactivo total, depende de personas | Bus factor: si se va la persona, se va el conocimiento |
| N2 | Administrado | Procesos por mesa, sin estandarizar | No escala: cada mesa reinventa el proceso |
| N3 | Definido | Estandarización entre mesas | Sin datos, no se demuestra mejora objetiva |
| N4 | Cuantitativo | Gestión basada en datos | Alto costo en horas-persona sin automatizar |
| N5 | Optimizado | IA activa, mejora continua | Sin gobierno de IA, falla a escala |

**Nivel mínimo esperado según tipo de mesa:**
- Mesa de Ayuda → N2 · Administrado
- Mesa de Soporte → N3 · Definido

---

## 3. Las 13 prácticas organizadas por las 4 dimensiones de ITIL v5

### Dimensión 1 · Organizaciones y Personas
*Gobierno, roles y cultura del equipo*

#### 3.1 Gobierno de roles (RACI) · Feedback operativo
> La ausencia de roles claros genera decisiones arbitrarias y escalamientos mal dirigidos. Un RACI bien definido es condición necesaria para que las demás prácticas funcionen.

| Nivel | Descripción |
|---|---|
| N0 | No aplica como práctica independiente en N0 |
| N1 · Inicial | Héroes aislados. Cualquiera hace cualquier cosa según disponibilidad |
| N2 · Administrado | Roles informales conocidos por el equipo, sin documentación ni RACI |
| N3 · Definido | RACI documentado: Coordinador de Servicio, Líder Técnico, Especialista / Desarrollador |
| N4 · Cuantitativo | Desempeño medido por rol, RACI ajustado con datos reales de carga |
| N5 · Optimizado | IA sugiere reasignación de tickets según carga, especialidad y disponibilidad |

#### 3.2 Capacidad y dimensionamiento del equipo · ITIL Foundation

| Nivel | Descripción |
|---|---|
| N0 | No aplica como práctica independiente en N0 |
| N1 · Inicial | Cálculo a ojo, sin datos de carga real |
| N2 · Administrado | Criterio estático que no se revisa aunque la realidad del cliente cambie |
| N3 · Definido | Calculadora FTE basada en volumen histórico real de tickets |
| N4 · Cuantitativo | Se mide % GAP de tiempo muerto por persona y se ajusta la capacidad con datos |
| N5 · Optimizado | Dimensionamiento dinámico: IA anticipa picos antes de que ocurran |

---

### Dimensión 2 · Información y Tecnología
*Herramientas, automatización y datos*

#### 3.3 Herramientas y automatización · ITIL Foundation

| Nivel | Descripción |
|---|---|
| N0 | No aplica como práctica independiente en N0 |
| N1 · Inicial | Dispersas: correo, Excel, chats personales sin ninguna integración |
| N2 · Administrado | Herramienta de tickets pero usada solo como bitácora, sin automatización |
| N3 · Definido | Flujos integrados: escalamiento y notificación automática, menos trabajo manual |
| N4 · Cuantitativo | Se mide % de automatización del flujo y su impacto en tiempos de resolución |
| N5 · Optimizado | Agentes de IA clasifican, sugieren y en algunos casos resuelven tickets automáticamente |

#### 3.4 Gestión del conocimiento (KEDB) · Monitor, Support and Fulfill

| Nivel | Descripción |
|---|---|
| N0 | KEDB activa y accesible al usuario final. Es la base del autoservicio — sin KEDB no hay N0 real |
| N1 · Inicial | En la cabeza de personas clave. Bus factor crítico |
| N2 · Administrado | Notas aisladas en correos y chats. Nadie sabe dónde buscar la respuesta correcta |
| N3 · Definido | KEDB centralizada, estructurada y con dueño responsable de mantenerla |
| N4 · Cuantitativo | Uso correlacionado con reducción del tiempo de resolución. Retorno medible |
| N5 · Optimizado | Se alimenta automáticamente. IA sugiere la solución antes de que el humano busque |

#### 3.5 Gestión de integraciones y entorno de aplicaciones · Feedback operativo
> Las mesas atienden ecosistemas completos, no aplicaciones aisladas. No saber cómo están integrados los sistemas es causa raíz de muchos incidentes mal resueltos.

| Nivel | Descripción |
|---|---|
| N0 | No aplica como práctica independiente en N0 |
| N1 · Inicial | Sin documentar. Conocimiento informal en pocas personas |
| N2 · Administrado | Lista básica de sistemas sin arquitectura ni dependencias |
| N3 · Definido | Mapa de integraciones: sistemas, APIs, dependencias y owner técnico de cada integración |
| N4 · Cuantitativo | Alertas por criticidad de API afectada. Priorización basada en impacto real |
| N5 · Optimizado | Monitoreo AIOps: detecta caídas de integración antes que el usuario las reporte |

---

### Dimensión 3 · Socios y Proveedores
*Niveles de servicio, contratos y límites del alcance*

#### 3.6 Catálogo de servicios y límites del alcance · ITIL Service

| Nivel | Descripción |
|---|---|
| N0 | No aplica como práctica independiente en N0 |
| N1 · Inicial | Informal, solo verbal. El alcance vive en la cabeza del equipo comercial |
| N2 · Administrado | Firmado y olvidado: desactualizado apenas se firmó el contrato |
| N3 · Definido | Catálogo vivo: el equipo lo conoce y lo usa como referencia real de qué entra y qué no |
| N4 · Cuantitativo | Costeo por servicio: se identifica rentabilidad de cada módulo del catálogo |
| N5 · Optimizado | Ajuste dinámico según demanda real y datos de uso |

#### 3.7 SLA / ANS por prioridad · ITIL Service
> Los ANS se evalúan en dos dimensiones: el acuerdo PS-cliente (externo) y los tiempos por prioridad de ticket.

| Nivel | Descripción |
|---|---|
| N0 | No aplica como práctica independiente en N0 |
| N1 · Inicial | No medidos o aspiracionales. Existen pero nunca se midieron |
| N2 · Administrado | Medición manual e inconsistente, solo cuando el cliente reclama |
| N3 · Definido | Tiempos por prioridad: Crítico <1h · Alto <4h · Medio <8h · Bajo <24h. Reporte mensual |
| N4 · Cuantitativo | Análisis de tendencia, ajuste de metas con patrones reales (picos estacionales) |
| N5 · Optimizado | Alertas predictivas: el sistema avisa que un ANS está en riesgo ANTES de que se incumpla |

**Tiempos de referencia por prioridad (N3 en adelante):**

| Prioridad | Criterio | Tiempo de respuesta | Tiempo de resolución |
|---|---|---|---|
| Crítico | Afecta continuidad del negocio / PDN | < 1 hora | < 4 horas |
| Alto | Afecta múltiples usuarios o proceso crítico | < 4 horas | < 8 horas |
| Medio | Afecta un usuario, tiene workaround | < 8 horas | < 24 horas |
| Bajo | Consulta, solicitud o mejora sin urgencia | < 24 horas | < 72 horas |

#### 3.8 Disponibilidad y cobertura horaria · Feedback operativo

| Nivel | Descripción |
|---|---|
| N0 | N0 activo = cobertura 24x7 automática para solicitudes frecuentes. Sin N0, el servicio tiene horario limitado |
| N1 · Inicial | Best effort: el equipo responde cuando puede, sin compromiso formal |
| N2 · Administrado | Horario conocido por el equipo pero no pactado contractualmente |
| N3 · Definido | Horario definido y pactado (ej. L-V 7:30AM–5PM). GAP administrativo negociado |
| N4 · Cuantitativo | Cumplimiento real de cobertura medido y reportado al cliente con datos |
| N5 · Optimizado | N0/N1 gestionado por IA fuera de horario: 24x7 efectivo sin costo de guardia humana |

---

### Dimensión 4 · Flujos de Valor y Procesos
*Soporte, incidentes, transición y experiencia del cliente*

#### 3.9 Gestión de incidentes · Monitor, Support and Fulfill

| Nivel | Descripción |
|---|---|
| N0 | No aplica como práctica independiente en N0 |
| N1 · Inicial | Reactivo / apagar incendios. Sin trazabilidad de qué pasó ni por qué |
| N2 · Administrado | Registro básico, categorización inconsistente entre agentes |
| N3 · Definido | Proceso estándar de registro, triaje y escalamiento N1→N2→N3 |
| N4 · Cuantitativo | Tiempos medidos por categoría y nivel con metas claras |
| N5 · Optimizado | Auto-resolución IA: clasifica y sugiere, escala solo cuando la confianza del modelo es baja |

#### 3.10 Gestión de solicitudes · Monitor, Support and Fulfill

| Nivel | Descripción |
|---|---|
| N0 · Autoservicio | El portal de N0 resuelve solicitudes frecuentes sin que el usuario abra un ticket ni contacte a nadie |
| N1 · Inicial | Mezcladas con incidentes, sin distinción ni priorización lógica |
| N2 · Administrado | Flujo completamente manual de principio a fin |
| N3 · Definido | Catálogo de solicitudes estándar con tiempos de cumplimiento definidos |
| N4 · Cuantitativo | ANS medido en tiempo real por tipo de solicitud |
| N5 · Optimizado | Portal N0 expandido con IA: resuelve y aprende de cada interacción automáticamente |

#### 3.11 Gestión de problemas (causa raíz) · Monitor, Support and Fulfill

| Nivel | Descripción |
|---|---|
| N0 | No aplica como práctica independiente en N0 |
| N1 · Inicial | No existe. Cada incidente se resuelve aislado como si fuera la primera vez |
| N2 · Administrado | A voluntad del analista, sin proceso formal institucionalizado |
| N3 · Definido | Análisis formal activado cuando un tipo de incidente se repite más de X veces |
| N4 · Cuantitativo | Se mide reducción de tickets recurrentes tras resolver causa raíz |
| N5 · Optimizado | IA detecta patrones ocultos proactivamente, antes del umbral de alerta humana |

#### 3.12 Transición y onboarding · ITIL Service

| Nivel | Descripción |
|---|---|
| N0 | No aplica como práctica independiente en N0 |
| N1 · Inicial | Improvisada. Se reinventa el proceso con cada cliente nuevo |
| N2 · Administrado | Pasos sueltos, no documentados ni replicables por otra persona |
| N3 · Definido | Playbook exacto: inducción, documentación, acuerdos, KEDB inicial |
| N4 · Cuantitativo | Métrica 30 días: calidad del arranque medida con datos reales |
| N5 · Optimizado | Plantillas IA aceleran la transición y reducen riesgo de errores en el arranque |

#### 3.13 Experiencia del cliente (CX / NPS / CSAT) · ITIL Experience

| Nivel | Descripción |
|---|---|
| N0 | Satisfacción medida por tasa de resolución autónoma (% de usuarios que resolvieron sin escalar) |
| N1 · Inicial | Cero quejas = todo OK. No hay mecanismo real de medición |
| N2 · Administrado | Encuesta anual esporádica sin seguimiento a resultados |
| N3 · Definido | CSAT continuo por ticket con seguimiento real a resultados negativos |
| N4 · Cuantitativo | Cruce operacional: CSAT correlacionado con tiempos, reincidencia y NPS |
| N5 · Optimizado | CX en tiempo real: el servicio se ajusta antes de que la insatisfacción se formalice |

---

## 4. Dimensión de negocio

Una mesa puede estar en N4 operativamente y ser poco rentable o estar perdiendo al cliente. Esta dimensión evalúa el éxito de la mesa como negocio para PS.

| Indicador | N1 | N3 | N5 |
|---|---|---|---|
| Salud financiera | Pérdida oculta: margen desconocido | Margen por FTE identificado y monitoreado | Upselling automático: IA detecta oportunidades |
| Retención y cuenta | Riesgo de churn no detectado | Plan de cuenta activo, renovación gestionada | Expansión automática: modelo detecta señales |
| NPS / CSAT | Cliente silencioso | CSAT sistemático, NPS periódico | Predicción de churn antes de la queja |
| Eficiencia de costo | Costo/ticket alto e invisible | Costo/ticket calculado vs. línea base | Automatización escala sola, costo marginal baja |

> Una mesa exitosa cumple ambas dimensiones: madura operativamente (N0–N5) y rentable / valiosa para PS y el cliente.

---

## 5. Capa sectorial: Banca

Complementa las 13 prácticas con criterios bajo supervisión de la **Superintendencia Financiera de Colombia (SFC)**.

| Práctica sectorial | Nivel mínimo | Qué evalúa |
|---|---|---|
| Continuidad de negocio (BCP/DRP) | N3 | ¿Planes de continuidad probados? ¿Simulacros ejecutados? |
| Trazabilidad de cambios (SOX) | N3 | ¿Todo cambio en producción tiene aprobación y trazabilidad? |
| Gestión de incidentes de seguridad | N3 | ¿Proceso diferenciado para fraude o vulnerabilidades? |
| Reportabilidad regulatoria | N4 | ¿La mesa genera evidencia auditable ante la SFC? |
| Segregación de funciones | N3 | ¿Quien atiende, aprueba y despliega están separados? |
| Disponibilidad de canales críticos | N4 | ¿Se mide y reporta disponibilidad de canales transaccionales? |

**Argumento de venta:** "Hoy su mesa opera sin trazabilidad completa de cambios. Eso es exposición regulatoria ante la SFC. Con N3 en adelante, cada cambio queda documentado y auditable."

---

## 6. Capa sectorial: Salud (EPS)

Complementa las 13 prácticas con criterios bajo **Supersalud** y la Ley 1581 de 2012 (Habeas Data en salud).

| Práctica sectorial | Nivel mínimo | Qué evalúa |
|---|---|---|
| Protección de datos sensibles de salud | N3 | ¿Acceso a historia clínica controlado y auditado individualmente? |
| Continuidad de servicios asistenciales | N3 | ¿Protocolos diferenciados para incidentes que afectan atención al paciente? |
| Trazabilidad clínica | N3 | ¿Todo cambio en historia clínica queda registrado y auditable? |
| Incidentes con impacto asistencial | N3 | ¿Clasificación diferenciada entre ticket admin y uno que afecta un paciente? |
| Interoperabilidad | N3 | ¿Los sistemas cumplen estándares RIPS / PISIS del Ministerio de Salud? |

**Argumento de venta:** "Un problema de autorización urgente puede esperar en la misma fila que un reseteo de contraseña. Con N3, los incidentes asistenciales se priorizan automáticamente."

---

## 7. Aplicación comercial

### 7.1 Flujo de uso en conversación de venta

1. **Clasificar** — ¿Mesa de Ayuda o Mesa de Soporte? ¿Tiene N0 activo?
2. **Evaluar** — Aplicar el instrumento Excel (13 prácticas + negocio, escala N0–N5)
3. **Diagnosticar** — Identificar prácticas por debajo del mínimo esperado (marcadas en rojo)
4. **Visualizar** — Mostrar el radar chart con perfil actual vs. objetivo
5. **Presentar roadmap** — Qué cambia en el negocio en cada salto de nivel
6. **Conectar con valor** — Menos tickets, menos riesgo regulatorio, mejor experiencia
7. **Activar capa sectorial** — Si aplica banca o salud, agregar criterios regulatorios como diferenciador

### 7.2 Conexión con el plan general del servicio

Este modelo es el insumo de entrada de la **Fase 4 (Transición de clientes actuales)**: antes de proponer la migración de una mesa al nuevo modelo, se aplica esta evaluación para tener evidencia objetiva del punto de partida y construir el caso de negocio.

---

## 8. Próximos pasos

1. **Pilotar el clasificador** en las mesas actuales, incluyendo verificar si tienen N0 activo
2. **Aplicar el instrumento v2.2** en al menos una mesa de banca y una de salud para calibrar la rúbrica
3. **Validar los tiempos de ANS** por prioridad con el equipo de delivery
4. **Construir el slide deck comercial** con el radar chart y el argumento por sector
5. **Definir estándar de mercado esperado** por tipo de mesa y sector como referencia comparativa
6. **Integrar con Fase 4** del plan de diseño como condición de entrada para la propuesta de transición
7. **Explorar capa sectorial para Centro América** (Curasao y otros) con sus particularidades regulatorias
