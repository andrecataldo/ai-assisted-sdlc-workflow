# Workflow de Desenvolvimento com IA (SDLC) — v0.1

## 1. Objetivo do Projeto

Este repositório documenta e evolui um **Workflow de Desenvolvimento de Software com IA**, concebido para viabilizar o uso consciente, governado e escalável de **Vibe Coding** ao longo de todo o **SDLC (Software Development Life Cycle)**.

O objetivo **não é apenas desenvolver software com IA**, mas **criar um processo reproduzível** no qual:

- A IA atua como **executora técnica especializada**
- O humano atua como **arquiteto, revisor e responsável final**
- A intenção do desenvolvimento é explícita, versionada e auditável
- O risco de autonomia excessiva da IA é mitigado por design

Este workflow é **agnóstico de ferramentas**, focado em **engenharia**, e aplicável a projetos reais de médio e grande porte.

---

## 2. Premissas Operacionais do SDLC com IA

Estas premissas funcionam como um **contrato cognitivo do workflow**.  
Todas as decisões técnicas e de processo devem respeitá-las.

### Premissas Técnicas

- **Stack dominante:** Python  
- **Controle de versão:** GitHub e/ou Azure DevOps  
- **Ambiente padrão:** Linux / Ubuntu  
- **Objetivo principal:** Criação de features end-to-end  

### Modelo Mental

- A **IA atua como executora**
- O **humano atua como arquiteto, revisor e responsável final**
- Nenhuma mudança relevante é considerada válida sem validação humana explícita
- A responsabilidade técnica **nunca** é delegada à IA

---

## 3. Papéis no Workflow de Desenvolvimento com IA

### 3.1. Human Lead Engineer

Responsável final pela integridade técnica do sistema.

**Responsabilidades:**
- Definir a intenção da feature
- Estabelecer critérios de qualidade
- Aprovar planos de execução
- Revisar diffs e Pull Requests
- Tomar decisões arquiteturais
- Assumir responsabilidade técnica final

---

### 3.2. AI Dev Agent

Agente executor especializado.

**Responsabilidades:**
- Propor planos de ação
- Implementar alterações no código
- Criar e executar testes
- Iterar sobre falhas e feedback
- Documentar alterações conforme solicitado

> A IA **não possui autonomia decisória** sobre arquitetura, escopo, releases ou priorização.

---

## 4. SDLC Orientado à Intenção (Intent-Centric)

Este workflow é explicitamente **orientado à intenção**, não à tarefa.

### 4.1. Feature Intent / Intent Spec

A **Feature Intent** é o artefato central do SDLC com IA.  
Ela atua como ponte entre **ideia/backlog** e **execução por agentes**.

Sem uma Feature Intent aprovada:
- Nenhum Action Plan é gerado
- Nenhuma execução de código é iniciada

A Feature Intent pode existir como:
- Seção dedicada no PRD-Lite, ou
- Artefato próprio (`feature-intent.md`) — **recomendado**

Ela é o **insumo primário** para:
- Action Plan Generator
- Execução dos AI Dev Agents

---

## 5. Ferramentas como *Capabilities*, não como Etapas

Este workflow **não depende de ferramentas específicas**.

As ferramentas são tratadas como **capacidades do SDLC**, intercambiáveis ao longo do tempo.

| Capability | Exemplos |
|---------|---------|
| Planejamento da feature | ChatGPT, Cursor |
| Execução multi-arquivo | Cursor, Copilot |
| Execução via terminal | Claude Code |
| Revisão de mudanças | IDE + Humano |
| Qualidade e CI | Pytest, Ruff, MyPy, Pipelines |

---

## 6. Governança & Guardrails (Camada Transversal)

Estas regras se aplicam **a todas as fases** do workflow.

### Limites de Autonomia da IA
- Não alterar arquitetura sem aprovação
- Não criar dependências críticas sem validação
- Não abrir PR sem revisão humana

### Checkpoints Humanos Obrigatórios
- Aprovação da Feature Intent
- Aprovação do Action Plan
- Revisão final de Pull Request

### Ações Proibidas sem Aprovação
- Refactors amplos
- Mudanças de contrato público
- Alterações em pipelines ou infraestrutura

### Rastreabilidade
- Feature Intents versionadas
- Action Plans registrados
- Diffs revisados
- Versões documentadas

---

## 7. Visão Geral do Workflow

Em alto nível, o workflow segue o seguinte fluxo lógico:

1. Definição da intenção da feature  
2. Contextualização do produto e do sistema  
3. Planejamento da execução  
4. Implementação assistida por IA  
5. Revisão humana e hardening  
6. Atualização de artefatos e aprendizado  

O detalhamento completo da execução está documentado no **roadmap do projeto**.

👉 **Ver:**  
[Roadmap – Workflow de Desenvolvimento com IA](./roadmap.md)

---

## 8. Fases do Projeto de Construção do Workflow

Este repositório **documenta a criação do próprio workflow**, organizado nas seguintes fases:

1. **Fase 0 – Preparação**  
   - Escolha do projeto piloto  
   - Organização do repositório  
   - Definição das ferramentas  

2. **Fase 1 – Desenho Conceitual**  
   - Visão geral do SDLC com IA  
   - Regras de ouro  
   - Ciclos de uso  

3. **Fase 2 – PRD-Lite / Documento de Contexto**  
   - Template de PRD-Lite  
   - Versão do projeto piloto  

4. **Fase 3 – Guidelines Técnicos**  
   - Convenções de código  
   - Regras para uso da IA  

5. **Fase 4 – Design dos Assistentes**  
   - Context Generator  
   - Tech Guidelines Generator  
   - Action Plan Generator  
   - Architecture Generator  
   - MCP Generator  

6. **Fase 5 – Implementação dos Assistentes**  
   - Criação e validação prática  
   - Ajustes de prompts  

7. **Fase 6 – Piloto**  
   - Uso do workflow em uma feature real  
   - Pós-mortem  

8. **Fase 7 – Refinamento & Playbook**  
   - Ajustes finais  
   - Consolidação do workflow  

O detalhamento de cada fase está descrito no roadmap.

---

## 9. Artefatos Principais

- **Documento de Contexto (PRD-Lite)**  
  `docs/context/`

- **Feature Intent / Intent Spec**  
  `docs/context/feature-intent-template.md`

- **Guidelines Técnicos**  
  `docs/guidelines/`

- **Visão de Arquitetura**  
  `docs/architecture/`

- **Assistentes / Agents**  
  `docs/agents/`

---

## 10. Métricas de Avaliação do Workflow

O sucesso do workflow será avaliado por:

- Lead time de desenvolvimento de features
- Qualidade dos planos de ação gerados
- Incidência de bugs pós-deploy
- Esforço de onboarding de novos devs ou agentes
- Clareza e atualização dos artefatos

---

## 11. Status do Documento

- **Versão:** v0.1  
- **Estado:** Em evolução  
- **Próximo foco:**  
  - Templates de Feature Intent  
  - Prompts dos Assistentes  
  - Execução do piloto  

---

### Resumo Final

Este README define o **alicerce conceitual, operacional e de governança** do Workflow de Desenvolvimento com IA.

O foco não é acelerar código a qualquer custo, mas **integrar IA ao SDLC de forma responsável, intencional e sustentável**.
