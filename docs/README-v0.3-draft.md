> ⚠️ **STATUS DO DOCUMENTO — LEITURA CONCEITUAL**
> 
> Este documento é um **draft conceitual** da versão v0.3 do AI-Assisted SDLC Workflow.
> 
> Ele **não possui autoridade normativa** e **não governa uso, execução ou decisão**.
> 
> 👉 A fonte normativa oficial da v0.3 está em:
> - `docs/v0.3/` (capítulos normativos)
> - `docs/checkpoints/checkpoint-v0.3-normative-closure.md` (encerramento normativo)
> 
> 👉 A versão vigente do workflow continua sendo a **v0.2**:
> - `docs/README-v0.2.md`
> 
> Use este documento apenas como **mapa conceitual e contextual**.
> 
> ---

# 📘 README — AI-Assisted SDLC Workflow v0.3 (Draft)

> **Status:** Draft (conceitual)  
> **Versão do workflow:** v0.3-draft  
> **Dependência obrigatória:** v0.2 (Contratos, Consistência e Memória Operacional)  
> **Escopo:** Pré-execução controlada  
> **Execução de código:** ❌ Não definida neste draft

---

## 1. Propósito deste Documento

Este documento descreve o **mapa conceitual da versão v0.3** do AI-Assisted SDLC Workflow.

A v0.3 introduz, pela primeira vez, a noção de **execução assistida por IA**, porém **apenas no nível conceitual e arquitetural**.  
Nenhuma regra executável, automação ou integração técnica é definida aqui.

> **Este README não governa execução.**  
> Ele governa o **desenho do território** onde a execução poderá existir futuramente.

---

## 2. Contexto e Continuidade

A v0.3 **não substitui** a v0.2.  
Ela **se apoia integralmente** nos contratos, regras e estruturas definidos na v0.2.

### Heranças obrigatórias da v0.2
- MCP+ como contrato forte por iteração
- Decision Locks explícitos e versionados
- Precedência normativa entre artefatos
- Checkpoints como unidade de continuidade
- IA sem autoridade decisória

Qualquer iniciativa na v0.3 que viole esses princípios é considerada **inválida**.

---

## 3. Pergunta Central da v0.3

> **Como permitir execução assistida por IA sem perder controle humano, consistência cognitiva e auditabilidade?**

A v0.3 não existe para acelerar código.  
Ela existe para **governar o risco introduzido pela execução**.

---

## 4. Princípio Arquitetural Dominante

> **Execução é um efeito colateral de decisões bem governadas — nunca o objetivo primário do workflow.**

Este princípio orienta todas as escolhas conceituais da v0.3.

---

## 5. Escopo da v0.3 (Draft)

### 5.1 O que a v0.3 pretende explorar
- Introdução conceitual de execução assistida por IA
- Fronteiras explícitas entre definição, decisão e execução
- Mecanismos conceituais de controle, observabilidade e reversibilidade
- Preparação para automação futura sem comprometer governança

### 5.2 O que a v0.3 **não decide neste momento**
- Ferramentas de execução
- Integração com CI/CD
- Execução automática ou end-to-end
- Orquestração de múltiplos agentes
- Métricas técnicas, thresholds ou SLAs

---

## 6. Camadas Conceituais da v0.3

A v0.3 é estruturada como **camadas dependentes**, nunca como um fluxo linear simples.

---

### 🔹 Camada 0 — Fundação (v0.2)

Base normativa herdada integralmente da v0.2.

Nada nesta camada é alterado, flexibilizado ou renegociado na v0.3.

---

### 🔹 Camada 1 — Modos de Execução

A v0.3 introduz a ideia de **modos**, não de execução padrão.

Modos conceituais:
- **No Run** — definição e decisão apenas (default)
- **Dry Run** — simulação ou geração não aplicada
- **Hot Run** — execução real (excepcional)

Este draft **não define critérios de permissão** para cada modo.

---

### 🔹 Camada 2 — Guards de Execução

Execução só pode existir se **explicitamente permitida**.

Conceitos de guard:
- pré-condições mínimas
- escopo autorizado
- impacto esperado conhecido
- avaliação de reversibilidade

Neste estágio, guards são **conceitos**, não checklists.

---

### 🔹 Camada 3 — Contrato de Qualidade Mínima

A v0.3 reconhece que executar algo mal definido é mais perigoso do que não executar.

Surge o conceito de:
- qualidade mínima aceitável para execução
- prontidão para executar (diferente da Definition of Ready)
- tolerância a erro explícita

Nenhuma métrica ou threshold é definida neste draft.

---

### 🔹 Camada 4 — Observabilidade Cognitiva

A execução só é aceitável se for **observável e explicável** posteriormente.

Observabilidade cognitiva inclui:
- decisões humanas envolvidas
- hipóteses assumidas
- contexto fornecido à IA
- divergência entre esperado e resultado

Não se trata ainda de observabilidade técnica.

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

## 7. Limites Explícitos deste Draft

Este documento **não é normativo**.

Ele:
- não autoriza execução
- não define regras finais
- não substitui MCP+, Decision Locks ou Checkpoints
- não governa ferramentas ou automações

Qualquer avanço além deste mapa exige **nova versão**.

---

## 8. Relação com Uso Real da v0.2

O desenho da v0.3 pressupõe que a v0.2 será:
- aplicada em contextos reais
- observada em uso
- criticada por usuários
- refinada empiricamente

Esses aprendizados alimentarão versões futuras da v0.3.

---

## 9. Próximos Passos Possíveis (não obrigatórios)

Após este draft, caminhos possíveis incluem:
- definição do índice normativo da v0.3
- criação de guards mínimos experimentais
- estudo de ergonomia da execução assistida
- conexão com um caso real documentado

Nenhum desses passos é automático.

---

## 10. Nota Final

A v0.3 representa uma transição crítica:
- de definição para ação
- de controle cognitivo para risco operacional

Por isso, ela começa como **mapa**, não como sistema fechado.

> **Na v0.3, desenhar bem é mais importante do que executar rápido.**

---

## 🏷️ Identificador de Draft

AI-Assisted SDLC Workflow — v0.3-draft  
Mapa Conceitual de Pré-Execução Controlada
