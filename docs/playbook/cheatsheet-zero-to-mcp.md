# Cheatsheet — Do Zero ao MCP (AI-Assisted SDLC)

Este cheatsheet mostra o **caminho mínimo e correto** para sair de uma ideia
e chegar a um **MCP pronto para execução por IA**, seguindo a gramática do workflow.

---

## Visão Geral (1 Página)

```text
IDEIA / PROBLEMA
      │
      ▼
PRD-Lite
      │
      ▼
Context Pack
      │
      ▼
Guidelines Técnicos
      │
      ▼
Visão de Arquitetura
      │
      ▼
Feature Intent
      │
      ▼
Action Plan
      │
      ▼
MCP
      │
      ▼
Execução por IA + Revisão Humana
```

## Passo a Passo Essencial

### 1️⃣ PRD-Lite

- 📄 **Artefato:** `prd-lite-<produto>-vX.md`
- 🧠 **Responsável:** Humano
- 🤖 **Gerado por:** —

Define **por que o produto existe** e **o que NÃO será feito agora**.

**Checklist**
- ✔ Problema
- ✔ Objetivo
- ✔ Escopo (In / Out)
- ✔ Restrições

---

### 2️⃣ Context Pack

- 📄 **Artefato:** `context-pack-<produto>-vX.md`
- 🤖 **Gerado por:** Context Generator

Consolida o **contexto cognitivo completo** para a IA.

**Checklist**
- ✔ Produto
- ✔ Usuários
- ✔ Linguagem
- ✔ Limites conceituais

---

### 3️⃣ Guidelines Técnicos

- 📄 **Artefato:** `guidelines-<produto>-vX.md`
- 🤖 **Gerado por:** Tech Guidelines Generator

Define **o que pode**, **o que não pode** e **como deve ser feito**.

**Checklist**
- ✔ Dependências permitidas
- ✔ Proibições explícitas
- ✔ Regras técnicas
- ✔ Guardrails da IA

---

### 4️⃣ Visão de Arquitetura

- 📄 **Artefato:** `architecture-<produto>-vX.md`
- 🤖 **Gerado por:** Architecture Generator

Define **estrutura mínima consciente**.

**Checklist**
- ✔ Componentes
- ✔ Responsabilidades
- ✔ Fluxos principais
- ✔ Decisões arquiteturais

---

### 5️⃣ Feature Intent

- 📄 **Artefato:** `feature-intent-<produto>-<id>.md`
- 🧠 **Responsável:** Humano (com apoio de IA)

Define **exatamente o que será feito agora**.

**Checklist**
- ✔ Objetivo da feature
- ✔ Entradas e saídas
- ✔ Casos de sucesso
- ✔ Casos de erro
- ✔ Limites claros

---

### 6️⃣ Action Plan

- 📄 **Artefato:** `action-plan-<feature>.md`
- 🤖 **Gerado por:** Action Plan Generator

Quebra a feature em **passos executáveis**, ainda **humanos-legíveis**.

**Checklist**
- ✔ Etapas numeradas
- ✔ Ordem explícita
- ✔ Dependências entre passos
- ✔ Pontos de verificação

---

### 7️⃣ MCP (Machine-Consumable Plan)

- 📄 **Artefato:** `mcp-<feature>-vX.md`
- 🤖 **Gerado por:** MCP Generator

Contrato **operacional** entre humano e IA.

**Checklist**
- ✔ Ações permitidas
- ✔ Ações proibidas
- ✔ Ordem obrigatória
- ✔ Critérios de parada
- ✔ Condições de erro

---

## Regras de Ouro

- ❌ Nunca pule um artefato
- ❌ Nunca execute IA sem MCP
- ❌ Nunca misture execução com definição
- ✅ Sempre versionar tudo
- ✅ Sempre revisão humana antes de executar

---

## Onde cada coisa vive

```text
ai-assisted-sdlc-workflow/
├── docs/templates/      ← gramática do método
├── docs/agents/         ← geradores
├── docs/context/examples/ ← casos reais
├── docs/playbook/       ← cheatsheets

```

```text
produto/
├── src/                 ← código executável
├── tests/
├── pyproject.toml

```
---

## Por que este cheatsheet é importante

Ele garante que:
- você **não se perca** no método
- novos colaboradores **entendam em 5 minutos**
- a IA **nunca receba contexto incompleto**
- o workflow seja **ensinável e escalável**


---

## Estado do Documento

- **Tipo:** Cheatsheet Visual
- **Workflow:** AI-Assisted SDLC
- **Versão:** v0.1
- **Uso:** Referência rápida “do zero à execução”

