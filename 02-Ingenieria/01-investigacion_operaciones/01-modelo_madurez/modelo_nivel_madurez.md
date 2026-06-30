# Modelo de Madurez de Mesas de Servicio · v2
**PersonalSoft · Basado en ITIL v5 · 13 prácticas + clasificador + dimensión de negocio**

---

## 1. Propósito del modelo

Este modelo tiene un doble uso: permite a PersonalSoft **diagnosticar** el estado real de cualquier mesa de servicio (propia o de un cliente), y sirve como **herramienta comercial** para mostrarle al cliente, con evidencia y lenguaje claro, dónde está parado hoy y qué gana al evolucionar.

El modelo es agnóstico por diseño, pero incorpora dos capas adicionales:

- **Clasificador inicial:** antes de evaluar cualquier práctica, se determina si la mesa es de **Ayuda** (N1, reactiva, baja complejidad) o de **Soporte** (N2-N3, proactiva, técnico especializado). Esto define el nivel mínimo de madurez esperado.
- **Capa sectorial:** profundización para los dos mercados prioritarios (**banca** y **salud / EPS**), con criterios regulatorios específicos que complementan las 13 prácticas generales.

### Clasificador inicial: Mesa de Ayuda vs Mesa de Soporte

| Aspecto | Mesa de Ayuda | Mesa de Soporte |
|---|---|---|
| Nivel de servicio | Básico (Nivel 1) | Avanzado (Niveles 2 y 3) |
| Tipo de atención | Reactiva | Reactiva y proactiva |
| Complejidad de casos | Baja | Media y alta |
| Perfil técnico del equipo | Atención al usuario / Junior | Técnico especializado / Senior |
| Enfoque principal | Usuario final | Tecnología y continuidad del servicio |
| Nivel mínimo esperado (madurez) | Nivel 2 · Administrado | Nivel 3 · Definido |
| ¿Incluye causa raíz y análisis técnico? | No | Sí |
| ¿Incluye KPIs de desempeño del equipo? | Básicos | Completos con tendencias |
| Roles típicos | Analista de soporte | Coordinador de servicio · Líder técnico · Desarrollador |

---

## 2. Los cinco niveles de madurez, en profundidad

Cada nivel no es solo una etiqueta — describe un estado real y reconocible del servicio, con comportamientos típicos, riesgos asociados y lo que el cliente experimenta.

### Nivel 1 · Inicial

**Qué caracteriza este nivel**
La mesa funciona, pero su funcionamiento depende casi exclusivamente de personas específicas, no de procesos. No hay documentación consistente, los criterios de priorización cambian según quién atiende, y la organización no tiene visibilidad real de qué está pasando dentro de la mesa más allá de "se resolvió o no se resolvió".

**Comportamientos típicos**
- Los tickets se resuelven, pero nadie sabe cuántos hay realmente ni cuánto tardan en promedio
- Si la persona que "sabe" se va de vacaciones o renuncia, el servicio se degrada visiblemente
- No existe un lugar único donde esté documentado cómo resolver los problemas comunes
- Las solicitudes y los incidentes se mezclan sin distinción

**Qué experimenta el cliente**
Percibe el servicio como impredecible: a veces rápido, a veces lento, sin explicación clara de por qué. No tiene forma de medir si está recibiendo lo que está pagando.

**Riesgo principal**
Dependencia crítica de personas individuales (bus factor). Alta rotación = alto riesgo de pérdida de continuidad del servicio.

---

### Nivel 2 · Administrado

**Qué caracteriza este nivel**
Ya existen procesos, pero viven dentro de cada mesa de forma aislada — no hay un estándar que se replique entre clientes o entre equipos. Hay algo de documentación, pero desactualizada o incompleta. Las decisiones todavía se toman mayormente por intuición, no por datos.

**Comportamientos típicos**
- Cada mesa tiene "su manera" de hacer las cosas, distinta a la mesa de al lado
- Existe una herramienta de tickets, pero se usa solo como bitácora, no como motor de gestión
- Hay reportes, pero se arman manualmente y consumen tiempo desproporcionado
- El conocimiento se transmite de boca a boca entre el equipo, no por escrito

**Qué experimenta el cliente**
Empieza a notar cierta regularidad, pero sigue sin tener visibilidad comparativa: no puede saber si su mesa funciona mejor o peor que el estándar del mercado, porque no hay estándar.

**Riesgo principal**
Falta de escalabilidad. Cada nuevo cliente o nueva mesa requiere reinventar el proceso desde cero.

---

### Nivel 3 · Definido

**Qué caracteriza este nivel**
Los procesos están documentados, son consistentes y se replican de una mesa a otra. Existe un catálogo de servicios claro, roles definidos con un RACI explícito, y una metodología común que no depende de quién esté operando. Este es el primer nivel donde se puede hablar de "servicio estandarizado" en lugar de "buena voluntad operativa".

**Comportamientos típicos**
- Catálogo de servicios formal, con descripciones claras de qué incluye y qué no
- Niveles de servicio (SLA) documentados y conocidos por el equipo y el cliente
- Proceso de transición estándar para arrancar con clientes nuevos
- KEDB (base de errores conocidos) estructurada y mantenida

**Qué experimenta el cliente**
Empieza a confiar en el servicio porque puede anticipar tiempos de respuesta y entender el alcance exacto de lo que está contratando. Las conversaciones dejan de ser reactivas ("¿por qué se tardó tanto?") y pasan a ser de seguimiento ("¿estamos cumpliendo el SLA?").

**Riesgo principal**
Sin medición cuantitativa, sigue sin poder demostrarse objetivamente que el servicio mejora con el tiempo.

---

### Nivel 4 · Administrado cuantitativamente

**Qué caracteriza este nivel**
La mesa se gestiona con datos reales, no con percepción. Los SLA no solo están pactados — se miden de forma sistemática. Hay tendencias analizadas, metas concretas y decisiones de mejora basadas en evidencia. Este es el nivel donde el servicio se vuelve gestionable como un activo, no solo operable como una función.

**Comportamientos típicos**
- Dashboard de KPIs actualizado, con metas claras por indicador
- Análisis de causa raíz sistemático para incidentes recurrentes
- Medición del % de tiempo muerto del equipo (GAP) y ajuste de capacidad basado en eso
- Reportes mensuales con tendencias, no solo fotos del mes

**Qué experimenta el cliente**
Recibe evidencia objetiva del desempeño del servicio. Puede tomar decisiones de negocio (renovar, ampliar, renegociar) basado en datos reales en lugar de percepción subjetiva.

**Riesgo principal**
Sin automatización, el costo de mantener este nivel de medición y análisis empieza a ser alto en horas-persona.

---

### Nivel 5 · Optimizado

**Qué caracteriza este nivel**
La mesa incorpora inteligencia artificial y automatización de forma activa en el flujo diario. El foco deja de ser "resolver rápido" y pasa a ser "anticipar antes de que el cliente note el problema". Es el nivel al que apunta la Mesa de Servicios de Nueva Generación con IA.

**Comportamientos típicos**
- Clasificación automática de tickets, sin intervención humana en el triaje inicial
- Sugerencia automática de soluciones antes de escalar (apoyada en la base de conocimiento)
- Monitoreo predictivo (AIOps) que detecta anomalías antes de que generen incidente
- El equipo humano se enfoca en lo que requiere juicio, no en tareas repetitivas

**Qué experimenta el cliente**
El servicio deja de sentirse como "soporte" y empieza a sentirse como un socio tecnológico activo que mejora continuamente sin que el cliente tenga que pedirlo.

**Riesgo principal**
Gobierno de IA insuficiente. Sin human-in-the-loop bien diseñado, la automatización puede generar errores a escala en lugar de valor.

---

## 3. Las trece prácticas, nivel por nivel

### Prácticas operativas · Monitor, Support and Fulfill

### 3.1 Gestión de incidentes

| Nivel | Qué implica este nivel |
|---|---|
| 1 · Inicial | Resolución ad hoc. El éxito depende de la memoria y experiencia individual del agente. No hay trazabilidad de qué pasó ni por qué se resolvió de cierta forma. |
| 2 · Administrado | Se registra el incidente, pero la categorización varía según quién lo registra. Imposible sacar reportes confiables porque los datos no son comparables. |
| 3 · Definido | Proceso de registro, categorización y escalamiento documentado. Cualquier persona nueva puede seguir el proceso sin depender de un mentor informal. |
| 4 · Cuantitativo | Se mide tiempo de resolución por categoría, se identifican cuellos de botella con datos y se ajustan procesos basados en esa evidencia. |
| 5 · Optimizado | El sistema clasifica el incidente automáticamente, sugiere la solución más probable y solo escala a humano cuando la confianza del modelo es baja. |

### 3.2 Gestión de solicitudes / peticiones

| Nivel | Qué implica este nivel |
|---|---|
| 1 · Inicial | No hay diferencia entre un incidente (algo que falló) y una solicitud (algo que se pide). Todo entra al mismo embudo sin priorización lógica. |
| 2 · Administrado | Se distingue solicitud de incidente, pero cada solicitud se atiende manualmente de principio a fin. |
| 3 · Definido | Existe un catálogo de solicitudes estándar con tiempos de cumplimiento definidos y conocidos por el usuario final. |
| 4 · Cuantitativo | Se mide el cumplimiento real contra el SLA pactado para cada tipo de solicitud, con reporte de tendencia al cliente. |
| 5 · Optimizado | Un portal de autoservicio (N0) resuelve las solicitudes más frecuentes sin intervención humana. |

### 3.3 Gestión de problemas (causa raíz)

| Nivel | Qué implica este nivel |
|---|---|
| 1 · Inicial | Cada incidente se apaga como un incendio aislado. Si el mismo problema vuelve la semana siguiente, se trata como si fuera la primera vez. |
| 2 · Administrado | A veces se investiga la causa raíz, pero depende de la motivación individual del analista, no de un proceso formal. |
| 3 · Definido | Existe un proceso formal: cuando un tipo de incidente se repite más de X veces, se activa un análisis de causa raíz documentado. |
| 4 · Cuantitativo | Se mide objetivamente cuánto se reduce el volumen de tickets recurrentes tras resolver la causa raíz, demostrando el retorno de la inversión. |
| 5 · Optimizado | La IA detecta patrones de causa raíz de forma proactiva, antes de que el volumen de tickets alcance un umbral de alerta humana. |

### 3.4 Gestión del conocimiento (KEDB)

| Nivel | Qué implica este nivel |
|---|---|
| 1 · Inicial | El conocimiento crítico vive únicamente en la cabeza de un puñado de personas. Es el riesgo organizacional más alto de este nivel. |
| 2 · Administrado | Hay documentación, pero dispersa en correos, chats y notas personales — nadie sabe con certeza dónde buscar la respuesta correcta. |
| 3 · Definido | Existe una base de conocimiento (KEDB) centralizada, estructurada y con un dueño responsable de mantenerla actualizada. |
| 4 · Cuantitativo | Se mide cuánto se usa la base de conocimiento y cómo correlaciona con la reducción del tiempo de resolución. |
| 5 · Optimizado | La base de conocimiento se alimenta automáticamente con cada ticket resuelto, y un agente de IA sugiere la solución antes de que el humano tenga que buscarla. |

---

### Prácticas operativas · ITIL Service

### 3.5 Catálogo de servicios y límites del alcance

| Nivel | Qué implica este nivel |
|---|---|
| 1 · Inicial | El alcance del servicio existe solo en la cabeza del equipo comercial — nunca se formalizó por escrito. |
| 2 · Administrado | Hay un catálogo, pero quedó desactualizado apenas se firmó el contrato; nadie lo revisa ni lo usa. |
| 3 · Definido | El catálogo está vivo: se actualiza, el equipo lo conoce y lo usa como referencia real para decidir qué entra y qué no entra en el alcance. |
| 4 · Cuantitativo | Se mide el uso real de cada servicio del catálogo, identificando cuáles generan valor y cuáles casi no se usan. |
| 5 · Optimizado | El catálogo se ajusta dinámicamente: si la demanda de un servicio crece, el modelo sugiere ajuste de capacidad o de tarifa. |

### 3.6 Niveles de servicio (SLA / ANS)

| Nivel | Qué implica este nivel |
|---|---|
| 1 · Inicial | No hay SLA, o si los hay, son aspiracionales — nunca se midieron desde que se firmaron. |
| 2 · Administrado | Se pactaron SLA, pero la medición es manual, inconsistente y se hace solo cuando el cliente reclama. |
| 3 · Definido | El SLA se mide sistemáticamente y se reporta al cliente de forma periódica y predecible. |
| 4 · Cuantitativo | Se analiza la tendencia de cumplimiento y se ajustan metas o recursos basado en patrones reales (ej. picos estacionales). |
| 5 · Optimizado | Alertas predictivas avisan al equipo que un SLA está en riesgo de incumplirse ANTES de que ocurra. |

### 3.7 Transición y onboarding de servicios

| Nivel | Qué implica este nivel |
|---|---|
| 1 · Inicial | Cada arranque con un cliente nuevo es una improvisación total — se reinventa el proceso cada vez. |
| 2 · Administrado | Hay algunos pasos básicos que se siguen, pero no están escritos ni son replicables por otra persona. |
| 3 · Definido | Existe un playbook estándar de transición (inducción, documentación, acuerdos) que cualquier líder de cuenta puede ejecutar. |
| 4 · Cuantitativo | Se mide el tiempo de transición y la calidad del arranque (volumen de tickets en los primeros 30 días vs. el mes 4). |
| 5 · Optimizado | Plantillas inteligentes y checklists automatizados aceleran la transición, reduciendo el tiempo de arranque. |

---

### Prácticas operativas · ITIL Experience

### 3.8 Satisfacción y experiencia del cliente

| Nivel | Qué implica este nivel |
|---|---|
| 1 · Inicial | Se asume que "si no hay quejas, todo está bien" — no hay ningún mecanismo real de medición. |
| 2 · Administrado | Se hacen encuestas de vez en cuando, sin proceso sistemático ni seguimiento a los resultados. |
| 3 · Definido | Existe una encuesta de satisfacción (CSAT) sistemática, con seguimiento real cuando el resultado es negativo. |
| 4 · Cuantitativo | Se correlaciona el CSAT con otros indicadores operativos (tiempo de resolución, reincidencia, NPS) para entender qué impacta la percepción del cliente. |
| 5 · Optimizado | La experiencia del cliente se monitorea en tiempo real, y el servicio se ajusta proactivamente antes de que la insatisfacción se convierta en queja formal. |

---

### Prácticas operativas · ITIL Foundation

### 3.9 Capacidad y dimensionamiento del equipo

| Nivel | Qué implica este nivel |
|---|---|
| 1 · Inicial | El equipo se dimensiona "a ojo", sin datos de carga real — frecuentemente sub o sobre dimensionado. |
| 2 · Administrado | Hay algún criterio inicial de dimensionamiento, pero nunca se revisa con el tiempo. |
| 3 · Definido | Existe una calculadora o modelo de estimación basado en volumen histórico real de tickets. |
| 4 · Cuantitativo | Se mide el % de tiempo muerto (GAP) por persona y se ajusta la capacidad con datos, optimizando costo sin sacrificar calidad. |
| 5 · Optimizado | El dimensionamiento se ajusta dinámicamente según la demanda predicha por modelos de IA, anticipando picos antes de que ocurran. |

### 3.10 Herramientas y automatización

| Nivel | Qué implica este nivel |
|---|---|
| 1 · Inicial | Las herramientas están dispersas (correo, Excel, chats personales) sin ninguna integración entre sí. |
| 2 · Administrado | Hay una herramienta de tickets, pero se usa solo para registrar — no automatiza ningún flujo. |
| 3 · Definido | La herramienta está integrada con flujos de escalamiento y notificación automática, reduciendo el trabajo manual del agente. |
| 4 · Cuantitativo | Se mide el % de automatización real del flujo de trabajo y su impacto en los tiempos de resolución. |
| 5 · Optimizado | Agentes de IA conectados a la herramienta clasifican, sugieren y en algunos casos resuelven tickets automáticamente. |

---

### Prácticas nuevas · Identificadas del feedback operativo real

### 3.11 Gobierno de roles (RACI)

> **Por qué es práctica independiente:** en las mesas actuales se detectó que la ausencia de roles claros (quién coordina, quién lidera técnicamente, quién es especialista) genera decisiones arbitrarias, escalamientos mal dirigidos y falta de rendición de cuentas. Un buen RACI es condición necesaria para que las demás prácticas funcionen.

| Nivel | Qué implica este nivel |
|---|---|
| 1 · Inicial | No hay roles definidos. Cualquier persona hace cualquier cosa según disponibilidad o voluntad. |
| 2 · Administrado | Roles informales y conocidos por el equipo, pero sin documentación ni RACI formal. |
| 3 · Definido | Roles documentados con RACI explícito: Coordinador de Servicio, Líder Técnico de Equipo, Especialista / Desarrollador. Cada uno sabe qué hace, qué aprueba y a quién informa. |
| 4 · Cuantitativo | Se mide el desempeño individual por rol y se ajusta el RACI con base en datos de carga real y resultados. |
| 5 · Optimizado | Roles adaptativos: la IA sugiere reasignación de tickets según carga, especialidad y disponibilidad real del equipo. |

### 3.12 Disponibilidad y cobertura horaria

> **Por qué es práctica independiente:** el horario de atención no es un detalle operativo — es un compromiso contractual y un diferenciador comercial. Evaluar si la mesa tiene cobertura definida, pactada y medida es fundamental para saber si el SLA es realista o solo declarativo.

| Nivel | Qué implica este nivel |
|---|---|
| 1 · Inicial | Sin horario definido. El equipo responde cuando puede, sin compromiso formal de disponibilidad. |
| 2 · Administrado | Horario informal, conocido por el equipo pero no pactado contractualmente con el cliente. |
| 3 · Definido | Horario definido y pactado con el cliente (ej. L-V 7:30AM–5PM). GAP administrativo negociado (capacitaciones, incapacidades, administrativo). |
| 4 · Cuantitativo | Se mide el cumplimiento real de la cobertura pactada vs. la cobertura entregada, con reporte periódico. |
| 5 · Optimizado | Cobertura adaptativa: la IA gestiona N0 y N1 fuera del horario laboral, habilitando efectivamente un servicio 24×7 sin costo de guardia humana permanente. |

### 3.13 Gestión de integraciones y entorno de aplicaciones

> **Por qué es práctica independiente:** las mesas en operación no atienden aplicaciones aisladas — atienden ecosistemas: Canal Asesor, Sura Masivos, Digital Venta, sistemas de historia clínica, ERPs, etc. No saber cómo están integrados esos sistemas es la causa raíz de muchos incidentes que se resuelven tarde o mal.

| Nivel | Qué implica este nivel |
|---|---|
| 1 · Inicial | Sin documentación de sistemas integrados. El conocimiento de las integraciones es informal y vive en pocas personas. |
| 2 · Administrado | Lista básica de sistemas, sin arquitectura de integración ni dependencias documentadas. |
| 3 · Definido | Mapa de integraciones documentado: sistemas, APIs, dependencias, canales y dueño técnico de cada integración. |
| 4 · Cuantitativo | Se mide el impacto de incidentes por sistema integrado y se prioriza la atención según criticidad de la integración afectada. |
| 5 · Optimizado | Monitoreo predictivo de integraciones: alertas automáticas antes de que fallen canales críticos (ej. caída de API de pagos, timeout de historia clínica). |

---

## 4. Dimensión de éxito de negocio

Más allá de las 13 prácticas operativas, una mesa de servicio debe evaluarse también como **negocio** — no solo como operación. Una mesa puede estar en nivel 4 operativamente y ser poco rentable o estar perdiendo al cliente. Esta dimensión evalúa cuatro indicadores de éxito de negocio:

| Indicador | Qué mide |
|---|---|
| Rentabilidad del contrato | Margen real vs. estimado por FTE asignado. ¿La mesa es negocio rentable para PS? |
| Retención y crecimiento de cuenta | ¿El cliente renueva? ¿Crece la cuenta hacia nuevos servicios o se estanca? |
| NPS / CSAT del cliente final | Promotor neto y recurrencia de quejas formales. ¿El cliente recomendaría el servicio? |
| Eficiencia de costo | Costo por ticket resuelto y % de resolución automatizada. ¿El servicio se vuelve más eficiente con el tiempo? |

> **Una mesa exitosa cumple ambas dimensiones:** madura operativamente (ITIL v5) y rentable / valiosa para PS y el cliente.

---

## 5. Capa sectorial: Banca

Para clientes de banca, el modelo general se complementa con criterios regulatorios y de criticidad propios del sector financiero. Estos criterios no reemplazan las 13 prácticas — se evalúan como una capa adicional de madurez específica.

### 5.1 Por qué banca necesita una capa adicional

El sector bancario en Colombia está bajo la supervisión de la **Superintendencia Financiera de Colombia (SFC)**, que exige niveles de control, trazabilidad y continuidad operativa más estrictos que en otros sectores. Una mesa de servicio que opera aplicaciones bancarias críticas (core bancario, canales digitales, medios de pago) tiene exigencias que van más allá de la operación técnica estándar.

### 5.2 Prácticas adicionales evaluadas en banca

| Práctica sectorial | Qué evalúa |
|---|---|
| Continuidad de negocio (BCP/DRP) | ¿La mesa tiene planes de continuidad probados para sistemas críticos? ¿Se han ejecutado simulacros? |
| Trazabilidad de cambios (control SOX) | ¿Todo cambio en producción tiene aprobación documentada y trazabilidad completa de quién, qué y cuándo? |
| Gestión de incidentes de seguridad | ¿Existe un proceso diferenciado para incidentes que involucran posible fraude o vulnerabilidad de seguridad? |
| Reportabilidad regulatoria | ¿La mesa puede generar evidencia auditable que demuestre cumplimiento ante un requerimiento de la SFC? |
| Segregación de funciones | ¿Quién atiende, quién aprueba y quién despliega están claramente separados, evitando conflicto de interés? |
| Disponibilidad de canales críticos | ¿Se mide y reporta específicamente la disponibilidad de canales transaccionales (banca móvil, cajeros, pagos)? |

### 5.3 Niveles de madurez sectorial en banca

| Nivel | Descripción |
|---|---|
| 1 · Inicial | No hay BCP probado, los cambios se hacen sin trazabilidad formal, no hay separación entre quien desarrolla y quien despliega |
| 2 · Administrado | Existen políticas de continuidad y control de cambios, pero no se ejecutan simulacros ni auditorías internas regulares |
| 3 · Definido | BCP probado anualmente, control de cambios con aprobación formal, segregación de funciones documentada |
| 4 · Cuantitativo | Se mide tiempo de recuperación ante incidentes críticos (RTO/RPO) y se reporta cumplimiento normativo de forma sistemática |
| 5 · Optimizado | Monitoreo predictivo de canales transaccionales, detección automática de patrones de fraude operativo, reportabilidad regulatoria generada automáticamente |

---

## 6. Capa sectorial: Salud (EPS)

Para clientes del sector salud, especialmente EPS e IPS, el modelo se complementa con criterios de protección de datos clínicos y continuidad asistencial.

### 6.1 Por qué salud necesita una capa adicional

El sector salud en Colombia opera bajo supervisión de la **Superintendencia Nacional de Salud (Supersalud)**, y maneja **datos sensibles de salud** protegidos bajo régimen especial de Habeas Data (Ley 1581 de 2012), que exige niveles de protección más estrictos que datos personales comunes.

### 6.2 Prácticas adicionales evaluadas en salud

| Práctica sectorial | Qué evalúa |
|---|---|
| Protección de datos sensibles de salud | ¿El acceso a historia clínica está controlado, registrado y auditado a nivel de cada consulta individual? |
| Continuidad de servicios asistenciales | ¿Existen protocolos diferenciados para incidentes que afectan la atención directa al paciente? |
| Trazabilidad clínica | ¿Todo cambio en el sistema de historia clínica queda registrado con quién, cuándo y por qué, de forma auditable ante Supersalud? |
| Gestión de incidentes con impacto asistencial | ¿Hay clasificación diferenciada entre un incidente administrativo y uno que pone en riesgo la atención de un paciente? |
| Cumplimiento de interoperabilidad | ¿Los sistemas soportados cumplen los estándares exigidos por el Ministerio de Salud (RIPS, PISIS)? |

### 6.3 Niveles de madurez sectorial en salud

| Nivel | Descripción |
|---|---|
| 1 · Inicial | No hay control de acceso diferenciado a historia clínica, los incidentes asistenciales se tratan igual que cualquier ticket |
| 2 · Administrado | Existe alguna restricción de acceso, pero sin auditoría sistemática de quién consultó qué información clínica |
| 3 · Definido | Control de acceso documentado por rol, incidentes con impacto asistencial clasificados y escalados con prioridad diferenciada |
| 4 · Cuantitativo | Se mide tiempo de respuesta para incidentes con impacto en atención al paciente, con metas más estrictas que el resto del catálogo |
| 5 · Optimizado | Monitoreo predictivo de sistemas asistenciales críticos, alertas automáticas ante riesgo de interrupción de servicios de atención |

---

## 7. Aplicación comercial del modelo

### 7.1 Cómo usarlo en una conversación de venta

El modelo permite construir una narrativa simple y poderosa frente al cliente: **"así está hoy su mesa, así podría estar en 6 meses, y esto es lo que cambia en el negocio."**

1. Aplicar el **clasificador inicial**: ¿es Mesa de Ayuda o Mesa de Soporte? Esto define el nivel mínimo esperado
2. Aplicar la evaluación de las **13 prácticas** (instrumento Excel) a la mesa actual del cliente
3. Construir el **perfil de madurez visual** (radar chart) por práctica
4. Identificar el nivel global y compararlo contra el estándar mínimo esperado según el tipo de mesa
5. Presentar el **roadmap de evolución**, mostrando qué cambia en el negocio en cada salto de nivel
6. Conectar cada salto de nivel con **valor concreto**: menos tickets recurrentes, menos riesgo regulatorio, mejor experiencia para el usuario final
7. Si aplica, presentar la **capa sectorial** (banca o salud) como diferenciador adicional

### 7.2 Argumento de valor por sector

**Banca:** "Hoy su mesa opera de forma reactiva, sin trazabilidad completa de cambios. Eso representa un riesgo frente a un requerimiento de la SFC. Con el modelo de Nivel 3 en adelante, cada cambio queda documentado y auditable — reduce su exposición regulatoria, no solo mejora el soporte técnico."

**Salud (EPS):** "Actualmente no hay diferenciación entre un ticket administrativo y uno que afecta la atención de un paciente. Eso significa que un problema de autorización de un procedimiento urgente puede esperar en la misma fila que un reseteo de contraseña. Con un modelo de Nivel 3, esos incidentes se priorizan automáticamente — protege la continuidad asistencial."

### 7.3 Conexión con el modelo de transición de clientes

Este modelo de madurez es el insumo de entrada para la **Fase 4 (Transición de clientes actuales)** del plan general del servicio: antes de proponer la migración de una mesa hacia el modelo de Mesa de Servicios de Nueva Generación, se aplica esta evaluación para tener evidencia objetiva del punto de partida y construir el caso de negocio de la transición.

---

## 8. Próximos pasos

1. **Pilotar el clasificador** en las mesas actuales — definir si cada mesa activa es de Ayuda o de Soporte, y qué nivel mínimo le corresponde
2. **Aplicar el instrumento v2** (Excel con 13 prácticas) en al menos una mesa de banca y una de salud para calibrar la rúbrica con evidencia real
3. **Validar la capa sectorial** con el equipo CTO/SICTO y, si es posible, con un experto regulatorio de cada sector
4. **Construir el material comercial** (slide deck) que traduce el modelo de madurez en argumento de venta con las 13 prácticas y el clasificador
5. **Definir el estándar de mercado esperado** por sector y tipo de mesa — referencia contra la cual comparar a cada cliente
6. **Integrar el modelo con la Fase 4** del plan de diseño del servicio: diagnóstico de madurez como condición de entrada para la propuesta de transición
7. **Explorar la capa sectorial para Centro América** (Curasao, otros) con sus particularidades regulatorias propias
