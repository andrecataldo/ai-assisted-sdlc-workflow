# 2️⃣ Princípios Normativos da Execução Assistida

> **Status:** Normativo (fundacional)  
> **Versão do workflow:** v0.3  
> **Dependência:** v0.2  
> **Autoridade:** Governa todos os capítulos subsequentes da v0.3

---

## 2.1 Propósito deste Capítulo

Este capítulo estabelece os **princípios normativos inegociáveis** que regem qualquer forma de execução assistida por IA no AI-Assisted SDLC Workflow.

Esses princípios:
- **precedem** regras específicas
- **limitam** decisões futuras
- **governam** playbooks, templates e automações derivadas

Qualquer norma, mecanismo ou automação da v0.3 que viole estes princípios é considerada **inválida**, independentemente de ganhos de eficiência ou conveniência.

---

## 2.2 Execução como Consequência, não como Objetivo

A execução assistida por IA **não é um objetivo do workflow**.

Ela só pode ocorrer como **consequência direta** de:
- decisões humanas explícitas
- contratos cognitivos estáveis
- contexto preservado e auditável

Nenhuma iniciativa pode justificar execução com base em:
- urgência
- curiosidade
- conveniência técnica
- pressão externa

> **Executar rápido não é sucesso.  
> Executar sob controle é o único critério aceitável.**

---

## 2.3 Soberania Humana Intransferível

A autoridade decisória no workflow é **exclusivamente humana**.

A IA:
- pode sugerir
- pode simular
- pode executar quando autorizada
- **não pode decidir**

Nenhuma decisão humana pode ser:
- inferida implicitamente pela IA
- substituída por heurística
- “assumida” por padrão de uso

A soberania humana **não é delegável**, nem mesmo parcialmente.

---

## 2.4 Autorização Explícita como Condição Necessária

Toda execução assistida exige **autorização explícita**.

Autorização:
- não é implícita
- não é inferida por contexto
- não é herdada de interações anteriores

A ausência de autorização explícita implica **proibição automática de execução**, independentemente do modo técnico disponível.

---

## 2.5 Primazia da Auditabilidade Cognitiva

Nenhuma execução é considerada válida se não puder ser **explicada posteriormente**.

A auditabilidade cognitiva exige que seja possível reconstruir:
- quais decisões humanas foram tomadas
- quais hipóteses estavam vigentes
- qual contexto foi fornecido à IA
- qual resultado era esperado

Execução sem explicabilidade posterior é considerada **falha sistêmica**, mesmo que tecnicamente bem-sucedida.

---

## 2.6 Reversibilidade como Direito Arquitetural

A reversibilidade é um **direito arquitetural**, não uma conveniência técnica.

Sempre que possível, a execução deve:
- permitir rollback
- permitir invalidação explícita
- preservar checkpoints anteriores

Quando a reversibilidade não for possível, isso deve ser:
- explicitado previamente
- conscientemente aceito
- registrado como exceção

Execuções irreversíveis por omissão são proibidas.

---

## 2.7 Conservadorismo Progressivo

Na presença de incerteza, o workflow deve **preferir menos execução, não mais**.

Este princípio estabelece que:
- novas capacidades de execução devem ser introduzidas gradualmente
- o ônus da prova é de quem propõe executar
- ausência de evidência não autoriza ação

O sistema deve evoluir por **ampliação controlada**, nunca por salto especulativo.

---

## 2.8 Separação Estrita entre Norma, Procedimento e Forma

Este workflow distingue explicitamente:
- **Norma** (o que é permitido ou proibido)
- **Procedimento** (como aplicar a norma)
- **Forma** (como registrar a aplicação)

Normas residem nos capítulos da v0.3.  
Procedimentos residem em playbooks.  
Formas residem em templates.

Nenhum template ou playbook pode:
- criar nova norma
- flexibilizar um princípio
- contradizer este capítulo

---

## 2.9 Precedência Normativa

Em caso de conflito, a precedência é:

1. Princípios Normativos (este capítulo)
2. Demais capítulos normativos da v0.3
3. Playbooks
4. Templates
5. Instâncias específicas

Nenhuma instância concreta pode invalidar um princípio normativo.

---

## 2.10 Violação de Princípios

Qualquer violação destes princípios caracteriza:
- erro de governança
- falha de uso do workflow
- risco sistêmico

Violações **não podem** ser justificadas por:
- sucesso pontual
- ganho de velocidade
- redução de custo
- pressão organizacional

O workflow privilegia **integridade sobre eficiência**.

---

## 2.11 Encerramento do Capítulo

Este capítulo estabelece o **fundamento normativo da v0.3**.

Todos os capítulos subsequentes:
- dependem deste
- não podem contradizê-lo
- devem citá-lo implicitamente como base de autoridade

> **Se a execução ameaça a governança,  
> a execução está errada — nunca a governança.**
