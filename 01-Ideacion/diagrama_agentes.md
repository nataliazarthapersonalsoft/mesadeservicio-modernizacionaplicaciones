```mermaid
flowchart TB

subgraph Cliente
A[Banca y Seguros]
end

subgraph Frontstage
B[Mesa de Servicios]
end

subgraph Core
C1[Intake]
C2[Evaluación]
C3[Diseño]
C4[Implementación]
C5[Testing]
C6[Operación]
C7[Evolución]
end

subgraph IA["Capa de Aceleración con IA"]
D1[Agente de Intake<br/>Clasificación automática]
D2[Agente de Análisis<br/>Código / Deuda técnica]
D3[Agente de Arquitectura<br/>Recomendaciones]
D4[Agente de Desarrollo<br/>Generación de código]
D5[Agente de Testing<br/>Pruebas automáticas]
D6[Agente AIOps<br/>Monitoreo predictivo]
D7[Agente de Optimización<br/>Mejora continua]
end

subgraph Gobierno
E[Human-in-the-loop<br/>Control / Riesgos / Trazabilidad]
end

subgraph Valor
G[Aceleración del servicio<br/>Menos tiempo / Mayor calidad / Cumplimiento]
end

A --> B
B --> C1
C1 --> C2 --> C3 --> C4 --> C5 --> C6 --> C7

%% IA conectada a cada etapa
D1 --> C1
D2 --> C2
D3 --> C3
D4 --> C4
D5 --> C5
D6 --> C6
D7 --> C7

%% Gobierno sobre IA
D1 --> E
D2 --> E
D3 --> E
D4 --> E
D5 --> E
D6 --> E
D7 --> E

%% Resultado
C7 --> G
E --> G