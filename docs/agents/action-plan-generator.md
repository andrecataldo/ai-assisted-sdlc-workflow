# Action Plan Generator — v0.1

## 1. Propósito

O Action Plan Generator é responsável por transformar um Feature Intent aprovado
em um plano de execução técnico claro, incremental e revisável.

O plano gerado deve permitir que um AI Dev Agent implemente a feature
de forma controlada, mantendo o escopo definido e respeitando os guardrails do SDLC com IA.

Este artefato atua como ponte explícita entre:
- intenção (Feature Intent)
- execução (implementação por IA)

---

## 2. Inputs e Pré-condições

### 2.1 Inputs obrigatórios

O Action Plan Generator deve ser executado somente quando todos os seguintes
artefatos estiverem disponíveis e aprovados:

- Feature Intent completo e aprovado pelo Human Lead Engineer
- Definição clara do recorte da feature (escopo In / Out)
- Critérios de aceite definidos

O Feature Intent é o **único insumo primário** para a geração do Action Plan.
Nenhum contexto adicional deve ser assumido implicitamente.

### 2.2 Pré-condições

Antes de gerar o Action Plan, deve ser garantido que:

- O Feature Intent possui status **“Aprovado”**
- O escopo está fechado e não há decisões pendentes
- As restrições técnicas estão explícitas
- O plano não está sendo gerado para fins exploratórios ou especulativos

Caso qualquer uma dessas pré-condições não seja atendida,
o Action Plan Generator deve **interromper a geração** e solicitar correções.

---

## 3. Estrutura do Action Plan

O Action Plan gerado deve seguir **obrigatoriamente** a estrutura abaixo.
Nenhuma seção pode ser omitida ou fundida.

### 3.1 Objetivo do Plano

Descrição sucinta do que será implementado,
derivada diretamente da Intenção (Outcome) do Feature Intent.

### 3.2 Estratégia Geral

Breve explicação da abordagem escolhida para implementar a feature,
incluindo:
- divisão em etapas
- decisões técnicas de alto nível
- justificativas alinhadas às restrições técnicas

Esta seção **não deve** conter detalhes de implementação fina.

### 3.3 Etapas de Execução

Lista ordenada de etapas pequenas e incrementais.
Cada etapa deve conter:

- **Descrição da etapa**
- **Arquivos/módulos afetados**
- **Resultado esperado ao final da etapa**
- **Critério simples de verificação**

As etapas devem:
- ser executáveis de forma independente
- evitar grandes mudanças transversais
- permitir validação progressiva

### 3.4 Checkpoints Humanos Obrigatórios

Identificação explícita dos pontos onde o Human Lead Engineer
deve revisar e aprovar antes de prosseguir.

Nenhuma etapa após um checkpoint pode ser executada
sem aprovação explícita.

### 3.5 Riscos e Mitigações

Lista curta de riscos técnicos relevantes identificados durante o planejamento,
com respectivas estratégias de mitigação.

### 3.6 Critério de Conclusão do Plano

Condições objetivas que indicam que:
- o plano foi executado com sucesso
- os critérios de aceite do Feature Intent foram atendidos

---

## 4. Regras, Limites e Checkpoints

### 4.1 Regras de Planejamento

- O plano deve respeitar integralmente o escopo definido no Feature Intent.
- O plano **não deve**:
  - introduzir novas funcionalidades
  - expandir escopo implicitamente
  - assumir requisitos não explicitados
- O plano deve priorizar simplicidade e previsibilidade,
  evitando refactors amplos ou otimizações prematuras.

### 4.2 Limites de Autonomia

- O Action Plan Generator **não pode**:
  - tomar decisões arquiteturais não explicitadas
  - adicionar dependências externas sem aprovação
  - propor mudanças fora da superfície de impacto definida
- Qualquer decisão fora do escopo explícito deve ser:
  - claramente sinalizada
  - proposta como pergunta ao Human Lead Engineer

### 4.3 Checkpoints Humanos

- O plano deve indicar explicitamente:
  - pontos de revisão obrigatória
  - quais decisões exigem aprovação humana
- A execução de etapas após um checkpoint
  depende de aprovação explícita do Human Lead Engineer.

---

## 5. Critérios de Qualidade do Action Plan

Um Action Plan gerado só pode ser considerado válido se atender aos seguintes critérios:

- O plano é diretamente derivado de um Feature Intent aprovado
- O escopo do plano está alinhado integralmente ao escopo In / Out definido
- As etapas são:
  - pequenas
  - ordenadas
  - incrementalmente verificáveis
- Cada etapa possui um resultado observável
- Existem checkpoints humanos explícitos antes de decisões sensíveis
- O plano evita:
  - refactors amplos
  - mudanças transversais desnecessárias
  - otimizações prematuras
- O plano é curto o suficiente para ser revisado facilmente
- O plano é claro o suficiente para ser executado sem ambiguidade
