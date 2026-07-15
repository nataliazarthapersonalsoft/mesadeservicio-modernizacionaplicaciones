# Verificación del PPTX — Benchmarking Mesa de Servicio
**Fecha:** 14 de julio de 2026 | **Método:** apertura directa de URLs + búsqueda web cruzada

---

## Resumen ejecutivo

Se verificaron **24 datos/estadísticas** presentes en el PPTX de Benchmarking. Resultado:

| Estado | Cantidad | Descripción |
|--------|----------|-------------|
| ✅ Confirmados exactamente | 13 | Dato correcto, fuente correcta, URL abre |
| 🟡 Correctos con ajuste | 8 | Dato válido pero fuente mal atribuida o etiqueta imprecisa |
| ❌ No confirmados | 3 | Sin fuente pública verificable |

Se identificaron **10 correcciones concretas** para el PPTX.

---

## Detalle por dato

### GRUPO 1 — Benchmarks métricas ITSM

| # | Dato en el PPTX | Estado | Hallazgo | URL verificada |
|---|-----------------|--------|----------|----------------|
| 1 | FCR industria = **74%** | ✅ | Confirmado por [HDI/MetricNet](https://www.thinkhdi.com/~/media/HDICorp/Files/Library-Archive/Insider%20Articles/First%20Contact%20Resolution.pdf). SQM (fuente citada) da 71% — corregir fuente | [HDI FCR PDF](https://www.thinkhdi.com/~/media/HDICorp/Files/Library-Archive/Insider%20Articles/First%20Contact%20Resolution.pdf) |
| 2 | MTTR industria = **8.85 horas** | ✅ | Exacto: "8.85 business hours" en base de datos global MetricNet/HDI | [HDI MTTR PDF](https://www.thinkhdi.com/~/media/HDICorp/Files/Library-Archive/Insider%20Articles/mean-time-to-resolve.pdf) |
| 3 | CSAT industria = **73–86%** | ✅ | Confirmado: HDI reporta 73.1% (2022-23) y 86.3% (2021-22) | [HDI SupportWorld](https://www.thinkhdi.com/library/supportworld/2023/metrics-matter-for-it-support/) |
| 4 | Costo/ticket: N0=$2, N1=$22–35, N2=$69, N3=$104 | ✅ | Exacto en Giva (N0/N2/N3) y Kwestra (N1 rango) | [Giva Shift-Left](https://www.givainc.com/blog/shift-left-analysis-how-to-guide-maximize-it-service-management-itsm-efficiency/) · [Kwestra](https://kwestra.com/insights/itsm-automation-roi/) |
| 5 | Deflection: 23% / 50% / 80–90% | 🟡 | 23% y 80–90% confirmados por Kwestra. "50% maduro" no aparece exacto (Kwestra da líder 40–80%) | [Kwestra](https://kwestra.com/insights/itsm-automation-roi/) |
| 6 | GenAI en MTTR = **−26.6%** | 🟡 | ⚠️ El −26.55% en Freshservice es mejora en **tiempo de respuesta**, NO en MTTR. El −26.63% es de automatización de flujos, no GenAI | [Freshservice Benchmark 2024](https://freshservice.com/assets/resources/freshservice/freshservice-it-service-management-benchmark-report-2024.pdf) |
| 7 | GenAI en resolución = **+34.6%** | 🟡 | ⚠️ El 34.58% es correcto pero la fuente es **Freshservice**, no Contentstack (que da 30.5%) | [Freshservice Benchmark 2024](https://freshservice.com/assets/resources/freshservice/freshservice-it-service-management-benchmark-report-2024.pdf) |
| 8 | KCS+IA en FCR = **+5–7 pts** | 🟡 | Número confirmado, pero la fuente lo atribuye a "IA + knowledge base" según BCG, no específicamente "KCS" | [SDI ITSM Statistics 2024](https://www.servicedeskinstitute.com/resources/itsm-statistics-facts-and-trends-for-2024/) |
| 9 | IA en CSAT = **+15–22 pts** (<5 min espera) | ✅ | Confirmado exactamente. Fuente primaria: HDI 2025 citado por Stealth Agents | [Stealth Agents](https://stealthagents.com/research/ai-it-helpdesk-automation-statistics-2026) |

---

### GRUPO 2 — Mercado y adopción

| # | Dato en el PPTX | Estado | Hallazgo | URL verificada |
|---|-----------------|--------|----------|----------------|
| 10 | ServiceNow = **44.4%** cuota ITSM | 🟡 | Dato correcto (2024) pero fuente es **Apps Run The World**, no IDC. Es cuota "entre los top 10", no del mercado total | [Apps Run The World](https://www.appsruntheworld.com/top-10-it-service-management-software-vendors-and-market-forecast/) |
| 11 | Atlassian 12.3% / BMC 8.5% / Ivanti 6.2% / Freshworks 5.8% | ❌ | No confirmados en fuente pública. Están detrás de suscripción paga. El ranking cualitativo es plausible | Sin URL pública disponible |
| 12 | **68%** adoptará XLA en 2026 | 🟡 | La fuente (XLA Institute) dice **"casi 70%"**, no 68% exacto | [XLA Institute — State of XLA 2025](https://www.einpresswire.com/article/823090394/xla-institute-releases-groundbreaking-state-of-xla-2025-report?code=9Hv3x5D-vwZo-peK) |
| 13 | ITIL v5 lanzado **12 feb 2026** | ✅ | Confirmado por dos fuentes independientes. Nombre oficial: "ITIL (Version 5)" | [Tideline Insights](https://www.tidelineinsights.com/blog/itil-5-whats-coming.html) · [Rixmind](https://rixmind.com/itil-5-what-changed-and-why-it-matters/) |
| 14 | **51%** con IA desplegada / **11%** producción plena / **>40%** cancelados 2027 | ✅ | Confirmados los tres datos. Fuente primaria del >40%: Gartner (jun 2025) | [Brilo AI](https://www.brilo.ai/resources/agentic-ai-statistics) |
| 15 | ITSM Colombia = **USD 108.5M** (2026), CAGR **14.08%** hasta 2031 | ✅ | Confirmado exactamente: $95.8M (2025) → $108.5M (2026) → $209.7M (2031) | [Mordor Intelligence — Colombia ITSM](https://www.mordorintelligence.com/industry-reports/colombia-information-technology-service-management-itsm-market) |

---

### GRUPO 3 — Casos de éxito y datos Colombia

| # | Dato en el PPTX | Estado | Hallazgo | URL verificada |
|---|-----------------|--------|----------|----------------|
| 16 | Robinhood+ServiceNow: 70% deflección, 2.200+ h/mes, 94% satisfacción | ✅ | Dato correcto. ⚠️ **No está en la URL de Brilo AI citada** — fuente real es ServiceNow/Jay Hammonds | [SaaS Intelligence](https://saasintelligence.substack.com/p/servicenow-just-made-ai-free-and) |
| 17 | Honeywell+Moveworks: **~80%** reducción tickets | 🟡 | Orden de magnitud confirmado (~80–85%). ⚠️ No está en Brilo AI — fuente real: Moveworks/Honeywell | [Moveworks AI Help Desk](https://www.moveworks.com/us/en/solutions/ai-help-desk) |
| 18 | Salesforce+Agentforce: **84%** de 380K interacciones resueltas | ✅ | Dato correcto. ⚠️ **No está en Brilo AI** — fuente real: Salesforce FY2025 Q4 | [Cloud Science Labs](https://www.cloudsciencelabs.com/blog/agentforce-roi-how-to-measure-the-business-impact-of-salesforce-ai-agents) |
| 19 | **81%** establecimientos crédito Colombia usan IA | ✅ | Confirmado exactamente por la Superintendencia Financiera de Colombia (2025) | [Superfinanciera](https://www.superfinanciera.gov.co/publicaciones/10116043/sistema-financiero-acelera-implementacion-de-canales-digitales/) |
| 20 | Service Desk & Incident Mgmt Colombia = **27.09%** | ✅ | Confirmado por Mordor Intelligence (2025) | [Mordor Colombia ITSM](https://www.mordorintelligence.com/industry-reports/colombia-information-technology-service-management-itsm-market) |
| 21 | CAGR IT Services Colombia = **9.8%** (más rápido Sudamérica) | ✅ | Confirmado: Colombia es el país de mayor crecimiento en IT Services en Sudamérica según Mordor | [Mordor South America IT Services](https://www.mordorintelligence.com/industry-reports/south-america-it-services-market) |
| 22 | Servicios ITSM Colombia **13.8% CAGR** vs soluciones **61.4%** | 🟡 | ⚠️ El 61.4% **NO es un CAGR** — es la **cuota de mercado** de soluciones en 2025. El 13.82% sí es CAGR de servicios | [Mordor Colombia ITSM](https://www.mordorintelligence.com/industry-reports/colombia-information-technology-service-management-itsm-market) |
| 23 | **30%** contratos TI enterprise serán outcome-based hacia **2029** (TCS) | ❌ | TCS solo dice que habrá migración gradual a outcome-based, sin porcentaje ni año 2029. Dato no sustentado | Sin URL que confirme |
| 24 | Payback **4–9 meses**; **19%** proyectos nunca alcanza ROI | 🟡 | Payback 4–8/9 meses confirmado. El "19% sin ROI" no tiene fuente localizable | [Kwestra](https://kwestra.com/insights/itsm-automation-roi/) (solo payback) |

---

## 10 correcciones recomendadas al PPTX

| # | Slide | Corrección |
|---|-------|------------|
| 1 | Slide 16 | Cambiar fuente de FCR 74%: de SQM → **HDI/MetricNet** |
| 2 | Slides 12/16 | Reetiquetar −26.6%: no es "reducción de MTTR por GenAI" — es "mejora en tiempo de *respuesta* por GenAI" (Freshservice) |
| 3 | Slides 12/16 | Cambiar fuente del +34.6%: de Contentstack → **Freshservice Benchmark 2024** |
| 4 | Slide 10 | Cambiar fuente de cuotas ITSM: de IDC → **Apps Run The World (2024)**; aclarar "entre top 10 proveedores" |
| 5 | Slide 10 | Los shares de Atlassian/BMC/Ivanti/Freshworks no son verificables públicamente; marcar como **"estimación"** o conseguir reporte pago |
| 6 | Slide 17 | Cambiar "68% adoptará XLA" → **"casi 70% planea adoptar XLA"** (XLA Institute) |
| 7 | Slide 18 | Para casos Robinhood/Honeywell/Salesforce: cambiar fuente de Brilo AI (incorrecta) → fuentes reales: ServiceNow, Moveworks, Salesforce |
| 8 | Slide 13 | Aclarar que **61.4% es cuota de mercado** de soluciones ITSM en Colombia (no un CAGR) |
| 9 | Slide 12/18 | El dato "30% contratos outcome-based hacia 2029 (TCS)": **eliminar o cambiar a Gartner** (">30% SaaS enterprise para 2025") |
| 10 | Slide 18 | El "19% proyectos nunca alcanza ROI": **eliminar o buscar fuente** — no localizable en ninguna fuente pública |

---

## URLs verificadas (para agregar al PPTX)

Las siguientes URLs estaban ausentes en el PPTX y ahora están confirmadas:

| Dato | URL confirmada |
|------|----------------|
| Service Desk Colombia 27.09% | https://www.mordorintelligence.com/industry-reports/colombia-information-technology-service-management-itsm-market |
| CAGR IT Services Colombia 9.8% | https://www.mordorintelligence.com/industry-reports/south-america-it-services-market |
| Robinhood+ServiceNow (fuente real) | https://saasintelligence.substack.com/p/servicenow-just-made-ai-free-and |
| Salesforce Agentforce 84% | https://www.cloudsciencelabs.com/blog/agentforce-roi-how-to-measure-the-business-impact-of-salesforce-ai-agents |
| Honeywell+Moveworks | https://www.moveworks.com/us/en/solutions/ai-help-desk |
| ServiceNow 44.4% (fuente correcta) | https://www.appsruntheworld.com/top-10-it-service-management-software-vendors-and-market-forecast/ |
| ITIL v5 12 feb 2026 | https://rixmind.com/itil-5-what-changed-and-why-it-matters/ |
