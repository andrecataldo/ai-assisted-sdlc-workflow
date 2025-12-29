# 5️⃣ Contrato de Qualidade para Execução

> **Status:** Normativo  
> **Versão do workflow:** v0.3  
> **Dependência:**  
> - Capítulo 2 — Princípios Normativos da Execução Assistida  
> - Capítulo 3 — Modos de Execução  
> - Capítulo 4 — Autorização e Guards de Execução  
> **Autoridade:** Define quando algo é considerado aceitável para execução

---

## 5.1 Propósito deste Capítulo

Este capítulo estabelece o **Contrato de Qualidade para Execução**, definindo os **critérios normativos mínimos** que devem ser atendidos para que uma execução assistida por IA seja considerada aceitável.

O contrato de qualidade:
- **não garante sucesso**
- **não elimina risco**
- **não substitui autorização ou guards**

Ele existe para evitar a execução de artefatos, decisões ou ações **intrinsecamente frágeis**, mesmo quando autorizadas.

---

## 5.2 Prontidão para Executar ≠ Prontidão para Decidir

O workflow distingue explicitamente:

- **Prontidão para decidir**: suficiente para escolher um caminho
- **Prontidão para executar**: suficiente para produzir efeitos reais

Algo pode estar pronto para decisão e **não** estar pronto para execução.

A execução só pode ser considerada quando a prontidão para executar estiver explicitamente reconhecida.

---

## 5.3 Qualidade como Contrato, não como Aspiração

Qualidade, no contexto da execução assistida, é um **contrato consciente**, não uma expectativa implícita.

Esse contrato:
- define o nível mínimo aceitável
- explicita limitações conhecidas
- reconhece riscos residuais

A ausência de um contrato de qualidade explícito implica **proibição automática da execução**.

---

## 5.4 Dimensões Normativas da Qualidade

A avaliação de qualidade para execução deve considerar, no mínimo, as seguintes dimensões:

- **Clareza** — o que será executado é compreendido sem ambiguidade
- **Coerência** — não há conflitos relevantes com decisões vigentes
- **Completude** — informações essenciais estão presentes
- **Consistência** — artefatos envolvidos não se contradizem
- **Compreensibilidade** — humanos conseguem explicar o que será feito
- **Adequação ao risco** — o nível de qualidade é compatível com o impacto esperado

A ausência grave em qualquer dimensão invalida a prontidão para execução.

---

## 5.5 Adequação da Qualidade ao Modo de Execução

O nível mínimo de qualidade exigido **varia conforme o modo de execução**.

- **No Run**: não exige contrato de qualidade para execução
- **Dry Run**: exige qualidade suficiente para simulação responsável
- **Hot Run**: exige o mais alto nível de qualidade aceitável no contexto

Executar em Hot Run com qualidade compatível apenas com Dry Run é proibido.

---

## 5.6 Tolerância a Erro e Qualidade Aceita

Todo contrato de qualidade deve tornar explícito:

- quais erros são toleráveis
- quais erros são inaceitáveis
- quais riscos são conscientemente assumidos

A tolerância a erro **não pode** ser:
- implícita
- inferida por histórico
- justificada retroativamente

Qualidade aceita deve ser **declarada antes da execução**.

---

## 5.7 Qualidade e Responsabilidade Humana

A aceitação do contrato de qualidade implica **responsabilidade humana explícita**.

Aceitar qualidade insuficiente:
- é uma decisão consciente
- carrega responsabilidade proporcional ao risco
- deve ser registrada como tal

A IA não pode aceitar, ajustar ou relativizar o contrato de qualidade.

---

## 5.8 Proibição de Execução por Otimismo

É explicitamente proibido executar com base em:

- “provavelmente está bom”
- “a IA costuma acertar”
- “se der errado, corrigimos depois”
- “é só um teste em produção”

O contrato de qualidade existe para **bloquear otimismo não fundamentado**.

---

## 5.9 Relação com Playbooks e Templates

Este capítulo define **o que** é qualidade aceitável.

Playbooks podem definir:
- **como avaliar** qualidade
- **como documentar** o contrato

Templates podem definir:
- **como registrar** a aceitação da qualidade

Nenhum playbook ou template pode:
- reduzir o nível mínimo exigido aqui
- relativizar dimensões normativas
- substituir a decisão humana de aceitação

---

## 5.10 Violação do Contrato de Qualidade

A execução que viole o contrato de qualidade caracteriza:

- falha de governança
- uso indevido do workflow
- risco sistêmico assumido indevidamente

Resultados positivos **não** validam violações do contrato.

---

## 5.11 Encerramento do Capítulo

O contrato de qualidade existe para **proteger o sistema de executar antes de estar pronto**.

> **Se a execução exige fé,  
> ela ainda não merece acontecer.**
