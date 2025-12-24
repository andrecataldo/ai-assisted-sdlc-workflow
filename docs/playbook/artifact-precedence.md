# 📘 Artifact Precedence — Playbook (v0.2)

## 1. O problema que este playbook resolve

Em workflows assistidos por IA, é comum existir **mais de um artefato válido** descrevendo o mesmo produto.

Quando esses artefatos:
- divergem
- usam linguagem diferente
- evoluem em ritmos distintos

a IA tende a:
- escolher o documento mais conveniente
- misturar instruções incompatíveis
- reinterpretar decisões humanas

> 📌 **Artifact Precedence define quem manda quando há conflito.**

---

## 2. Princípio central

> **Quando dois artefatos entram em conflito, vence o artefato de maior precedência — não o mais recente, nem o mais detalhado.**

Essa regra é **normativa** e não pode ser ignorada pela IA.

---

## 3. Matriz oficial de precedência (v0.2)

Ordem **decrescente** de autoridade:

1. **MCP+ — Machine-Consumable Plan Plus**
2. **PRD-Lite**
3. **Feature Intent**
4. **Context Pack**
5. **Guidelines Técnicos**
6. **Arquitetura (quando existir)**
7. **Exemplos / Casos reais**

📌 Um artefato **nunca pode invalidar** um artefato acima dele.

---

## 4. Responsabilidade por resolução de conflito

Quando um conflito é detectado:

### 4.1 A IA deve
- identificar explicitamente o conflito
- apontar quais artefatos divergem
- obedecer ao artefato de maior precedência
- **não tentar conciliar automaticamente**

### 4.2 O humano deve
- decidir se o conflito é aceitável
- atualizar os artefatos inferiores
- ou versionar o MCP+ se a decisão mudar

---

## 5. Exemplos práticos

### Exemplo 1 — PRD vs Context Pack
- PRD-Lite define público como “pesquisadores”
- Context Pack sugere “estudantes”

➡️ **Vale o PRD-Lite.**

---

### Exemplo 2 — MCP+ vs Feature Intent
- Feature Intent sugere Feature X
- MCP+ declara Feature X fora do escopo

➡️ **Vale o MCP+.**

---

### Exemplo 3 — Guidelines Técnicos vs Arquitetura
- Guidelines sugerem REST
- Arquitetura define event-driven

➡️ **Vale a Arquitetura.**

---

## 6. Regras de ouro (anti-drift)

- ❌ IA não pode escolher o artefato “mais completo”
- ❌ IA não pode misturar instruções conflitantes
- ❌ IA não pode reinterpretar precedência
- ✔ IA deve sempre declarar qual artefato está seguindo

---

## 7. Atualização de artefatos inferiores

Quando um artefato superior muda:

- artefatos inferiores **devem ser revisados**
- inconsistências **devem ser corrigidas**
- exemplos **devem ser atualizados ou descartados**

📌 Exemplo nunca corrige regra.

---

## 8. Relação com Decision Locks

- Decision Locks **vivem no MCP+**
- Nenhum artefato abaixo pode:
  - reabrir uma decisão bloqueada
  - sugerir alternativa incompatível

📌 Precedência + Decision Locks = estabilidade cognitiva.

---

## 9. Checklist rápido (uso prático)

Antes de avançar uma fase, verifique:
- há divergências entre artefatos?
- a precedência está clara?
- a IA sabe qual documento obedecer?
- alguma decisão bloqueada foi violada?

Se houver dúvida → **parar e resolver antes de continuar**.

---

## 10. Regra final (memorável)

> **Documento não decide — precedência decide.**
