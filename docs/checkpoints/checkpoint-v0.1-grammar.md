# 🔖 CHECKPOINT — Gramática do AI-Assisted SDLC (v0.1)

<!-- CHECKPOINT OFICIAL -->
Projeto: ai-assisted-sdlc-workflow  
Produto: AI-Assisted SDLC Workflow  
Versão do workflow: v0.1  
Versão do checkpoint: v0.1-grammar-final  
Data: 2025-12-22  
Responsável humano: Andre Cataldo  
Objetivo do checkpoint: Encerrar formalmente a v0.1 (gramática do método) e registrar estado consolidado para retomada fiel em novos chats.

---

## 1. Contexto do Checkpoint

Este checkpoint marca o fechamento da **v0.1**, focada em definir a **gramática do método** e produzir os artefatos canônicos (templates, agentes, playbooks iniciais e exemplos) para demonstrar o uso correto do workflow.

A v0.1 estabelece a separação fundamental:
- **Workflow ≠ Produto**
- O método vive no repositório `ai-assisted-sdlc-workflow`
- Código executável vive em repositórios de produto
- IA executa, humano decide
- **MCP é obrigatório** antes de qualquer execução

---

## 2. Estado Atual Consolidado

### 2.1 O que está concluído

#### 👨‍💻 Repositório
- Local: https://github.com/andrecataldo/ai-assisted-sdlc-workflow

#### 📐 Gramática do Método (v0.1)
Templates canônicos criados e versionados:
- PRD-Lite Template
- Feature Intent Template
- Context Pack Template
- Guidelines Técnicos Template
- Architecture Template
- MCP Template

📁 Local: `docs/templates/`

#### 🤖 Assistentes do Workflow (v0.1)
Especificações criadas para:
- Context Generator
- Tech Guidelines Generator
- Architecture Generator
- Action Plan Generator
- MCP Generator

📁 Local: `docs/agents/`

#### 🧪 Caso Real de Validação
Produto exemplo **Academic Paper Builder** criado como instância da gramática, incluindo:
- PRD-Lite real
- Context Pack real
- Guidelines reais
- Visão de Arquitetura
- Feature Intent (Feature 01)
- Action Plan
- MCP

📁 Local: `docs/context/examples/`  
> Importante: exemplos não definem o método, apenas demonstram o uso correto.

#### 📘 Playbook / Cheatsheets
Criado cheatsheet visual **“Do Zero ao MCP”**, com:
- fluxo completo
- responsabilidades
- artefatos
- regras de ouro

📁 Local: `docs/playbook/`

---

### 2.2 O que NÃO está concluído (fora de escopo v0.1)

- Contratos cognitivos avançados (ex.: Decision Locks, Artifact Precedence, DoR/DoS)
- Memória operacional formal via checkpoints (pasta e estratégia canônicas)
- Preparação para execução quente de código (Hot Run)

Esses itens foram deixados para evolução do método em versões seguintes.

---

### 2.3 Decisões vigentes (nível de versão)

- A v0.1 define a gramática, não a execução
- Exemplos são demonstrativos e não normativos
- MCP é obrigatório antes de qualquer execução

---

## 3. Artefatos Válidos neste Momento

Os seguintes artefatos governam a v0.1:

- Templates: `docs/templates/`
- Agentes: `docs/agents/`
- Exemplos: `docs/context/examples/`
- Playbooks/Cheatsheets: `docs/playbook/`
- Workflow operacional: `docs/workflow/README-workflow-ia.md`

---

## 4. Próximo Passo Recomendado

Após este checkpoint, os caminhos previstos eram:

- Evoluir para **v0.2** (contratos, consistência e memória operacional)  
**ou**
- Aplicar o método a um novo produto do zero (mantendo v0.1 como base)

---

## 5. Regras de Retomada

Ao retomar a partir deste checkpoint:

- Este documento deve ser lido primeiro
- Os templates em `docs/templates/` são referência canônica
- Os exemplos em `docs/context/examples/` não definem o método
- MCP é obrigatório antes de execução

---

## 🏷️ TAG DE RETOMADA

RETOMADA:  
Checkpoint fechado — Gramática do AI-Assisted SDLC v0.1 concluída (v0.1-grammar)
