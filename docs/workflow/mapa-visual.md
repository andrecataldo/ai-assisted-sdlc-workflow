# 🗺️ Mapa Visual — AI-Assisted SDLC Workflow (Governado)

<!-- MAPA VISUAL -->
<!-- DIDÁTICO | NÃO NORMATIVO -->
<!-- EXPLICITA ARTEFATOS, ASSISTENTES E GOVERNANÇA -->

Este mapa visual apresenta a **estrutura completa e governada** do
**AI-Assisted SDLC Workflow**, explicitando:

- artefatos canônicos
- assistentes (agents) como geradores
- contratos e memória como eixo central
- execução como conceito bloqueado

⚠️ Este diagrama **não representa pipeline técnico**
nem autoriza execução automática.

---

## 🧭 Como ler este mapa

- **Centro:** contratos e decisões humanas
- **Esquerda:** artefatos principais do método
- **Direita:** assistentes (agents) que geram artefatos
- **Abaixo:** execução apenas conceitual
- **Acima:** diretriz primária (autoridade máxima)

---

## 🧩 Mapa Conceitual (Artefatos × Assistentes × Governança)

```mermaid
flowchart TB

%% =========================
%% CAMADA 0 — DIRETRIZ
%% =========================
DIRETRIZ["Diretriz Primária<br/>IA acelera, humano responde"]

%% =========================
%% CAMADA 1 — ARTEFATOS (GRAMÁTICA)
%% =========================
subgraph A["Artefatos Canônicos"]
  PRD["PRD-Lite"]
  CP["Context Pack"]
  FI["Feature Intent"]
  TG["Guidelines Técnicos"]
  ARCH["Visão de Arquitetura"]
end

%% =========================
%% CAMADA 2 — ASSISTENTES (AGENTS)
%% =========================
subgraph B["Assistentes do Workflow (Agents)"]
  CG["Context Generator"]
  TGG["Tech Guidelines Generator"]
  AG["Architecture Generator"]
  APG["Action Plan Generator"]
  MCPG["MCP / MCP+ Generator"]
end

%% =========================
%% CAMADA 3 — CONTRATOS & MEMÓRIA (v0.2 — VIGENTE)
%% =========================
subgraph C["Contratos & Memória (v0.2)"]
  MCP["MCP / MCP+"]
  DL["Decision Locks"]
  DOR["Definition of Ready"]
  DOS["Definition of Stop"]
  CK["Checkpoint"]
end

%% =========================
%% CAMADA 4 — EXECUÇÃO CONCEITUAL (v0.3 — ENCERRADA)
%% =========================
subgraph D["Execução Assistida (Conceitual)"]
  NR["No Run"]
  DR["Dry Run"]
  HR["Hot Run (bloqueado)"]
end

%% =========================
%% RELAÇÕES — AUTORIDADE
%% =========================
DIRETRIZ --> A
DIRETRIZ --> C

%% =========================
%% RELAÇÕES — ARTEFATOS
%% =========================
PRD --> CP --> FI
FI --> TG
FI --> ARCH

TG --> MCP
ARCH --> MCP
FI --> MCP

%% =========================
%% RELAÇÕES — ASSISTENTES (GERAÇÃO)
%% =========================
CG -. gera .-> CP
TGG -. gera .-> TG
AG -. gera .-> ARCH
APG -. gera .-> FI
MCPG -. gera .-> MCP

%% =========================
%% RELAÇÕES — CONTRATOS
%% =========================
MCP --> DL
MCP --> DOR
MCP --> DOS
DOS --> CK

%% =========================
%% EXECUÇÃO (REFERÊNCIA, NÃO PIPELINE)
%% =========================
MCP -. referencia .-> NR
NR -. referencia .-> DR
DR -. referencia .-> HR

%% =========================
%% BLOQUEIOS
%% =========================
classDef blocked fill:#ffe6e6,stroke:#cc0000,stroke-width:2px;
class HR blocked
```
```
Diretriz Primária
  |
  +--> Artefatos Canônicos: PRD-Lite -> Context Pack -> Feature Intent
  |                         Feature Intent -> Guidelines / Arquitetura
  |                         (todos alimentam MCP/MCP+)
  |
  +--> Contratos & Memória (v0.2): MCP/MCP+ -> Decision Locks -> DoR/DoS -> Checkpoint
  |
  +--> Assistentes (Agents) geram artefatos:
        - Context Generator ---------> Context Pack
        - Tech Guidelines Generator -> Guidelines
        - Architecture Generator ----> Arquitetura
        - Action Plan Generator -----> Feature Intent (ou Action Plan, se existir)
        - MCP/MCP+ Generator --------> MCP/MCP+

Execução (v0.3): No Run -> Dry Run -> Hot Run (BLOQUEADO)
```

