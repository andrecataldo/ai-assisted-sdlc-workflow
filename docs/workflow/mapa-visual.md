# Mapa Visual — Workflow de Desenvolvimento com IA (v0.1)

```mermaid
flowchart TB

  subgraph A[Artefatos Principais]
    PRD[PRD-Lite]
    CP[Context Pack]
    FI[Feature Intent]
    TG[Guidelines Técnicos]
    ARCH[Visão de Arquitetura]
    SPECS[Prompts & Specs dos Assistentes]
    PB[Playbook & Cheatsheet]
  end

  subgraph B[Assistentes do Workflow]
    CG[Context Generator]
    TGG[Tech Guidelines Generator]
    APG[Action Plan Generator]
    AG[Architecture Generator]
    MCP[MCP Generator]
  end

  subgraph C[Execução (Capacidades)]
    PLAN[Planejamento]
    EXEC[Execução]
    REVIEW[Revisão Humana]
    QA[Qualidade/CI]
  end

  PRD --> CG --> CP
  PRD --> TGG --> TG
  CP --> FI
  TG --> FI
  FI --> APG
  FI --> AG --> ARCH
  APG --> PLAN --> EXEC --> REVIEW --> QA

  SPECS --- CG
  SPECS --- TGG
  SPECS --- APG
  SPECS --- AG
  SPECS --- MCP

  PB --> REVIEW
  PB --> QA
