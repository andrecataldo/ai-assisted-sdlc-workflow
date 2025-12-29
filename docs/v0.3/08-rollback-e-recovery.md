# 8️⃣ Rollback, Invalidação e Recovery Cognitivo

> **Status:** Normativo  
> **Versão do workflow:** v0.3  
> **Dependência:**  
> - Capítulo 2 — Princípios Normativos da Execução Assistida  
> - Capítulo 3 — Modos de Execução  
> - Capítulo 4 — Autorização e Guards de Execução  
> - Capítulo 5 — Contrato de Qualidade para Execução  
> - Capítulo 6 — Autoridade, Responsabilidade e Limites da IA  
> - Capítulo 7 — Observabilidade Cognitiva e Rastreabilidade  
> **Autoridade:** Define o direito, os limites e as condições de retorno após execução

---

## 8.1 Propósito deste Capítulo

Este capítulo estabelece as **normas de rollback, invalidação e recovery cognitivo** aplicáveis à execução assistida por IA.

Seu objetivo é garantir que o workflow:
- possa **voltar atrás** quando necessário
- consiga **invalidar decisões** conscientemente
- preserve a **integridade cognitiva** do sistema após falhas, desvios ou aprendizado

Rollback não é falha.  
A incapacidade de voltar é.

---

## 8.2 Reversibilidade como Direito Arquitetural

A reversibilidade é um **direito arquitetural fundamental** do workflow.

Sempre que tecnicamente possível, a execução deve:
- permitir retorno ao estado anterior
- preservar o contexto decisório
- manter rastreabilidade das mudanças

Quando a reversibilidade não for possível, isso deve ser:
- conhecido antes da execução
- explicitamente aceito
- registrado como exceção consciente

Execuções irreversíveis por omissão são proibidas.

---

## 8.3 Rollback Técnico vs Rollback Cognitivo

O workflow distingue explicitamente:

- **Rollback técnico** — desfazer efeitos em sistemas, código ou dados
- **Rollback cognitivo** — retornar ao estado decisório anterior

Rollback técnico **não substitui** rollback cognitivo.

Mesmo quando o rollback técnico é impossível, o rollback cognitivo **permanece obrigatório**.

---

## 8.4 Invalidação Explícita de Decisões

O rollback cognitivo exige a **invalidação explícita** de decisões anteriores.

A invalidação deve:
- ser declarada conscientemente
- identificar a decisão invalidada
- registrar o motivo da invalidação
- preservar o histórico da decisão original

Decisões invalidadas **não desaparecem**; elas deixam de governar.

---

## 8.5 Checkpoints como Âncoras de Recovery

Checkpoints funcionam como **âncoras de recovery cognitivo**.

Eles:
- capturam o estado decisório vigente
- delimitam versões de entendimento
- permitem retomada controlada após falhas

Qualquer rollback cognitivo deve referenciar:
- um checkpoint anterior válido
- ou criar um novo checkpoint de invalidação

---

## 8.6 Recovery Cognitivo Pós-Execução

O recovery cognitivo é o processo de **restabelecer governança** após execução.

Ele inclui:
- análise do desvio entre esperado e observado
- identificação de hipóteses inválidas
- atualização consciente do contexto
- redefinição de decisões, quando necessário

Recovery não é correção automática.  
É **reconstrução deliberada de entendimento**.

---

## 8.7 Relação entre Rollback e Responsabilidade

A execução pode ser revertida.  
A responsabilidade **não**.

Mesmo após rollback:
- a decisão original permanece registrada
- o responsável humano continua identificável
- o aprendizado deve ser preservado

Rollback não apaga responsabilidade; ele **protege o sistema de persistir no erro**.

---

## 8.8 Proibição de Rollback Implícito ou Silencioso

É explicitamente proibido:
- desfazer execução sem registrar
- “voltar atrás” sem invalidação explícita
- sobrescrever decisões sem histórico
- tratar rollback como erro a ser escondido

Rollback silencioso é considerado **violação de governança**.

---

## 8.9 Proporcionalidade do Recovery ao Impacto

O nível de recovery exigido deve ser **proporcional ao impacto da execução**.

- Hot Run exige recovery explícito e registrado
- Dry Run exige análise suficiente para aprendizado
- No Run não exige rollback, mas pode exigir revisão cognitiva

A ausência de proporcionalidade invalida o processo de recovery.

---

## 8.10 Violação de Rollback e Recovery

A violação dos princípios deste capítulo caracteriza:

- falha grave de governança
- execução irresponsável
- perda de integridade cognitiva

Resultados positivos **não legitimam** a ausência de rollback ou recovery adequado.

---

## 8.11 Encerramento do Capítulo

Rollback e recovery existem para garantir que o sistema **aprenda sem se cristalizar no erro**.

> **Se não conseguimos voltar com consciência,  
> avançar foi precipitado.**
