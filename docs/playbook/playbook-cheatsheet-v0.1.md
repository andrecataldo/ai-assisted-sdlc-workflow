# 📘 Playbook & Cheatsheet  
## Workflow de Desenvolvimento com IA (v0.1)

Este playbook descreve **como usar o Workflow de Desenvolvimento com IA na prática**, com foco em **clareza, governança e repetibilidade**.

Ele deve ser lido como um **manual operacional** do SDLC com IA — tanto para humanos quanto para agentes.

---

## 1️⃣ Princípios Fundamentais (não negociáveis)

- IA é **executora**, não dona do produto
- Humano é **responsável final**
- Todo avanço relevante gera **artefato versionado**
- Nenhuma execução ocorre sem **intenção explícita**
- O processo é **agnóstico de ferramenta**

> Se um desses princípios for violado, o workflow está sendo usado incorretamente.

---

## 2️⃣ Papéis no Workflow

### 🧠 Human Lead Engineer
Responsável por:
- Definir intenção
- Aprovar artefatos
- Validar planos
- Revisar execução
- Assumir riscos técnicos

### 🤖 AI Dev Agent
Responsável por:
- Gerar documentos
- Propor planos
- Implementar código
- Executar tarefas sob regras explícitas

---

## 3️⃣ Artefatos Principais (ordem recomendada)

| Ordem | Artefato | Objetivo |
|-----|---------|----------|
| 1 | PRD-Lite / Documento de Contexto | Entender o **porquê** do produto |
| 2 | Context Pack | Traduzir contexto para IA |
| 3 | Feature Intent | Definir claramente **o que** será feito |
| 4 | Guidelines Técnicos | Definir **como** pode ser feito |
| 5 | Action Plan | Planejar execução passo a passo |
| 6 | Código / Execução | Implementação |
| 7 | Revisão / QA | Garantia de qualidade |

---

## 📐 Tipos de Artefatos no Workflow (Distinção Fundamental)

No **AI-Assisted SDLC Workflow**, existem **três categorias distintas de artefatos**.  
Confundir essas categorias gera ambiguidade conceitual e acoplamento indevido entre processo e produto.

---

### 1. Artefatos do Processo (Meta-nível)

São artefatos que **definem e governam o método** de desenvolvimento com IA.

**Características:**
- Descrevem *como* criar produtos
- São reutilizáveis entre diferentes produtos
- Não dependem de um domínio específico
- Não fazem parte de nenhum produto final

**Exemplos:**
- Roadmap do Workflow
- Playbook / Cheatsheet
- Templates (PRD-Lite, Feature Intent)
- Specs de agentes (`context-generator-v0.1.md`, `action-plan-generator-v0.1.md`)
- Regras, guardrails e convenções

📍 **Localização:**  
`ai-assisted-sdlc-workflow`

---

### 2. Artefatos de Demonstração do Processo (Case Studies)

São artefatos que **demonstram o workflow em funcionamento**, usando um produto real ou fictício como exemplo.

Eles existem para:
- validar o método
- ilustrar o uso correto dos agentes
- servir como referência didática
- provar que o processo é operável

**Características:**
- São gerados *antes* da implementação do produto
- São consumidos por agentes do workflow
- Não são necessários para rodar o produto
- Não fazem parte do runtime ou da entrega ao usuário final

**Exemplos:**
- PRD-Lite preenchido de um produto real
- Context Pack gerado a partir desse PRD
- Feature Intent real
- Action Plan real (pré-execução)

📍 **Localização:**  
`ai-assisted-sdlc-workflow/docs/context/examples/`  
*(ou `case-studies/`, se adotado futuramente)*

---

### 3. Artefatos do Produto

São artefatos que **implementam, executam e entregam valor ao usuário final**.

**Características:**
- Executáveis ou distribuíveis
- Dependem de decisões técnicas
- Fazem parte do ciclo de vida do produto
- São versionados com foco em releases e versionamento semântico

**Exemplos:**
- Código-fonte
- Testes automatizados
- README do produto
- CLI, API ou UI
- Scripts de build e deploy

📍 **Localização:**  
Repositório específico do produto  
(ex.: `academic-paper-builder`)

---

### 🔑 Regra de Ouro (Versão Refinada)

> **Tudo que define, governa ou demonstra o workflow  
> vive no repositório do workflow — mesmo quando usa um produto real como exemplo.**
>
> **Tudo que executa, entrega valor ou é distribuído ao usuário  
> vive no repositório do produto.**

---

### ⚠️ Anti-padrões a Evitar

- Copiar artefatos de demonstração para o repositório do produto
- Misturar documentação do processo com README do produto
- Tratar Context Pack ou Feature Intent como documentação do usuário final

Esses anti-padrões causam **acoplamento conceitual indevido** e dificultam a evolução do método.


---

## 4️⃣ Assistentes do Workflow

### 🔹 Context Generator
- **Input:** PRD-Lite
- **Output:** Context Pack
- **Função:** alinhar IA ao domínio, negócio e problema

---

### 🔹 Tech Guidelines Generator
- **Input:** Context Pack + decisões humanas
- **Output:** Guidelines Técnicos
- **Função:** limitar soluções técnicas possíveis

---

### 🔹 Action Plan Generator
- **Input:** Feature Intent + Guidelines
- **Output:** Plano de execução numerado
- **Função:** reduzir improviso e risco

---

### 🔹 Architecture Generator
- **Input:** Feature Intent + Guidelines
- **Output:** Visão de Arquitetura
- **Função:** antecipar decisões estruturais

---

### 🔹 MCP Generator
- **Input:** Todos os artefatos
- **Output:** Manifesto de Controle do Processo
- **Função:** governança e rastreabilidade (v1+)

---

## 5️⃣ Ferramentas como Capabilities (não como etapas)

O workflow **não depende de ferramentas específicas**.

| Capability | Exemplos |
|----------|---------|
| Planejamento | ChatGPT |
| Execução multi-arquivo | Codex, Cursor |
| Execução via terminal | Codex, Claude Code |
| Revisão | IDE + Humano |
| Qualidade / CI | Pytest, Ruff, MyPy |

> Trocar ferramenta **não muda o processo**.

---

## 6️⃣ Regras práticas para diagramas Mermaid

### ✅ Sempre fazer
- Usar **aspas em subgraphs**
- Usar labels simples
- Testar no GitHub antes de considerar “pronto”

### ❌ Evitar
- Parênteses em títulos de subgraph
- Uso de `&` em labels
- Misturar Markdown e Mermaid em editores externos

---

## 7️⃣ Regras de Versionamento

- Cada artefato relevante → **commit próprio**
- Mudanças estruturais → **tag**
- Nunca versionar:
  - `.venv`
  - `__pycache__`
  - `.pytest_cache`
  - `*.egg-info`

---

## 8️⃣ Checkpoints humanos obrigatórios

Pare e revise quando:
- Um novo artefato for criado
- Um plano for gerado
- Um agente executar código
- Algo “funcionou” rápido demais

---

## 9️⃣ Anti-padrões comuns (alerta)

- Pular direto para código
- “Deixar a IA decidir”
- Não versionar decisões
- Misturar workflow e produto
- Continuar executando sem intenção clara

---

## 🔑 Regra de ouro

> **Se você não consegue explicar o que a IA está fazendo,  
> é porque o workflow falhou.**

---

## Estado do Documento

- **Versão:** v0.1  
- **Status:** Estável  
- **Próxima evolução:**
  - exemplos reais por artefato
  - checklist por assistente
