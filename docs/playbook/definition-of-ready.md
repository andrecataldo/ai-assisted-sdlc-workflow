# 📘 Definition of Ready (DoR) — Playbook (v0.2)

## 1. O que é Definition of Ready

**Definition of Ready (DoR)** define os critérios mínimos para que um artefato,
fase ou iteração seja considerada **pronta para avançar** no workflow.

> 📌 DoR evita avançar com ambiguidade, lacunas ou decisões implícitas.

Sem DoR explícito, o workflow tende a:
- avançar cedo demais
- gerar retrabalho
- criar loops de refinamento com IA

---

## 2. Princípio central

> **Se não está Ready, não avança — mesmo que a IA “consiga continuar”.**

A capacidade da IA de improvisar **não é critério de prontidão**.

---

## 3. Definition of Ready por Artefato

### 3.1 PRD-Lite — Ready quando:
- problema está descrito em uma frase clara
- objetivo é observável (não genérico)
- escopo IN e OUT estão explícitos
- restrições conhecidas estão listadas
- não há contradições internas

---

### 3.2 Context Pack — Ready quando:
- público-alvo está definido
- linguagem e tom estão claros
- limites conceituais existem
- não contradiz o PRD-Lite
- exemplos são coerentes com o escopo

---

### 3.3 Feature Intent — Ready quando:
- a feature tem propósito claro
- existe justificativa de valor
- dependências são conhecidas
- não viola escopo do PRD/MCP+
- não introduz decisões ocultas

---

### 3.4 Guidelines Técnicos — Ready quando:
- tecnologias permitidas e proibidas estão listadas
- restrições técnicas são explícitas
- não contradizem decisões arquiteturais
- nível de detalhe é proporcional à fase

---

### 3.5 MCP+ — Ready quando:
- objetivo da iteração está claro
- escopo IN/OUT está congelado
- Decision Locks estão definidos
- critérios de sucesso existem
- critérios de parada existem
- artefatos referenciados estão atualizados

📌 **Se o MCP+ não está Ready, nenhuma interação com IA deve continuar.**

---

## 4. DoR como gate do workflow

- DoR é um **gate explícito**
- avançar sem DoR é **violação do método**
- DoR vale tanto para humano quanto para IA

---

## 5. Anti-padrões comuns

- ❌ “Está bom o suficiente”
- ❌ “Depois a gente ajusta”
- ❌ Avançar porque a IA já começou a responder
- ❌ Confundir velocidade com prontidão

---

## 6. Regra final

> **Pronto para avançar ≠ possível de continuar**
