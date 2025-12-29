# 7️⃣ Observabilidade Cognitiva e Rastreabilidade

> **Status:** Normativo  
> **Versão do workflow:** v0.3  
> **Dependência:**  
> - Capítulo 2 — Princípios Normativos da Execução Assistida  
> - Capítulo 3 — Modos de Execução  
> - Capítulo 4 — Autorização e Guards de Execução  
> - Capítulo 5 — Contrato de Qualidade para Execução  
> - Capítulo 6 — Autoridade, Responsabilidade e Limites da IA  
> **Autoridade:** Define os requisitos mínimos de explicabilidade, rastreabilidade e aprendizado do workflow

---

## 7.1 Propósito deste Capítulo

Este capítulo estabelece os **princípios normativos de observabilidade cognitiva** aplicáveis a qualquer forma de execução assistida por IA.

A observabilidade cognitiva existe para garantir que seja possível, **após a execução**, compreender:

- o que foi feito
- por que foi feito
- sob quais decisões
- com quais hipóteses
- e com quais expectativas de resultado

Sem observabilidade cognitiva, a execução é considerada **opaca, não auditável e inválida** do ponto de vista do workflow.

---

## 7.2 Observabilidade Cognitiva ≠ Observabilidade Técnica

O AI-Assisted SDLC Workflow distingue explicitamente:

- **Observabilidade técnica**: métricas, logs, tracing, eventos de sistema
- **Observabilidade cognitiva**: decisões, hipóteses, contexto e intenção humana

A observabilidade técnica **não substitui** a observabilidade cognitiva.

Mesmo uma execução tecnicamente perfeita é considerada falha se não puder ser **explicada cognitivamente**.

---

## 7.3 Princípio da Explicabilidade Posterior Obrigatória

Toda execução assistida por IA deve ser **explicável a posteriori** por um humano.

Isso implica que deve ser possível reconstruir, de forma razoável:

- o modo de execução vigente
- a autorização concedida
- as decisões humanas relevantes
- o contrato de qualidade aceito
- o papel desempenhado pela IA
- o resultado esperado versus o observado

Execuções que não possam ser explicadas posteriormente são consideradas **falhas sistêmicas**, independentemente do resultado obtido.

---

## 7.4 Elementos Mínimos de Observabilidade Cognitiva

A observabilidade cognitiva mínima exige rastreabilidade explícita de:

- **Decisões** — o que foi decidido e por quem  
- **Hipóteses** — suposições assumidas como verdadeiras  
- **Contexto** — informações fornecidas à IA no momento da execução  
- **Intenção** — por que a execução foi considerada necessária  
- **Expectativa** — qual resultado era esperado  
- **Resultado** — o que de fato ocorreu  

A ausência relevante de qualquer desses elementos invalida a observabilidade cognitiva.

---

## 7.5 Relação com MCP+ e Checkpoints

A observabilidade cognitiva se apoia diretamente em:

- **MCP+**, como contrato de contexto e decisão
- **Checkpoints**, como snapshots cognitivos do estado do sistema

Execuções que não possam ser vinculadas a:
- um MCP+ válido
- um checkpoint vigente

são consideradas **não rastreáveis** e, portanto, inválidas.

---

## 7.6 Observabilidade como Condição para Aprendizado

A execução assistida por IA só gera aprendizado quando é **observável**.

Sem observabilidade cognitiva:
- erros não podem ser analisados
- acertos não podem ser explicados
- melhorias não podem ser justificadas

O workflow privilegia **aprendizado consciente** sobre otimização cega.

---

## 7.7 Proibição de Execução Opaca

É explicitamente proibido:

- executar sem registro de decisão
- executar sem contexto rastreável
- executar sem expectativa declarada
- depender exclusivamente de logs técnicos para explicação

Execução opaca é tratada como **violação de governança**, não como limitação técnica.

---

## 7.8 Proporcionalidade da Observabilidade ao Risco

O nível de observabilidade exigido deve ser **proporcional ao risco da execução**.

- execuções de maior impacto exigem maior nível de explicabilidade
- Hot Run exige o mais alto nível de observabilidade cognitiva
- Dry Run exige observabilidade suficiente para avaliação crítica

A ausência de proporcionalidade invalida a execução.

---

## 7.9 Responsabilidade Humana pela Observabilidade

A responsabilidade por garantir observabilidade cognitiva é **humana**, não da IA.

A IA pode:
- auxiliar na geração de registros
- sugerir resumos ou explicações

A IA não pode:
- decidir o que é suficiente para observabilidade
- omitir informações relevantes
- substituir o julgamento humano sobre explicabilidade

---

## 7.10 Violação de Observabilidade Cognitiva

A violação dos princípios deste capítulo caracteriza:

- falha de governança
- execução não auditável
- risco sistêmico oculto

Resultados positivos **não legitimam** execuções cognitivamente opacas.

---

## 7.11 Encerramento do Capítulo

A observabilidade cognitiva é o que transforma execução em **conhecimento**, não apenas em ação.

> **Se não conseguimos explicar depois,  
> não deveríamos ter executado antes.**
