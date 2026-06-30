# Modelo de Madurez de Mesas de Servicio · v2.1
**PersonalSoft · ITIL v5 · 4 dimensiones · 13 prácticas + negocio + capa sectorial**

---

## 1. Propósito del modelo

Este modelo tiene un doble uso: **diagnosticar** el estado real de cualquier mesa de servicio (propia o de un cliente), y servir como **herramienta comercial** para mostrarle al cliente dónde está parado hoy y qué gana al evolucionar.

El modelo tiene tres capas:
- **Clasificador inicial** — determina si la mesa es de Ayuda o de Soporte, definiendo el nivel mínimo esperado
- **13 prácticas operativas** — organizadas por las 4 dimensiones reales de ITIL v5
- **Dimensión de negocio** — evalúa si la mesa es exitosa como negocio, no solo como operación
- **Capa sectorial** — profundización regulatoria para banca (SFC/SOX) y salud (Supersalud/Habeas Data)

### 1.1 Clasificador inicial

| Aspecto | Mesa de Ayuda | Mesa de Soporte |
|---|---|---|
| Nivel de servicio | Básico (Nivel 1) | Avanzado (Niveles 2 y 3) |
| Tipo de atención | Reactiva | Reactiva y proactiva |
| Complejidad | Baja | Media y alta |
| Perfil del equipo | Junior · Atención al usuario | Técnico especializado / Senior |
| Enfoque | Usuario final | Tecnología y continuidad |
| ¿Incluye causa raíz? | No | Sí |
| ¿KPIs de desempeño? | Básicos | Completos con tendencias |
| Roles típicos | Analista de soporte | Coordinador · Líder técnico · Desarrollador |
| **Nivel mínimo esperado** | **2 · Administrado** | **3 · Definido** |

---

## 2. Los cinco niveles de madurez

| Nivel | Nombre | Qué caracteriza | Riesgo principal |
|---|---|---|---|
| 1 | Inicial | Reactivo total. Depende de personas, no de procesos | Bus factor: si se va la persona, se va el conocimiento |
| 2 | Administrado | Procesos por mesa, sin estandarizar entre clientes | No escala: cada nueva mesa reinventa el proceso |
| 3 | Definido | Procesos documentados y consistentes entre mesas | Sin datos, no se puede demostrar que el servicio mejora |
| 4 | Cuantitativo | Gestión basada en datos: SLA medidos, KPIs reales | Alto costo en horas-persona para mantener la medición |
| 5 | Optimizado | IA y automatización activas, anticipación de problemas | Sin gobierno de IA, la automatización falla a escala |

### Nivel 1 · Inicial
La mesa funciona pero depende de personas específicas. No hay documentación, los criterios cambian según quién atiende. El cliente percibe el servicio como impredecible y no puede medir si está recibiendo lo que paga.

### Nivel 2 · Administrado
Existen procesos pero viven dentro de cada mesa de forma aislada. La herramienta de tickets se usa solo como bitácora. Los reportes se arman manualmente. El cliente nota regularidad pero no puede comparar contra ningún estándar.

### Nivel 3 · Definido
Los procesos están documentados y se replican entre mesas. Existe catálogo de servicios, RACI explícito y metodología común. El cliente empieza a confiar porque puede anticipar tiempos de respuesta y entender el alcance exacto.

### Nivel 4 · Administrado cuantitativamente
La mesa se gestiona con datos reales. Los SLA se miden sistemáticamente. Hay tendencias analizadas y decisiones basadas en evidencia. El cliente recibe evidencia objetiva del desempeño y puede tomar decisiones de negocio con datos.

### Nivel 5 · Optimizado
La mesa incorpora IA y automatización en el flujo diario. El foco pasa de "resolver rápido" a "anticipar antes de que el cliente note el problema". Es el nivel al que apunta la Mesa de Servicios de Nueva Generación con IA.

---

## 3. Las 13 prácticas organizadas por las 4 dimensiones de ITIL v5

### Dimensión 1 · Organizaciones y Personas
*Gobierno, roles y cultura del equipo*

#### 3.1 Gobierno de roles (RACI)
> Origen: feedback operativo real. La ausencia de roles claros genera decisiones arbitrarias y escalamientos mal dirigidos.

| Nivel | Descripción |
|---|---|
| 1 · Inicial | Héroes aislados. Cualquiera hace cualquier cosa según disponibilidad |
| 2 · Administrado | Roles informales conocidos por el equipo, sin documentación ni RACI |
| 3 · Definido | RACI documentado: Coordinador de Servicio, Líder Técnico, Especialista / Desarrollador |
| 4 · Cuantitativo | Desempeño medido por rol, RACI ajustado con datos reales de carga |
| 5 · Optimizado | IA sugiere reasignación de tickets según carga, especialidad y disponibilidad |

#### 3.2 Capacidad y dimensionamiento del equipo
| Nivel | Descripción |
|---|---|
| 1 · Inicial | Cálculo a ojo, sin datos de carga real. Frecuentemente sub o sobre dimensionado |
| 2 · Administrado | Criterio estático que no se revisa aunque la realidad del cliente haya cambiado |
| 3 · Definido | Calculadora FTE basada en volumen histórico real de tickets |
| 4 · Cuantitativo | Se mide % de tiempo muerto (GAP) por persona y se ajusta la capacidad con datos |
| 5 · Optimizado | Dimensionamiento dinámico: IA anticipa picos antes de que ocurran |

---

### Dimensión 2 · Información y Tecnología
*Herramientas, automatización y datos*

#### 3.3 Herramientas y automatización
| Nivel | Descripción |
|---|---|
| 1 · Inicial | Dispersas: correo, Excel, chats personales sin ninguna integración |
| 2 · Administrado | Herramienta de tickets pero usada solo como bitácora, sin automatización |
| 3 · Definido | Flujos integrados: escalamiento y notificación automática, menos trabajo manual |
| 4 · Cuantitativo | Se mide % de automatización del flujo y su impacto en tiempos de resolución |
| 5 · Optimizado | Agentes de IA clasifican, sugieren y en algunos casos resuelven tickets automáticamente |

#### 3.4 Gestión del conocimiento (KEDB)
| Nivel | Descripción |
|---|---|
| 1 · Inicial | En la cabeza de personas clave. Bus factor crítico |
| 2 · Administrado | Notas aisladas en correos y chats. Nadie sabe dónde buscar la respuesta correcta |
| 3 · Definido | KEDB centralizada, estructurada y con dueño responsable de mantenerla |
| 4 · Cuantitativo | Uso correlacionado con reducción del tiempo de resolución. Retorno medible |
| 5 · Optimizado | Se alimenta automáticamente. IA sugiere la solución antes de que el humano busque |

#### 3.5 Gestión de integraciones y entorno de aplicaciones
> Origen: feedback operativo. Las mesas atienden ecosistemas completos (Canal Asesor, Masivos, Digital Venta, etc.) y no saber cómo están integrados es causa raíz de muchos incidentes mal resueltos.

| Nivel | Descripción |
|---|---|
| 1 · Inicial | Sin documentar. Conocimiento informal en pocas personas |
| 2 · Administrado | Lista básica de sistemas sin arquitectura ni dependencias |
| 3 · Definido | Mapa de integraciones: sistemas, APIs, dependencias y owner técnico de cada integración |
| 4 · Cuantitativo | Alertas por criticidad de API afectada. Priorización basada en impacto real |
| 5 · Optimizado | Monitoreo AIOps: detecta caídas de integración antes que el usuario las reporte |

---

### Dimensión 3 · Socios y Proveedores
*Niveles de servicio, contratos y límites del alcance*

#### 3.6 Catálogo de servicios y límites del alcance
| Nivel | Descripción |
|---|---|
| 1 · Inicial | Informal, solo verbal. El alcance vive en la cabeza del equipo comercial |
| 2 · Administrado | Firmado y olvidado: desactualizado apenas se firmó el contrato |
| 3 · Definido | Catálogo vivo: el equipo lo conoce y lo usa como referencia real de qué entra y qué no |
| 4 · Cuantitativo | Costeo por servicio: se identifica rentabilidad de cada módulo del catálogo |
| 5 · Optimizado | Ajuste dinámico según demanda real y datos de uso |

#### 3.7 SLA / ANS por prioridad
> Los ANS se evalúan en dos dimensiones: el SLA externo (acuerdo PS-cliente) y los tiempos por prioridad de ticket (Crítico · Alto · Medio · Bajo).

| Nivel | Descripción |
|---|---|
| 1 · Inicial | No medidos o aspiracionales. Existen pero nunca se midieron desde que se firmaron |
| 2 · Administrado | Medición manual e inconsistente, solo cuando el cliente reclama |
| 3 · Definido | Tiempos definidos por prioridad: Crítico <1h · Alto <4h · Medio <8h · Bajo <24h. Reporte mensual sistemático |
| 4 · Cuantitativo | Análisis de tendencia, ajuste de metas con patrones reales (picos estacionales, cambios de volumen) |
| 5 · Optimizado | Alertas predictivas: el sistema avisa que un ANS está en riesgo ANTES de que se incumpla |

**Tiempos de referencia por prioridad (nivel 3 en adelante):**

| Prioridad | Criterio | Tiempo de respuesta | Tiempo de resolución |
|---|---|---|---|
| Crítico | Afecta continuidad del negocio / PDN caído | < 1 hora | < 4 horas |
| Alto | Afecta a múltiples usuarios o proceso crítico | < 4 horas | < 8 horas |
| Medio | Afecta a un usuario, tiene workaround | < 8 horas | < 24 horas |
| Bajo | Consulta, solicitud o mejora sin urgencia | < 24 horas | < 72 horas |

#### 3.8 Disponibilidad y cobertura horaria
> Origen: feedback operativo. El horario no es un detalle operativo — es un compromiso contractual y un diferenciador comercial.

| Nivel | Descripción |
|---|---|
| 1 · Inicial | Best effort: el equipo responde cuando puede, sin compromiso formal |
| 2 · Administrado | Horario conocido por el equipo pero no pactado contractualmente con el cliente |
| 3 · Definido | Horario definido y pactado (ej. L-V 7:30AM–5PM). GAP administrativo negociado |
| 4 · Cuantitativo | Cumplimiento real de cobertura medido y reportado al cliente con datos |
| 5 · Optimizado | N0/N1 gestionado por IA fuera de horario: 24x7 efectivo sin costo de guardia humana |

---

### Dimensión 4 · Flujos de Valor y Procesos
*Soporte, incidentes, transición y experiencia del cliente*

#### 3.9 Gestión de incidentes
| Nivel | Descripción |
|---|---|
| 1 · Inicial | Reactivo / apagar incendios. Sin trazabilidad de qué pasó ni por qué |
| 2 · Administrado | Registro básico, categorización inconsistente entre agentes |
| 3 · Definido | Proceso estándar de registro, triaje y escalamiento N1→N2→N3 |
| 4 · Cuantitativo | Tiempos medidos por categoría y nivel con metas claras |
| 5 · Optimizado | Auto-resolución IA: clasifica y sugiere, escala solo cuando la confianza del modelo es baja |

#### 3.10 Gestión de solicitudes
| Nivel | Descripción |
|---|---|
| 1 · Inicial | Mezcladas con incidentes, sin distinción ni priorización lógica |
| 2 · Administrado | Flujo completamente manual de principio a fin |
| 3 · Definido | Catálogo de solicitudes estándar con tiempos de cumplimiento definidos |
| 4 · Cuantitativo | SLA medido en tiempo real por tipo de solicitud |
| 5 · Optimizado | Portal de autoservicio N0: resuelve solicitudes frecuentes sin intervención humana |

#### 3.11 Gestión de problemas (causa raíz)
| Nivel | Descripción |
|---|---|
| 1 · Inicial | No existe. Cada incidente se resuelve aislado como si fuera la primera vez |
| 2 · Administrado | A voluntad del analista, sin proceso formal institucionalizado |
| 3 · Definido | Análisis formal activado cuando un tipo de incidente se repite más de X veces |
| 4 · Cuantitativo | Se mide reducción de tickets recurrentes tras resolver causa raíz |
| 5 · Optimizado | IA detecta patrones ocultos proactivamente, antes del umbral de alerta humana |

#### 3.12 Transición y onboarding
| Nivel | Descripción |
|---|---|
| 1 · Inicial | Improvisada. Se reinventa el proceso con cada cliente nuevo |
| 2 · Administrado | Pasos sueltos, no documentados ni replicables por otra persona |
| 3 · Definido | Playbook exacto: inducción, documentación, acuerdos, KEDB inicial |
| 4 · Cuantitativo | Métrica 30 días: calidad del arranque medida con datos reales |
| 5 · Optimizado | Carga automática: plantillas IA aceleran la transición y reducen riesgo de errores |

#### 3.13 Experiencia del cliente (CX / NPS / CSAT)
| Nivel | Descripción |
|---|---|
| 1 · Inicial | Cero quejas = todo OK. No hay mecanismo real de medición |
| 2 · Administrado | Encuesta anual esporádica sin seguimiento a resultados |
| 3 · Definido | CSAT continuo por ticket con seguimiento real a resultados negativos |
| 4 · Cuantitativo | Cruce operacional: CSAT correlacionado con tiempos, reincidencia y NPS |
| 5 · Optimizado | CX en tiempo real: el servicio se ajusta antes de que la insatisfacción se formalice |

---

## 4. Dimensión de negocio

Una mesa puede estar en nivel 4 operativamente y ser poco rentable o estar perdiendo al cliente. Esta dimensión evalúa el éxito de la mesa **como negocio para PS**, no solo como operación.

| Indicador | Nivel 1 | Nivel 3 | Nivel 5 |
|---|---|---|---|
| Salud financiera | Pérdida oculta: margen desconocido | Margen por FTE identificado y monitoreado | Upselling automático: IA detecta oportunidades |
| Retención y cuenta | Riesgo de churn no detectado | Plan de cuenta activo, renovación gestionada | Expansión automática: modelo detecta señales |
| NPS / CSAT | Cliente silencioso | CSAT sistemático, NPS periódico | Predicción de churn antes de la queja |
| Eficiencia de costo | Costo/ticket alto e invisible | Costo/ticket calculado vs. línea base | Automatización escala sola, costo marginal baja |

> **Una mesa exitosa cumple ambas dimensiones:** madura operativamente (ITIL v5) y rentable / valiosa para PS y el cliente.

---

## 5. Capa sectorial: Banca

Para clientes de banca, el modelo general se complementa con criterios bajo la supervisión de la **Superintendencia Financiera de Colombia (SFC)**.

| Práctica sectorial | Nivel mínimo requerido | Qué evalúa |
|---|---|---|
| Continuidad de negocio (BCP/DRP) | 3 · Definido | ¿Planes de continuidad probados? ¿Simulacros ejecutados? |
| Trazabilidad de cambios (SOX) | 3 · Definido | ¿Todo cambio en producción tiene aprobación y trazabilidad? |
| Gestión de incidentes de seguridad | 3 · Definido | ¿Proceso diferenciado para fraude o vulnerabilidades? |
| Reportabilidad regulatoria | 4 · Cuantitativo | ¿La mesa genera evidencia auditable ante un requerimiento SFC? |
| Segregación de funciones | 3 · Definido | ¿Quien atiende, aprueba y despliega están claramente separados? |
| Disponibilidad de canales críticos | 4 · Cuantitativo | ¿Se mide y reporta disponibilidad de canales transaccionales? |

**Argumento de venta:** "Hoy su mesa opera sin trazabilidad completa de cambios. Eso representa exposición regulatoria ante la SFC. Con el modelo de Nivel 3 en adelante, cada cambio queda documentado y auditable."

---

## 6. Capa sectorial: Salud (EPS)

Para clientes de salud, el modelo se complementa con criterios bajo la **Superintendencia Nacional de Salud (Supersalud)** y la Ley 1581 de 2012 (Habeas Data en salud).

| Práctica sectorial | Nivel mínimo requerido | Qué evalúa |
|---|---|---|
| Protección de datos sensibles de salud | 3 · Definido | ¿Acceso a historia clínica controlado y auditado individualmente? |
| Continuidad de servicios asistenciales | 3 · Definido | ¿Protocolos diferenciados para incidentes que afectan atención al paciente? |
| Trazabilidad clínica | 3 · Definido | ¿Todo cambio en historia clínica queda registrado y es auditable? |
| Incidentes con impacto asistencial | 3 · Definido | ¿Hay clasificación diferenciada entre ticket admin y uno que afecta un paciente? |
| Interoperabilidad | 3 · Definido | ¿Los sistemas cumplen estándares RIPS / PISIS del Ministerio de Salud? |

**Argumento de venta:** "Actualmente un problema de autorización de un procedimiento urgente puede esperar en la misma fila que un reseteo de contraseña. Con Nivel 3, los incidentes asistenciales se priorizan automáticamente."

---

## 7. Aplicación comercial

### 7.1 Flujo de uso en conversación de venta

1. **Clasificar** — ¿Mesa de Ayuda o Mesa de Soporte? Define el nivel mínimo esperado
2. **Evaluar** — Aplicar el instrumento Excel a la mesa actual del cliente (13 prácticas + negocio)
3. **Diagnosticar** — Identificar qué prácticas están por debajo del mínimo esperado (marcadas en rojo)
4. **Visualizar** — Mostrar el radar chart con el perfil actual vs. el objetivo
5. **Presentar el roadmap** — Qué cambia en el negocio en cada salto de nivel
6. **Conectar con valor** — Menos tickets recurrentes, menos riesgo regulatorio, mejor experiencia del usuario
7. **Activar capa sectorial** — Si aplica banca o salud, agregar los criterios regulatorios como diferenciador

### 7.2 Conexión con el plan general del servicio

Este modelo es el insumo de entrada de la **Fase 4 (Transición de clientes actuales)**: antes de proponer la migración de una mesa al nuevo modelo, se aplica esta evaluación para tener evidencia objetiva del punto de partida y construir el caso de negocio de la transición.

---

## 8. Próximos pasos

1. **Pilotar el clasificador** en las mesas actuales para definir si cada una es de Ayuda o Soporte
2. **Aplicar el instrumento v2.1** (Excel) en al menos una mesa de banca y una de salud para calibrar la rúbrica
3. **Validar los tiempos de ANS** por prioridad (Crítico/Alto/Medio/Bajo) con el equipo de delivery
4. **Construir el slide deck comercial** que traduce el modelo en argumento de venta con el radar chart
5. **Definir el estándar de mercado esperado** por sector como referencia comparativa
6. **Integrar con Fase 4** del plan de diseño: diagnóstico de madurez como condición de entrada para la propuesta de transición
7. **Explorar capa sectorial para Centro América** (Curasao y otros) con sus particularidades regulatorias
