# Mesa de Servicios de Nueva Generación con IA
**PersonalSoft · Estrategia CTO / SICTO**

---

## 1. Resumen ejecutivo

La Mesa de Servicios de Nueva Generación es un servicio gestionado que permite a clientes del sector banca y seguros operar, escalar y evolucionar continuamente sus aplicaciones mediante capacidades de soporte técnico, gestión de conocimiento e inteligencia artificial, bajo un modelo controlado, medible y alineado a estándares ITIL v4, ISO 27000 e ISO 42000.

A diferencia de un modelo tradicional de staff augmentation, este es un **servicio nuevo**, con propuesta de valor propia, catálogo definido, indicadores de desempeño, herramientas estándar y modelo de gobierno.

**Value proposition:** Útil + Disponibilidad

---

## 2. Problema que resuelve

| Problema | Impacto |
|---|---|
| No hay límites definidos del servicio por niveles y características | Alcance difuso, sin estándar |
| Sin RACI claro entre roles | Confusión de responsabilidades |
| Plan de cuenta sin control de crecimientos | El cliente no quiere pagar más |
| Herramientas no estandarizadas | Dependencia de la herramienta del cliente |
| Medición empírica, sin KPIs reales | Imposible demostrar valor |
| Líderes técnicos sin claridad de función | Gestión ad hoc |

---

## 3. Valor entregado

- Mejora en la calidad del servicio
- Mayor satisfacción del cliente
- Equipos especializados y enfocados
- Datos y registros para reportes y retroalimentación
- Automatización con herramientas propias
- Madurez continua del servicio
- Aumento del tiempo de disponibilidad de los servicios ITIL
- Gestión de conocimiento activa (base de conocimiento nivel 0)
- IA como diferenciador y acelerador — no como reemplazo

---

## 4. Alcance del servicio

### 4.1 Qué incluye

- Recepción, categorización y resolución de solicitudes (niveles 1, 2 y 3)
- Gestión de incidentes, problemas y requerimientos
- Escalamiento adecuado según SLA
- Gestión de conocimiento: base de conocimiento construida con el cliente
- Reportes e indicadores mensuales
- Retroalimentación del cliente
- Gestión de herramienta (propia o del cliente)
- Capacitación, inducción y entrenamiento del equipo
- Gestión de conocimiento sobre integraciones con otros sistemas
- Seguimiento y control con el cliente y al interior del equipo
- Entregable mensual con victorias tempranas cada 15 días

### 4.2 Sabores del servicio

| Sabor | Descripción |
|---|---|
| Equipo dedicado | Asignación 100% a un cliente |
| Soporte compartido | Una misma persona atiende varios clientes pequeños (capacidad compartida) |
| Versión Express (Alfa) | Modalidad inicial para piloto y clientes nuevos |

> **Premisa operativa:** Se opera desde la herramienta del cliente. Si el cliente no tiene herramienta definida, PersonalSoft provee la propia.

### 4.3 Qué NO incluye (por definir)

- Desarrollo de nuevas funcionalidades (va a desarrollo / proyectos)
- Infraestructura física (por definir si aplica nivel 3 infra)
- Soporte 24×7 por defecto (se negocia por cliente)

---

## 5. Niveles del servicio

### Niveles Mesa de Ayuda vs Mesa de Soporte

| Aspecto | Mesa de Ayuda | Mesa de Soporte |
|---|---|---|
| Nivel | Básico (Nivel 1) | Avanzado (Nivel 2 y 3) |
| Tipo de atención | Reactiva | Reactiva y proactiva |
| Complejidad | Baja | Media y alta |
| Perfil | Atención al usuario | Técnico especializado |
| Enfoque | Usuario | Tecnología y servicio |

---

### Nivel 1 · Front-end

**Perfil:** Técnico junior, Analista junior

**Funciones:**
- Recepción de solicitudes (llamadas, chat, correo, tickets)
- Registro y categorización inicial del Caso / Incidente / Requerimiento
- Resolución de problemas sencillos con KEDB (Manuales, Guías)
- Escalamiento a N2 si no se resuelve en tiempo determinado (SLA)

**Tipos de casos:**
- Reseteo de contraseñas y desbloqueo de cuentas
- Configuración básica de aplicativos
- Dudas sobre el uso de software comunes
- Instalación de software estandarizado

**Lenguajes / herramientas:**
- PowerShell (Windows)
- Bash (Linux)
- HTML, CSS
- Python básico

---

### Nivel 2 · Soporte especializado

**Perfil:** Técnico especializado, en campo si es necesario

**Funciones:**
- Investigación y diagnóstico técnico más detallado
- Soporte especializado en campo si es necesario
- Configuración de hardware, redes y sistemas operativos
- Validación de errores de software que podrían ser más graves

**Tipos de casos:**
- Fallas de hardware (cambio de discos, memoria, periféricos)
- Problemas de acceso a la VPN
- Conflicto de drivers o software específico de negocio
- Recuperación de copias de seguridad

**Lenguajes / herramientas:**
- Python avanzado
- SQL (básico)
- JavaScript

---

### Nivel 3 · Back-end

**Perfil:** Desarrollador senior, dominio

**Funciones:**
- Atención de incidentes en PDN que afectan continuidad de negocio
- Desarrollo de parches o correcciones de código
- Configuración de servidores, bases de datos y seguridad perimetral
- Relación directa con proveedores externos

**Tipos de casos:**
- Caídas masivas de servidores o servicios en la nube
- Vulnerabilidad de seguridad o ciberataques
- Errores críticos en el código de una aplicación interna (bugs)
- Optimización de arquitectura de red, BD, integración

**Lenguajes / herramientas:**
- Python, Go, Java, C#
- YAML, JSON, SQL

> **Pendiente de decisión:** ¿Se incluye soporte de infraestructura física (discos, equipos, infra) en el nivel 3 o se deja por fuera del alcance?

---

## 6. Roles y RACI

### 6.1 Roles del servicio

| Rol | Responsabilidad principal |
|---|---|
| Gerente de Mesa de Servicio | Gestión del servicio, relación con el cliente, reportes, indicadores, gobierno |
| Líder Técnico de Equipo | Coordinación técnica, escalamientos, calidad de resolución |
| Analista de Servicios (N1) | Atención primer nivel, categorización, resolución básica |
| Coordinador de Service Desk (N2) | Diagnóstico especializado, soporte en campo |
| Desarrollador / Especialista (N3) | Resolución de alto impacto, parches, correcciones críticas |
| Especialista IA / Datos | Automatización, gestión de conocimiento, AIOps |

> **Pendiente:** Definir RACI detallado — quién hace, quién aprueba, quién es consultado, quién es informado. Especialmente entre Gerente de Mesa y Líder Técnico.

### 6.2 Modelo de asignación

- Equipos dedicados: asignación a 100% por cliente (modelo preferido)
- Soporte compartido: porcentaje de capacidad que atiende varios clientes (Centro América, clientes pequeños)
- Es raro asignar a alguien al 50% o 30% — se pilotea primero

---

## 7. Modelo operativo

### 7.1 Flujo comercial y operativo

```
Solicitud de cliente / Presentar oferta al cliente
        ↓
    Estimación ──── Comercial (preventa) / Operaciones / Financiera
        ↓
      Venta ──── A&S: Búsqueda de personas
        ↓
   Transición ──── Inducción, capacitación funcional y técnica
                   Entrega de documentación, casos (historia)
                   Capacitación sobre integraciones con otros sistemas
                   Gestión de conocimiento
                   Acuerdos con cliente y mesas de otros niveles
        ↓
  Montaje del modelo de operación
        ↓
    Ejecución ──── Operación del servicio
        ↓
Seguimiento y control ──── Solicitud / Recepción / Niveles
```

### 7.2 Criterios para estimar el servicio

Al recibir una solicitud de cliente, se requiere parametrizar:

1. Tipo de mesa: qué nivel(es) requiere
2. Tecnologías / lenguajes / aplicativos
3. ¿Afecta continuidad de negocio? Criticidad
4. Histórico de casos/ticket (últimos 3 meses) — Frecuencia
5. Tiempo promedio de cierre por ticket, esfuerzo real del cierre (HH)
6. ¿Si tiene SLA establecidos? ¿Quién los define y quién los mide?
7. Disponibilidad que se requiere del servicio (24×7 / 5×8)
8. Negociar GAP de labores administrativas (no al 100%)
9. ¿El cliente usará su aplicativo o PS debe adquirir herramienta?

> **Parámetros base para la calculadora:**
> - Matriz de conocimiento
> - Línea base
> - % GAP de tiempo muerto por FTE
> - Horas laborales
> - Monetización por ticket

### 7.3 Conversaciones requeridas por etapa

**Comercial:**
- Validación de requerimientos con el cliente
- Percepción propia y del cliente de las mesas actuales

**Preventa:**
- Crear modelo de estimación con la información que se solicitará al cliente

**Transición:**
- Definir plan de entrenamientos de PS y con el cliente
- Gestión de conocimiento

**Montaje del modelo:**
- Check list de recursos a tener para operar (personas, HW, SW, capacitaciones)

**Ejecución:**
- Levantamiento detalle de RACI y proceso a detalle

---

## 8. Herramientas

### 8.1 Filosofía

PersonalSoft debe tener una **herramienta estándar propia** para gestión de tickets, por si el cliente no tiene una definida. Herramienta del cliente = primera opción. Herramienta PS = respaldo y estándar mínimo.

### 8.2 Componentes de herramienta

| Componente | Propósito |
|---|---|
| Gestión de tickets | Recepción, asignación, seguimiento, cierre |
| Base de conocimiento (nivel 0) | Respuestas a incidentes más comunes del cliente |
| Reportes y dashboards | KPIs, SLA, tendencias |
| Integración con IA | Clasificación automática, sugerencias de solución |
| Portal de autoservicio | El usuario ingresa sus peticiones sin intermediario |

### 8.3 Licencias

> **Pendiente de decisión:** ¿Quién paga las licencias — el cliente o PersonalSoft? Definir en acuerdo comercial por cliente.

---

## 9. Indicadores (KPIs)

| Indicador | Descripción |
|---|---|
| Tiempo de respuesta | Desde que llega el ticket hasta primera atención |
| Tiempo de resolución | Desde apertura hasta cierre del ticket |
| Cumplimiento SLA | % de tickets resueltos dentro del SLA pactado |
| Tickets por nivel | Distribución de carga entre N1, N2, N3 |
| Reducción de tickets recurrentes | Impacto de la base de conocimiento |
| Velocidad de despliegue | Para mesas con componente de desarrollo |
| Nivel de automatización | % de tickets resueltos con apoyo de IA |
| Satisfacción del cliente (CSAT) | Encuesta post-cierre |
| Medición del rendimiento por FTE | Esfuerzo real vs. esfuerzo estimado |

> **Modelo de reporting:** Entregable mensual al cliente. Victorias tempranas cada 15 días.

---

## 10. Acuerdo de niveles de servicio (SLA)

> **Pendiente de estandarización.** Actualmente no hay un estándar definido.

Aspectos a negociar por cliente:
- Horario de atención (¿24×7? ¿5×8? ¿L-V con extensión de guardia?)
- Tiempo de respuesta por prioridad (crítico / alto / medio / bajo)
- Tiempo de resolución por nivel (N1 / N2 / N3)
- Penalidades y compromisos ante incumplimiento
- GAP administrativo del equipo (capacitación, incapacidades, reuniones)

---

## 11. Capacidades de Inteligencia Artificial

La IA es el diferenciador estratégico del servicio. Se incorpora en el ciclo completo de operación.

### 11.1 Principios de IA

- **Human-in-the-loop** como base de operación — la IA asiste, el humano decide
- IA como aumento de capacidades, no reemplazo de personas
- Cumplimiento con ISO 42000
- Trazabilidad de decisiones asistidas por IA
- Gestión de riesgos: seguridad, privacidad y sesgos

### 11.2 Capacidades por módulo

| Módulo | Capacidad IA | Descripción |
|---|---|---|
| Recepción / Intake | Clasificación automática | Categoriza y prioriza tickets sin intervención humana |
| Base de conocimiento (N0) | Sugerencia de solución | La herramienta sugiere la respuesta antes de escalar |
| Evaluación técnica | Análisis de código | Detecta patrones de error y propone diagnóstico |
| Diseño | Recomendaciones de arquitectura | Sugiere caminos de solución basado en histórico |
| Implementación | Desarrollo asistido | Generación y análisis de código para resolución |
| Testing | Generación automática de pruebas | Cobertura de casos de prueba para cambios |
| Operación | Monitoreo predictivo (AIOps) | Detecta anomalías antes de que generen incidente |
| Mejora continua | Optimización automática | Identifica causas raíz recurrentes y propone ajustes |
| Reportes | Generación de informes | Reportes automáticos con insights para el cliente |

### 11.3 Ingeniería asistida por IA

- Generación de código para correcciones
- Análisis estático de código
- Refactorización asistida
- Reducción del tiempo de resolución en N2 y N3

### 11.4 Calidad automatizada

- Testing automático de regresión ante cambios
- Validación continua de integraciones
- Reducción de tickets por errores en despliegue

### 11.5 AIOps — Operación inteligente

- Monitoreo predictivo de aplicaciones y servicios
- Detección temprana de incidentes antes de afectar al usuario
- Correlación de eventos para diagnóstico acelerado

### 11.6 Gobierno y cumplimiento

- Auditoría automatizada de cambios
- Control de riesgos regulatorios (banca / seguros)
- Trazabilidad completa de decisiones asistidas por IA

---

## 12. Gestión del conocimiento

La gestión del conocimiento es un componente estructural del servicio — no un accesorio.

- **Base de conocimiento nivel 0:** respuestas a los incidentes más comunes del cliente, disponibles antes de abrir ticket
- La base se construye **con el cliente** durante la transición y se actualiza continuamente
- Aplica para autoservicio: el usuario consulta antes de llamar
- La IA alimenta y prioriza la base según tickets resueltos
- **Matriz de conocimiento por nivel:** cada nivel tiene su propio repositorio de soluciones y lenguajes
- Conversar si la gestión de conocimiento va como parte de Staffing o como parte de Proyectos (definición pendiente)

---

## 13. Modelo de transición (clientes actuales)

Los clientes actuales que hoy operan bajo un modelo de staff augmentation deben migrar hacia el nuevo modelo de servicio.

### 13.1 Clientes prioritarios

| Cliente | Estado | Acción |
|---|---|---|
| SURA (Tren 2) | Virginia Durango / Lina Vargas | Reunión: que nos muestren 30 min de operación real |
| Bancolombia (CoEs) | Más maduro — ya tienen metodología | Ir a recoger la metodología, aprender de ellos |
| Centro América | Yamis — soporte y mantenimiento | Modelo de soporte compartido, capacidad compartida |
| XM / otras | Maritza, Paula Soto | Buscar y conocer cómo operan |

### 13.2 Modelo de transición

```
Hoy: Staff augmentation (persona dentro del cliente)
        ↓
Transición: Definir qué hay, quién hace qué, qué hay que cambiar
        ↓
Nuevo modelo: Mesa de Servicios con SLA, KPIs, herramienta, IA
```

- Delivery en 4 meses para SURA
- Cuentas ticket SOPORTA: niveles 1, 2, 3. Reducir tickets con causa-raíz
- Palancas: modernizaciones, otros servicios que se cobran aparte
- Discovery de otros servicios dentro del cliente

---

## 14. Enfoque estratégico

- Foco principal: banca y seguros (alta regulación, alto volumen de tickets, madurez)
- Evolución hacia servicios con IA como diferenciador real
- Expansión internacional (Centro América como primer paso)
- Transición de staffing a servicios de alto valor y margen
- Integración de tecnología, negocio y gobierno en un solo modelo
- Portafolio actual: incluir IA como diferenciador y escalabilidad
- Versión Express (Alfa): arrancar el 1 de julio, definir procesos y condiciones
- Capacitación a comerciales para vender el servicio correctamente

---

## Glosario

| Término | Definición |
|---|---|
| KEDB | Knowledge Error Database — base de errores conocidos y sus soluciones |
| RACI | Responsible, Accountable, Consulted, Informed |
| SLA | Service Level Agreement — acuerdo de niveles de servicio |
| FTE | Full Time Equivalent — equivalente a tiempo completo |
| PDN | Producción — ambiente productivo del cliente |
| AIOps | Artificial Intelligence for IT Operations |
| GAP | Diferencia entre capacidad disponible y capacidad efectiva |
| ITIL v4 | Information Technology Infrastructure Library — marco de buenas prácticas |
| N0 | Nivel 0 — autoservicio, sin intervención humana |
| CoE | Center of Excellence — centro de excelencia |
