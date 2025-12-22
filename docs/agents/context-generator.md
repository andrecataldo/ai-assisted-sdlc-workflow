# Context Generator — v0.1

## 1. Propósito
Gerar um **Context Pack** objetivo e reutilizável para IA, a partir de um **PRD-Lite aprovado**.
O Context Pack deve permitir que um AI Dev Agent:
- entenda o produto e o problema
- conheça o recorte (MVP/feature)
- respeite restrições e guardrails
- opere com mínima inferência

## 2. Inputs e Pré-condições

### 2.1 Inputs obrigatórios
- PRD-Lite aprovado (única fonte primária)

### 2.2 Pré-condições
- O PRD-Lite está completo e com escopo definido
- Termos críticos estão definidos (ex.: “paper”, “seção”, “CLI”)
- Restrições técnicas e não-funcionais explícitas

Se qualquer pré-condição falhar: **interromper** e pedir correção no PRD-Lite.

## 3. Saída: Context Pack (formato obrigatório)
O Context Pack deve ser gerado em Markdown seguindo esta estrutura (não omitir seções):

### 3.1 Product Snapshot
- Nome do produto
- Quem usa
- Por que existe
- Valor entregue

### 3.2 Problem & Outcome
- Problema (1–2 parágrafos)
- Outcome mensurável / critério de sucesso

### 3.3 Scope (In / Out)
- In: lista objetiva
- Out: lista objetiva
- Anti-objetivos (o que NÃO fazer)

### 3.4 Users & Use Cases
- Perfis de usuário
- 3–5 casos principais (1 linha cada)

### 3.5 Constraints & Guardrails
- Restrições técnicas (stack, execução, ambiente)
- Limites (ex.: tamanhos, contagens)
- Proibições explícitas (ex.: não inventar referências)
- Checkpoints humanos obrigatórios

### 3.6 Acceptance Criteria
Lista objetiva do que define “pronto”.

### 3.7 Risks & Open Questions
- Riscos principais
- Questões em aberto (se existirem) — **sem inventar**

## 4. Regras do gerador (limites de autonomia)
- Não inventar requisitos ausentes no PRD-Lite
- Não “melhorar” escopo nem sugerir features extras dentro do Context Pack
- Se algo for necessário e não estiver no PRD-Lite, registrar em **Open Questions** e parar.

## 5. Critérios de Qualidade
O Context Pack é válido se:
- cabe em 1–2 páginas (Markdown)
- contém escopo claro (In/Out)
- não tem inferências sobre stack/arquitetura não presentes no PRD-Lite
- tem guardrails acionáveis (não genéricos)
