> ⚠️ **STATUS DO DOCUMENTO — REFERÊNCIA CONCEITUAL (ENCERRADO)**
>
> Este documento é um **mapa conceitual da versão v0.3** do AI-Assisted SDLC Workflow.
>
> A v0.3 encontra-se **normativamente encerrada**.
> Este arquivo **não possui autoridade normativa** e **não governa uso, execução ou decisão**.
>
> 👉 A fonte normativa oficial da v0.3 está em:
> - `docs/v0.3/` (capítulos normativos encerrados)
> - `docs/checkpoints/checkpoint-v0.3-normative-closure.md` (encerramento normativo)
>
> 👉 A versão vigente do workflow é a **v0.2**:
> - `docs/README-v0.2.md`
>
> Use este documento **apenas como referência conceitual**, leitura contextual e material de aprendizado.
>
> ---

# 📘 AI-Assisted SDLC Workflow — v0.3 (Mapa Conceitual Encerrado)

> **Status:** Encerrado (referência conceitual)  
> **Versão do workflow:** v0.3  
> **Autoridade normativa:** ❌ Nenhuma  
> **Dependência obrigatória:** v0.2 (Contratos, Consistência e Memória Operacional)  
> **Escopo:** Conceitos de pré-execução assistida  
> **Execução de código:** ❌ Não definida  

---

## 1. Propósito deste Documento

Este documento descreve o **mapa conceitual da v0.3** do AI-Assisted SDLC Workflow.

A v0.3 introduz, em nível **estritamente conceitual**, a noção de **execução assistida por IA**, com foco em:
- governança
- risco
- controle humano
- auditabilidade

Nenhuma regra executável, automação ou integração técnica é definida aqui.

> Este documento **não governa execução**.  
> Ele governa apenas o **desenho do território conceitual** onde a execução poderia existir no futuro.

---

## 2. Relação com a v0.2 (Versão Vigente)

A v0.3 **não substitui** a v0.2.  
Ela **depende integralmente** da v0.2 para existir.

### Fundamentos herdados obrigatoriamente da v0.2

- MCP+ como contrato forte por iteração
- Decision Locks explícitos e versionados
- Precedência normativa entre artefatos
- Checkpoints como unidade de continuidade
- IA sem autoridade decisória

Qualquer iniciativa inspirada na v0.3 que viole esses fundamentos é considerada **inválida**.

---

## 3. Pergunta Central da v0.3

> **Como permitir execução assistida por IA sem perder controle humano, consistência cognitiva e auditabilidade?**

A v0.3 **não existe para acelerar código**.  
Ela existe para **governar o risco introduzido pela execução**.

---

## 4. Princípio Arquitetural Dominante

> **Execução é um efeito colateral de decisões bem governadas — nunca o objetivo primário do workflow.**

Este princípio orienta todo o desenho conceitual da v0.3.

---

## 5. Escopo Conceitual da v0.3

### 5.1 O que a v0.3 explora conceitualmente

- introdução da ideia de execução assistida por IA
- separação explícita entre definição, decisão e execução
- mecanismos conceituais de controle, observabilidade e reversibilidade
- preparação para automação futura **sem comprometer governança**

### 5.2 O que a v0.3 explicitamente NÃO define

- ferramentas de execução
- integração com CI/CD
- execução automática ou end-to-end
- orquestração de múltiplos agentes
- métricas técnicas, thresholds ou SLAs

---

## 6. Camadas Conceituais da v0.3

A v0.3 é estruturada como **camadas dependentes**, nunca como um fluxo linear simples.

---

### 🔹 Camada 0 — Fundação (v0.2)

Base normativa herdada integralmente da v0.2.

Nada nesta camada é alterado, flexibilizado ou renegociado.

---

### 🔹 Camada 1 — Modos de Execução (conceito)

A v0.3 introduz a ideia de **modos**, não de execução padrão.

Modos conceituais:
- **No Run** — definição e decisão apenas (default)
- **Dry Run** — simulação ou geração não aplicada
- **Hot Run** — execução real (excepcional)

Este documento **não define critérios normativos** para uso desses modos.

---

### 🔹 Camada 2 — Guards de Execução (conceito)

Execução só pode existir se **explicitamente permitida**.

Conceitos explorados:
- pré-condições mínimas
- escopo autorizado
- impacto esperado conhecido
- avaliação de reversibilidade

Guards são tratados aqui como **conceitos arquiteturais**, não como checklists operacionais.

---

### 🔹 Camada 3 — Contrato de Qualidade Mínima (conceito)

A v0.3 reconhece que executar algo mal definido é mais perigoso do que não executar.

Surge o conceito de:
- qualidade mínima aceitável para execução
- prontidão para executar (diferente da Definition of Ready)
- tolerância a erro explicitada

Nenhuma métrica, SLA ou threshold é definida.

---

### 🔹 Camada 4 — Observabilidade Cognitiva

A execução só é aceitável se for **observável e explicável** posteriormente.

Observabilidade cognitiva inclui:
- decisões humanas envolvidas
- hipóteses assumidas
- contexto fornecido à IA
- divergência entre esperado e resultado

Não se trata de observabilidade técnica.

---

### 🔹 Camada 5 — Rollback & Recovery Cognitivo

Pergunta fundamental:
> *Se algo der errado, conseguimos voltar ao estado cognitivo anterior?*

Conceitos explorados:
- rollback de execução
- invalidação explícita de decisões
- checkpoints como snapshots cognitivos

A v0.3 estabelece o **direito arquitetural ao rollback**, não o mecanismo.

---

## 7. Limites Explícitos deste Documento

Este documento:

- ❌ não é normativo
- ❌ não autoriza execução
- ❌ não define automação
- ❌ não substitui MCP+, Decision Locks ou Checkpoints
- ❌ não governa ferramentas ou pipelines

Qualquer avanço além deste mapa exige **nova versão e nova autoridade explícita**.

---

## 8. Relação com Uso Real e Evidência

O desenho da v0.3 pressupõe que a v0.2 será:
- aplicada em contextos reais
- observada em uso
- criticada por usuários
- refinada empiricamente

Esses aprendizados **não alteram este documento**  
e só podem alimentar versões futuras mediante checkpoint explícito.

---

## 9. Nota Final

A v0.3 representa uma transição crítica:
- de definição para ação
- de controle cognitivo para risco operacional

Por isso, ela existe como **mapa conceitual encerrado**, não como sistema em evolução.

> **Na v0.3, desenhar bem é mais importante do que executar rápido.**

---

## 🏷️ Identificação

AI-Assisted SDLC Workflow — v0.3  
Mapa Conceitual Encerrado (referência)
