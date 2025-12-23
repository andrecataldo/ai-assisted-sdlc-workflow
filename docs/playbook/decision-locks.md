# 📘 Decision Locks — Playbook (v0.2)

## 1. O que é um Decision Lock

**Decision Lock** é um mecanismo explícito para **congelar decisões humanas relevantes** durante uma iteração do workflow, impedindo que:

- a IA reabra discussões já resolvidas
- o escopo seja renegociado implicitamente
- decisões “escorram” entre artefatos

> 📌 Um Decision Lock não é uma opinião.  
> É um **compromisso operacional temporário**.

---

## 2. Quando um Decision Lock é obrigatório

Um Decision Lock **deve** ser criado quando a decisão:

- afeta escopo, arquitetura ou direção do produto
- reduz graus de liberdade futuros
- tem alto custo de reversão
- foi debatida e conscientemente encerrada

### Exemplos comuns
- escolha de arquitetura (monolito vs serviço)
- decisão de não incluir uma feature
- escolha de stack ou abordagem técnica
- definição clara de público-alvo
- decisão de não executar código nesta fase

---

## 3. Onde o Decision Lock vive

Decision Locks **sempre vivem dentro do MCP+**, na seção:

> **4. Decisões Bloqueadas (Decision Locks)**

Eles **não** vivem:
- em prompts soltos
- em mensagens de chat
- apenas “na cabeça” do humano

---

## 4. Estrutura mínima de um Decision Lock

Cada Decision Lock deve conter:

| Campo | Obrigatório | Descrição |
|------|-------------|-----------|
| ID | ✅ | Identificador único (DL-01, DL-02…) |
| Decisão | ✅ | O que foi decidido |
| Justificativa | ✅ | Por que essa decisão foi tomada |
| Data | ✅ | Quando foi bloqueada |

📌 Justificativa curta, objetiva, factual.

---

## 5. Regras de imutabilidade

Durante a validade do MCP+:

- ❌ A IA **não pode** questionar Decision Locks
- ❌ A IA **não pode** sugerir alternativas
- ❌ A IA **não pode** reinterpretar a decisão

✔ A IA **pode**:
- trabalhar dentro da decisão
- otimizar soluções respeitando o lock
- apontar impactos **sem sugerir mudança**

---

## 6. Como alterar um Decision Lock (regra de ouro)

Decision Locks **nunca são editados**.

Para alterar uma decisão bloqueada:

1. Encerrar a iteração atual  
2. Criar novo checkpoint  
3. Criar **nova versão do MCP+**  
4. Registrar novo Decision Lock (DL-novo)  
5. Explicitar a mudança de contexto

📌 Alterar decisão = **alterar versão**, não texto.

---

## 7. Decision Lock vs Suposição Aceita

| Aspecto | Decision Lock | Suposição Aceita |
|--------|---------------|------------------|
| Pode ser questionado | ❌ | ✔ |
| Pode ser invalidado | ❌ (na iteração) | ✔ |
| Impacto | Estrutural | Operacional |
| Vive no MCP+ | ✔ | ✔ |

📌 Confundir os dois é uma fonte clássica de loop.

---

## 8. Anti-padrões comuns (o que NÃO fazer)

- ❌ “Vamos ver depois” como Decision Lock  
- ❌ Lock sem justificativa  
- ❌ Alterar lock no meio da iteração  
- ❌ Criar Decision Lock para coisas triviais  
- ❌ Usar Decision Lock como desculpa para não pensar  

---

## 9. Checklist rápido (antes de criar um lock)

Antes de bloquear, pergunte:
- essa decisão reduz ambiguidade real?
- o custo de reversão é alto?
- ela afeta outras decisões?
- estamos confortáveis em conviver com ela nesta iteração?

Se a resposta for “não” → **não crie o lock**.

---

## 10. Relação com o Workflow v0.2

Decision Locks:
- ancoram o MCP+
- estabilizam a iteração
- reduzem rework
- preparam execução futura

Sem Decision Locks, o workflow **degenera em prompt engineering**.

---

## 11. Regra final

> **Decisão discutida ≠ decisão bloqueada**  
> **Decisão bloqueada ≠ decisão eterna**
