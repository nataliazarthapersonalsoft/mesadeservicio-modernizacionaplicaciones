# Mesa de Servicios de Nueva Generación con IA
**PersonalSoft · Estrategia CTO / SICTO**

---

## Arquitectura del servicio

<svg width="100%" viewBox="0 0 780 760" xmlns="http://www.w3.org/2000/svg" role="img">
<title>Mesa de Servicios de Nueva Generación con IA — PersonalSoft</title>
<desc>Arquitectura por capas con modernización continua como servicio externo</desc>
<defs>
<marker id="arrow" viewBox="0 0 10 10" refX="8" refY="5" markerWidth="6" markerHeight="6" orient="auto-start-reverse">
<path d="M2 1L8 5L2 9" fill="none" stroke="context-stroke" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</marker>
<marker id="arrow-coral" viewBox="0 0 10 10" refX="8" refY="5" markerWidth="6" markerHeight="6" orient="auto-start-reverse">
<path d="M2 1L8 5L2 9" fill="none" stroke="#D85A30" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</marker>
</defs>
<text x="370" y="22" text-anchor="middle" font-size="13" font-weight="500" fill="#2C2C2A" font-family="sans-serif">Mesa de Servicios de Nueva Generación</text>
<text x="370" y="38" text-anchor="middle" font-size="11" fill="#888780" font-family="sans-serif">PersonalSoft · Arquitectura de servicio</text>
<text x="40" y="66" font-size="10" font-weight="500" fill="#888780" font-family="sans-serif" letter-spacing="1">CANAL DE ENTRADA</text>
<rect x="40" y="72" width="600" height="44" rx="8" fill="#E6F1FB" stroke="#85B7EB" stroke-width="0.5"/>
<text x="180" y="98" text-anchor="middle" font-size="12" font-weight="500" fill="#0C447C" font-family="sans-serif">Portal de autoservicio</text>
<text x="340" y="98" text-anchor="middle" font-size="12" font-weight="500" fill="#0C447C" font-family="sans-serif">Correo · Chat · Teléfono</text>
<text x="510" y="98" text-anchor="middle" font-size="12" font-weight="500" fill="#0C447C" font-family="sans-serif">API / Integraciones</text>
<line x1="270" y1="80" x2="270" y2="108" stroke="#85B7EB" stroke-width="0.5"/>
<line x1="420" y1="80" x2="420" y2="108" stroke="#85B7EB" stroke-width="0.5"/>
<line x1="340" y1="116" x2="340" y2="134" stroke="#B4B2A9" stroke-width="1" marker-end="url(#arrow)"/>
<text x="40" y="152" font-size="10" font-weight="500" fill="#888780" font-family="sans-serif" letter-spacing="1">NIVELES DE SERVICIO</text>
<rect x="40" y="158" width="130" height="64" rx="8" fill="#E1F5EE" stroke="#5DCAA5" stroke-width="0.5"/>
<text x="105" y="178" text-anchor="middle" font-size="11" font-weight="500" fill="#085041" font-family="sans-serif">N0 · Autoservicio</text>
<text x="105" y="194" text-anchor="middle" font-size="10" fill="#0F6E56" font-family="sans-serif">Base de conocimiento</text>
<text x="105" y="208" text-anchor="middle" font-size="10" fill="#0F6E56" font-family="sans-serif">IA generativa</text>
<rect x="185" y="158" width="130" height="64" rx="8" fill="#E1F5EE" stroke="#1D9E75" stroke-width="0.5"/>
<text x="250" y="178" text-anchor="middle" font-size="11" font-weight="500" fill="#085041" font-family="sans-serif">N1 · Front-End</text>
<text x="250" y="194" text-anchor="middle" font-size="10" fill="#0F6E56" font-family="sans-serif">Recepción · Triaje</text>
<text x="250" y="208" text-anchor="middle" font-size="10" fill="#0F6E56" font-family="sans-serif">Resolución básica</text>
<rect x="330" y="158" width="130" height="64" rx="8" fill="#EEEDFE" stroke="#AFA9EC" stroke-width="0.5"/>
<text x="395" y="178" text-anchor="middle" font-size="11" font-weight="500" fill="#3C3489" font-family="sans-serif">N2 · Especializado</text>
<text x="395" y="194" text-anchor="middle" font-size="10" fill="#534AB7" font-family="sans-serif">Diagnóstico técnico</text>
<text x="395" y="208" text-anchor="middle" font-size="10" fill="#534AB7" font-family="sans-serif">Redes · HW · SW</text>
<rect x="475" y="158" width="165" height="64" rx="8" fill="#26215C" stroke="#534AB7" stroke-width="0.5"/>
<text x="557" y="178" text-anchor="middle" font-size="11" font-weight="500" fill="#CECBF6" font-family="sans-serif">N3 · Back-End</text>
<text x="557" y="194" text-anchor="middle" font-size="10" fill="#AFA9EC" font-family="sans-serif">Incidentes críticos · PDN</text>
<text x="557" y="208" text-anchor="middle" font-size="10" fill="#AFA9EC" font-family="sans-serif">Parches · Arquitectura</text>
<line x1="170" y1="190" x2="183" y2="190" stroke="#1D9E75" stroke-width="0.8" marker-end="url(#arrow)"/>
<line x1="315" y1="190" x2="328" y2="190" stroke="#7F77DD" stroke-width="0.8" marker-end="url(#arrow)"/>
<line x1="460" y1="190" x2="473" y2="190" stroke="#534AB7" stroke-width="0.8" marker-end="url(#arrow)"/>
<line x1="640" y1="190" x2="666" y2="190" stroke="#D85A30" stroke-width="1" stroke-dasharray="5 3" marker-end="url(#arrow-coral)"/>
<rect x="666" y="148" width="104" height="200" rx="8" fill="#FAECE7" stroke="#F0997B" stroke-width="0.5" stroke-dasharray="5 3"/>
<text x="718" y="170" text-anchor="middle" font-size="10" font-weight="500" fill="#712B13" font-family="sans-serif">Servicio externo</text>
<text x="718" y="184" text-anchor="middle" font-size="10" font-weight="500" fill="#993C1D" font-family="sans-serif">Modernización</text>
<text x="718" y="198" text-anchor="middle" font-size="10" font-weight="500" fill="#993C1D" font-family="sans-serif">Continua</text>
<line x1="680" y1="206" x2="758" y2="206" stroke="#F0997B" stroke-width="0.5"/>
<text x="718" y="222" text-anchor="middle" font-size="9" fill="#712B13" font-family="sans-serif">Evaluación AS-IS</text>
<text x="718" y="236" text-anchor="middle" font-size="9" fill="#712B13" font-family="sans-serif">Arquitectura TO-BE</text>
<text x="718" y="250" text-anchor="middle" font-size="9" fill="#712B13" font-family="sans-serif">Roadmap evolutivo</text>
<text x="718" y="264" text-anchor="middle" font-size="9" fill="#712B13" font-family="sans-serif">Migración cloud</text>
<text x="718" y="278" text-anchor="middle" font-size="9" fill="#712B13" font-family="sans-serif">Refactorización</text>
<text x="718" y="292" text-anchor="middle" font-size="9" fill="#712B13" font-family="sans-serif">Nuevas capacidades</text>
<line x1="680" y1="302" x2="758" y2="302" stroke="#F0997B" stroke-width="0.5"/>
<text x="718" y="316" text-anchor="middle" font-size="9" font-weight="500" fill="#993C1D" font-family="sans-serif">Costos y alcance</text>
<text x="718" y="330" text-anchor="middle" font-size="9" fill="#712B13" font-family="sans-serif">independientes</text>
<text x="653" y="183" text-anchor="middle" font-size="8" fill="#D85A30" font-family="sans-serif" transform="rotate(-90 653 183)">se activa si aplica</text>
<line x1="340" y1="222" x2="340" y2="250" stroke="#B4B2A9" stroke-width="1" marker-end="url(#arrow)"/>
<text x="40" y="268" font-size="10" font-weight="500" fill="#888780" font-family="sans-serif" letter-spacing="1">MOTOR DE INTELIGENCIA ARTIFICIAL</text>
<rect x="40" y="274" width="600" height="100" rx="8" fill="#FAEEDA" stroke="#EF9F27" stroke-width="0.5"/>
<rect x="56" y="288" width="128" height="72" rx="6" fill="#FFF8EE" stroke="#FAC775" stroke-width="0.5"/>
<text x="120" y="308" text-anchor="middle" font-size="11" font-weight="500" fill="#633806" font-family="sans-serif">Ingeniería IA</text>
<text x="120" y="324" text-anchor="middle" font-size="10" fill="#854F0B" font-family="sans-serif">Generación de código</text>
<text x="120" y="338" text-anchor="middle" font-size="10" fill="#854F0B" font-family="sans-serif">Análisis · Refactorización</text>
<text x="120" y="352" text-anchor="middle" font-size="10" fill="#854F0B" font-family="sans-serif">Asistencia en N2 y N3</text>
<rect x="200" y="288" width="128" height="72" rx="6" fill="#FFF8EE" stroke="#FAC775" stroke-width="0.5"/>
<text x="264" y="308" text-anchor="middle" font-size="11" font-weight="500" fill="#633806" font-family="sans-serif">Testing IA</text>
<text x="264" y="324" text-anchor="middle" font-size="10" fill="#854F0B" font-family="sans-serif">Pruebas automáticas</text>
<text x="264" y="338" text-anchor="middle" font-size="10" fill="#854F0B" font-family="sans-serif">Validación continua</text>
<text x="264" y="352" text-anchor="middle" font-size="10" fill="#854F0B" font-family="sans-serif">Regresión ante cambios</text>
<rect x="344" y="288" width="128" height="72" rx="6" fill="#FFF8EE" stroke="#FAC775" stroke-width="0.5"/>
<text x="408" y="308" text-anchor="middle" font-size="11" font-weight="500" fill="#633806" font-family="sans-serif">AIOps</text>
<text x="408" y="324" text-anchor="middle" font-size="10" fill="#854F0B" font-family="sans-serif">Monitoreo predictivo</text>
<text x="408" y="338" text-anchor="middle" font-size="10" fill="#854F0B" font-family="sans-serif">Detección temprana</text>
<text x="408" y="352" text-anchor="middle" font-size="10" fill="#854F0B" font-family="sans-serif">Correlación de eventos</text>
<rect x="488" y="288" width="136" height="72" rx="6" fill="#FFF8EE" stroke="#FAC775" stroke-width="0.5"/>
<text x="556" y="308" text-anchor="middle" font-size="11" font-weight="500" fill="#633806" font-family="sans-serif">Cumplimiento IA</text>
<text x="556" y="324" text-anchor="middle" font-size="10" fill="#854F0B" font-family="sans-serif">Auditoría automatizada</text>
<text x="556" y="338" text-anchor="middle" font-size="10" fill="#854F0B" font-family="sans-serif">Trazabilidad · Riesgos</text>
<text x="556" y="352" text-anchor="middle" font-size="10" fill="#854F0B" font-family="sans-serif">ISO 42000</text>
<line x1="340" y1="374" x2="340" y2="402" stroke="#B4B2A9" stroke-width="1" marker-end="url(#arrow)"/>
<text x="40" y="420" font-size="10" font-weight="500" fill="#888780" font-family="sans-serif" letter-spacing="1">PLATAFORMA DE OPERACIÓN</text>
<rect x="40" y="426" width="600" height="56" rx="8" fill="#F1EFE8" stroke="#B4B2A9" stroke-width="0.5"/>
<text x="175" y="450" text-anchor="middle" font-size="11" font-weight="500" fill="#2C2C2A" font-family="sans-serif">Gestión de conocimiento</text>
<text x="175" y="466" text-anchor="middle" font-size="10" fill="#5F5E5A" font-family="sans-serif">KEDB · Base N0 · Wiki</text>
<line x1="310" y1="434" x2="310" y2="474" stroke="#D3D1C7" stroke-width="0.5"/>
<text x="390" y="450" text-anchor="middle" font-size="11" font-weight="500" fill="#2C2C2A" font-family="sans-serif">Herramienta de tickets</text>
<text x="390" y="466" text-anchor="middle" font-size="10" fill="#5F5E5A" font-family="sans-serif">Cliente o estándar PS</text>
<line x1="470" y1="434" x2="470" y2="474" stroke="#D3D1C7" stroke-width="0.5"/>
<text x="555" y="450" text-anchor="middle" font-size="11" font-weight="500" fill="#2C2C2A" font-family="sans-serif">SLA · KPIs · Reportes</text>
<text x="555" y="466" text-anchor="middle" font-size="10" fill="#5F5E5A" font-family="sans-serif">Entregable mensual</text>
<line x1="340" y1="482" x2="340" y2="510" stroke="#B4B2A9" stroke-width="1" marker-end="url(#arrow)"/>
<text x="40" y="528" font-size="10" font-weight="500" fill="#888780" font-family="sans-serif" letter-spacing="1">GOBIERNO DE IA · HUMAN-IN-THE-LOOP</text>
<rect x="40" y="534" width="600" height="44" rx="8" fill="#EEEDFE" stroke="#AFA9EC" stroke-width="0.5"/>
<text x="200" y="558" text-anchor="middle" font-size="11" font-weight="500" fill="#3C3489" font-family="sans-serif">ISO 42000 · Trazabilidad</text>
<line x1="320" y1="542" x2="320" y2="570" stroke="#AFA9EC" stroke-width="0.5"/>
<text x="430" y="550" text-anchor="middle" font-size="11" font-weight="500" fill="#3C3489" font-family="sans-serif">Gestión de riesgos</text>
<text x="430" y="566" text-anchor="middle" font-size="10" fill="#534AB7" font-family="sans-serif">Seguridad · Privacidad · Sesgos</text>
<line x1="540" y1="542" x2="540" y2="570" stroke="#AFA9EC" stroke-width="0.5"/>
<text x="590" y="558" text-anchor="middle" font-size="11" font-weight="500" fill="#3C3489" font-family="sans-serif">ITIL v4</text>
<line x1="340" y1="578" x2="340" y2="606" stroke="#B4B2A9" stroke-width="1" marker-end="url(#arrow)"/>
<rect x="40" y="606" width="600" height="52" rx="8" fill="#1D9E75" stroke="#0F6E56" stroke-width="0.5"/>
<text x="340" y="628" text-anchor="middle" font-size="13" font-weight="500" fill="#E1F5EE" font-family="sans-serif">Valor al negocio</text>
<text x="155" y="648" text-anchor="middle" font-size="10" fill="#9FE1CB" font-family="sans-serif">Disponibilidad</text>
<text x="275" y="648" text-anchor="middle" font-size="10" fill="#9FE1CB" font-family="sans-serif">Eficiencia operativa</text>
<text x="400" y="648" text-anchor="middle" font-size="10" fill="#9FE1CB" font-family="sans-serif">Cumplimiento</text>
<text x="535" y="648" text-anchor="middle" font-size="10" fill="#9FE1CB" font-family="sans-serif">Evolución continua</text>
<rect x="648" y="426" width="24" height="204" rx="4" fill="#F1EFE8" stroke="#B4B2A9" stroke-width="0.5"/>
<text x="660" y="528" text-anchor="middle" font-size="9" fill="#5F5E5A" font-family="sans-serif" transform="rotate(-90 660 528)">Comercial · Financiera · A&S · CTO / Infraestructura</text>
<line x1="40" y1="690" x2="70" y2="690" stroke="#B4B2A9" stroke-width="1" marker-end="url(#arrow)"/>
<text x="76" y="694" font-size="10" fill="#888780" font-family="sans-serif">Flujo del servicio</text>
<line x1="180" y1="690" x2="210" y2="690" stroke="#D85A30" stroke-width="1" stroke-dasharray="5 3" marker-end="url(#arrow-coral)"/>
<text x="216" y="694" font-size="10" fill="#888780" font-family="sans-serif">Derivación a servicio externo</text>
<rect x="400" y="683" width="12" height="12" rx="2" fill="#FAECE7" stroke="#F0997B" stroke-width="0.5" stroke-dasharray="3 2"/>
<text x="418" y="694" font-size="10" fill="#888780" font-family="sans-serif">Servicio externo / costo independiente</text>
</svg>