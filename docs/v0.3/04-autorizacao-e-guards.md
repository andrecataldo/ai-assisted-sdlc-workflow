# 4️⃣ Autorização e Guards de Execução

> **Status:** Normativo  
> **Versão do workflow:** v0.3  
> **Dependência:**  
> - Capítulo 2 — Princípios Normativos da Execução Assistida  
> - Capítulo 3 — Modos de Execução  
> **Autoridade:** Define as condições mínimas sob as quais a execução pode ser considerada

---

## 4.1 Propósito deste Capítulo

Este capítulo estabelece as **regras normativas de autorização e proteção** (guards) para qualquer forma de execução assistida por IA.

Seu objetivo é:
- impedir execução por inércia, entusiasmo ou pressão
- garantir que toda execução seja **consciente, delimitada e rastreável**
- separar claramente **capacidade técnica** de **permissão normativa**

Nenhuma capacidade técnica de executar implica autorização para executar.

---

## 4.2 Princípio da Execução Bloqueada por Padrão

No AI-Assisted SDLC Workflow, a execução é **bloqueada por padrão**.

Isso significa que:
- a ausência de autorização explícita implica proibição
- a disponibilidade de ferramentas não altera o status de bloqueio
- o modo de execução, por si só, **não desbloqueia** a execução

> **Executar exige permissão explícita.  
> Não executar é o estado natural do sistema.**

---

## 4.3 Autorização como Ato Consciente e Deliberado

A autorização de execução é um **ato humano consciente**, nunca um efeito colateral do fluxo.

A autorização deve ser:
- explícita
- específica
- contextualizada
- limitada no tempo e no escopo

Autorizações genéricas, implícitas ou permanentes são **proibidas**.

---

## 4.4 Autoridade de Autorização

A autoridade para autorizar execução:
- é sempre humana
- é explicitamente assumida
- não pode ser delegada à IA

A definição de **quem** pode autorizar:
- pertence ao contexto organizacional
- deve ser conhecida antes da execução
- deve ser registrada quando exercida

Nenhuma execução é válida sem **responsável humano identificável**.

---

## 4.5 Guards de Execução

Guards são **condições normativas mínimas** que devem existir antes de qualquer execução assistida.

Eles:
- não são checklists técnicos
- não garantem sucesso
- existem para **reduzir risco sistêmico**

A ausência de qualquer guard implica **proibição automática da execução**.

---

## 4.6 Guards Normativos Mínimos

Independentemente do contexto, a execução só pode ser considerada quando:

- o **modo de execução** está explicitamente declarado
- as **decisões humanas relevantes** estão registradas
- o **escopo da execução** está claramente delimitado
- os **impactos esperados** são conhecidos
- a **reversibilidade** foi avaliada
- a **responsabilidade humana** está explicitada

Estes guards são **necessários**, mas não necessariamente suficientes.

---

## 4.7 Escopo e Limitação da Autorização

Toda autorização de execução deve:
- delimitar claramente **o que pode ser executado**
- excluir explicitamente o que **não** está autorizado
- ser válida apenas para o contexto em que foi concedida

A autorização:
- não é transferível
- não é reutilizável por padrão
- não sobrevive a mudanças significativas de contexto

---

## 4.8 Validade Temporal da Autorização

Autorizações de execução possuem **validade temporal limitada**.

Uma autorização expirada é considerada **inexistente**, mesmo que:
- o contexto pareça similar
- a execução ainda não tenha ocorrido
- a intenção original persista

Execução baseada em autorização expirada é proibida.

---

## 4.9 Relação entre Autorização e Guards

A autorização:
- **não substitui** os guards
- **não enfraquece** os guards
- **não ignora** os guards

Guards existem para proteger o sistema **inclusive de autorizações mal avaliadas**.

Se os guards não são satisfeitos, a execução deve ser bloqueada, independentemente da autorização concedida.

---

## 4.10 Proibição de Bypass e Exceções Implícitas

É explicitamente proibido:
- executar “só desta vez”
- ignorar guards por urgência
- criar exceções não registradas
- usar falhas de processo como justificativa

Exceções só existem quando:
- explicitadas previamente
- conscientemente aceitas
- registradas como tais
- compatíveis com os princípios normativos

---

## 4.11 Encerramento do Capítulo

Autorização e guards existem para **proteger o sistema de seus próprios incentivos**.

> **Se a execução parece inevitável,  
> os guards são o último direito de dizer não.**
