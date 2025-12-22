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
