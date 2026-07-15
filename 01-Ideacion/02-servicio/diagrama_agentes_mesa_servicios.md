# Arquitectura agéntica · Mesa de Servicios de Nueva Generación
**PersonalSoft · Red de agentes de IA**

---

## Diagrama de agentes

<svg width="100%" viewBox="0 0 680 620" xmlns="http://www.w3.org/2000/svg">
<defs>
<marker id="arr" viewBox="0 0 10 10" refX="8" refY="5" markerWidth="6" markerHeight="6" orient="auto-start-reverse">
<path d="M2 1L8 5L2 9" fill="none" stroke="context-stroke" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</marker>
</defs>
<text x="340" y="20" text-anchor="middle" font-size="13" font-weight="500" fill="#2C2C2A" font-family="sans-serif">Arquitectura agéntica · Mesa de Servicios</text>
<text x="340" y="36" text-anchor="middle" font-size="11" fill="#888780" font-family="sans-serif">PersonalSoft · Red de agentes de IA</text>
<rect x="230" y="50" width="220" height="40" rx="8" fill="#E6F1FB" stroke="#85B7EB" stroke-width="0.5"/>
<text x="340" y="66" text-anchor="middle" font-size="11" font-weight="500" fill="#0C447C" font-family="sans-serif">Ticket / Solicitud entrante</text>
<text x="340" y="82" text-anchor="middle" font-size="10" fill="#185FA5" font-family="sans-serif">Portal · Chat · Correo · API</text>
<line x1="340" y1="90" x2="340" y2="118" stroke="#B4B2A9" stroke-width="1" marker-end="url(#arr)"/>
<rect x="190" y="118" width="300" height="64" rx="10" fill="#26215C" stroke="#7F77DD" stroke-width="1"/>
<text x="340" y="142" text-anchor="middle" font-size="13" font-weight="500" fill="#CECBF6" font-family="sans-serif">Agente orquestador</text>
<text x="340" y="158" text-anchor="middle" font-size="10" fill="#AFA9EC" font-family="sans-serif">Clasificación · Enrutamiento · Coordinación · Human-in-the-loop</text>
<text x="340" y="172" text-anchor="middle" font-size="10" fill="#AFA9EC" font-family="sans-serif">Memoria de contexto · Historial del ticket</text>
<line x1="240" y1="182" x2="108" y2="248" stroke="#7F77DD" stroke-width="0.8" marker-end="url(#arr)"/>
<line x1="280" y1="182" x2="218" y2="248" stroke="#7F77DD" stroke-width="0.8" marker-end="url(#arr)"/>
<line x1="340" y1="182" x2="340" y2="248" stroke="#7F77DD" stroke-width="0.8" marker-end="url(#arr)"/>
<line x1="400" y1="182" x2="462" y2="248" stroke="#7F77DD" stroke-width="0.8" marker-end="url(#arr)"/>
<line x1="440" y1="182" x2="572" y2="248" stroke="#7F77DD" stroke-width="0.8" marker-end="url(#arr)"/>
<rect x="44" y="248" width="118" height="100" rx="8" fill="#FAEEDA" stroke="#EF9F27" stroke-width="0.5"/>
<text x="103" y="268" text-anchor="middle" font-size="11" font-weight="500" fill="#633806" font-family="sans-serif">Agente triaje</text>
<line x1="52" y1="274" x2="154" y2="274" stroke="#FAC775" stroke-width="0.5"/>
<text x="103" y="288" text-anchor="middle" font-size="9" fill="#854F0B" font-family="sans-serif">Priorización</text>
<text x="103" y="301" text-anchor="middle" font-size="9" fill="#854F0B" font-family="sans-serif">Categorización</text>
<text x="103" y="314" text-anchor="middle" font-size="9" fill="#854F0B" font-family="sans-serif">SLA automático</text>
<text x="103" y="327" text-anchor="middle" font-size="9" fill="#854F0B" font-family="sans-serif">N1 / N2 / N3</text>
<text x="103" y="340" text-anchor="middle" font-size="9" fill="#854F0B" font-family="sans-serif">Base N0</text>
<rect x="174" y="248" width="118" height="100" rx="8" fill="#FAEEDA" stroke="#EF9F27" stroke-width="0.5"/>
<text x="233" y="268" text-anchor="middle" font-size="11" font-weight="500" fill="#633806" font-family="sans-serif">Agente diagnóstico</text>
<line x1="182" y1="274" x2="284" y2="274" stroke="#FAC775" stroke-width="0.5"/>
<text x="233" y="288" text-anchor="middle" font-size="9" fill="#854F0B" font-family="sans-serif">Análisis de código</text>
<text x="233" y="301" text-anchor="middle" font-size="9" fill="#854F0B" font-family="sans-serif">Causa raíz</text>
<text x="233" y="314" text-anchor="middle" font-size="9" fill="#854F0B" font-family="sans-serif">Deuda técnica</text>
<text x="233" y="327" text-anchor="middle" font-size="9" fill="#854F0B" font-family="sans-serif">Impacto estimado</text>
<text x="233" y="340" text-anchor="middle" font-size="9" fill="#854F0B" font-family="sans-serif">Logs · trazas</text>
<rect x="304" y="248" width="118" height="100" rx="8" fill="#FAEEDA" stroke="#EF9F27" stroke-width="0.5"/>
<text x="363" y="268" text-anchor="middle" font-size="11" font-weight="500" fill="#633806" font-family="sans-serif">Agente desarrollo</text>
<line x1="312" y1="274" x2="414" y2="274" stroke="#FAC775" stroke-width="0.5"/>
<text x="363" y="288" text-anchor="middle" font-size="9" fill="#854F0B" font-family="sans-serif">Generación código</text>
<text x="363" y="301" text-anchor="middle" font-size="9" fill="#854F0B" font-family="sans-serif">Refactorización</text>
<text x="363" y="314" text-anchor="middle" font-size="9" fill="#854F0B" font-family="sans-serif">Hotfix asistido</text>
<text x="363" y="327" text-anchor="middle" font-size="9" fill="#854F0B" font-family="sans-serif">PR automático</text>
<text x="363" y="340" text-anchor="middle" font-size="9" fill="#854F0B" font-family="sans-serif">Revisión de código</text>
<rect x="434" y="248" width="118" height="100" rx="8" fill="#FAEEDA" stroke="#EF9F27" stroke-width="0.5"/>
<text x="493" y="268" text-anchor="middle" font-size="11" font-weight="500" fill="#633806" font-family="sans-serif">Agente testing</text>
<line x1="442" y1="274" x2="544" y2="274" stroke="#FAC775" stroke-width="0.5"/>
<text x="493" y="288" text-anchor="middle" font-size="9" fill="#854F0B" font-family="sans-serif">Pruebas automáticas</text>
<text x="493" y="301" text-anchor="middle" font-size="9" fill="#854F0B" font-family="sans-serif">Regresión</text>
<text x="493" y="314" text-anchor="middle" font-size="9" fill="#854F0B" font-family="sans-serif">Validación continua</text>
<text x="493" y="327" text-anchor="middle" font-size="9" fill="#854F0B" font-family="sans-serif">Cobertura de casos</text>
<text x="493" y="340" text-anchor="middle" font-size="9" fill="#854F0B" font-family="sans-serif">Reporte de calidad</text>
<rect x="564" y="248" width="108" height="100" rx="8" fill="#FAEEDA" stroke="#EF9F27" stroke-width="0.5"/>
<text x="618" y="265" text-anchor="middle" font-size="11" font-weight="500" fill="#633806" font-family="sans-serif">Agente AIOps</text>
<text x="618" y="278" text-anchor="middle" font-size="10" font-weight="500" fill="#633806" font-family="sans-serif">+ Conocimiento</text>
<line x1="572" y1="284" x2="664" y2="284" stroke="#FAC775" stroke-width="0.5"/>
<text x="618" y="298" text-anchor="middle" font-size="9" fill="#854F0B" font-family="sans-serif">Monitoreo predictivo</text>
<text x="618" y="311" text-anchor="middle" font-size="9" fill="#854F0B" font-family="sans-serif">Detección temprana</text>
<text x="618" y="324" text-anchor="middle" font-size="9" fill="#854F0B" font-family="sans-serif">KEDB · Base N0</text>
<text x="618" y="337" text-anchor="middle" font-size="9" fill="#854F0B" font-family="sans-serif">Wiki automática</text>
<line x1="103" y1="348" x2="240" y2="390" stroke="#EF9F27" stroke-width="0.6" stroke-dasharray="4 2" marker-end="url(#arr)"/>
<line x1="233" y1="348" x2="290" y2="390" stroke="#EF9F27" stroke-width="0.6" stroke-dasharray="4 2" marker-end="url(#arr)"/>
<line x1="363" y1="348" x2="340" y2="390" stroke="#EF9F27" stroke-width="0.6" stroke-dasharray="4 2" marker-end="url(#arr)"/>
<line x1="493" y1="348" x2="390" y2="390" stroke="#EF9F27" stroke-width="0.6" stroke-dasharray="4 2" marker-end="url(#arr)"/>
<line x1="618" y1="348" x2="440" y2="390" stroke="#EF9F27" stroke-width="0.6" stroke-dasharray="4 2" marker-end="url(#arr)"/>
<rect x="190" y="390" width="300" height="56" rx="8" fill="#E1F5EE" stroke="#1D9E75" stroke-width="0.5"/>
<text x="340" y="412" text-anchor="middle" font-size="12" font-weight="500" fill="#085041" font-family="sans-serif">Resolución coordinada</text>
<text x="340" y="428" text-anchor="middle" font-size="10" fill="#0F6E56" font-family="sans-serif">Cierre automático · Escalamiento humano · Derivación a modernización</text>
<text x="340" y="442" text-anchor="middle" font-size="10" fill="#0F6E56" font-family="sans-serif">Registro en base de conocimiento · Actualización SLA</text>
<line x1="340" y1="446" x2="340" y2="470" stroke="#B4B2A9" stroke-width="1" marker-end="url(#arr)"/>
<rect x="100" y="470" width="480" height="44" rx="8" fill="#EEEDFE" stroke="#AFA9EC" stroke-width="0.5"/>
<text x="340" y="490" text-anchor="middle" font-size="11" font-weight="500" fill="#3C3489" font-family="sans-serif">Gobierno de IA · Human-in-the-loop · ISO 42000 · Trazabilidad · Auditoría</text>
<text x="340" y="506" text-anchor="middle" font-size="10" fill="#534AB7" font-family="sans-serif">Toda decisión agéntica es supervisada, trazada y auditable</text>
<line x1="340" y1="514" x2="340" y2="538" stroke="#B4B2A9" stroke-width="1" marker-end="url(#arr)"/>
<rect x="150" y="538" width="380" height="44" rx="8" fill="#1D9E75" stroke="#0F6E56" stroke-width="0.5"/>
<text x="340" y="558" text-anchor="middle" font-size="12" font-weight="500" fill="#E1F5EE" font-family="sans-serif">Valor al negocio</text>
<text x="340" y="574" text-anchor="middle" font-size="10" fill="#9FE1CB" font-family="sans-serif">Disponibilidad · Velocidad · Calidad · Cumplimiento · Evolución continua</text>
<line x1="44" y1="606" x2="74" y2="606" stroke="#7F77DD" stroke-width="1" marker-end="url(#arr)"/>
<text x="80" y="610" font-size="10" fill="#888780" font-family="sans-serif">Orquestador → agente</text>
<line x1="230" y1="606" x2="260" y2="606" stroke="#EF9F27" stroke-width="1" stroke-dasharray="4 2" marker-end="url(#arr)"/>
<text x="266" y="610" font-size="10" fill="#888780" font-family="sans-serif">Agente → retorno resultado</text>
</svg>