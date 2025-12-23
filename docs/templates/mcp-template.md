# MCP — <Nome do Produto> / <Nome da Feature> (v<versão>)

Este documento define o **Machine-Consumable Plan (MCP)** para a execução de uma
feature específica do produto **<Nome do Produto>**, no contexto do
**AI-Assisted SDLC Workflow**.

O MCP é um **contrato operacional** entre humanos e agentes de IA, descrevendo
exatamente **o que pode, o que não pode e como executar** uma feature.

---

## 1. Identificação

- Produto: <Nome do Produto>
- Feature: <Nome ou ID da Feature>
- Versão: <versão>
- Status: <rascunho | aprovado para execução>

---

## 2. Artefatos de Origem (Obrigatórios)

Este MCP **só pode existir** se todos os artefatos abaixo estiverem aprovados:

- PRD-Lite — <referência>
- Context Pack — <referência>
- Guidelines Técnicos — <referência>
- Visão de Arquitetura — <referência>
- Action Plan — <referência>

Nenhuma decisão fora desses documentos é permitida durante a execução.

---

## 3. Papéis e Responsabilidades

### Human Lead Engineer

Responsabilidades:

- Aprovar este MCP
- Definir a ferramenta de execução (ex.: Codex, Claude Code)
- Revisar resultados e diffs
- Decidir continuidade ou rollback

---

### AI Dev Agent

Responsabilidades:

- Executar exatamente as etapas descritas neste MCP
- Não extrapolar escopo
- Não introduzir dependências não autorizadas
- Interromper execução em caso de dúvida ou erro

---

## 4. Escopo Autorizado

O agente **está autorizado** a:

- <ação permitida 1>
- <ação permitida 2>

O agente **não está autorizado** a:

- <ação proibida 1>
- <ação proibida 2>

---

## 5. Plano de Execução

As etapas abaixo devem ser executadas **na ordem**, sem omissões:

1. <etapa 1>
2. <etapa 2>
3. <etapa 3>

Cada etapa deve ser considerada **atômica**.

---

## 6. Checkpoints Humanos Obrigatórios

A execução **deve ser interrompida** para aprovação humana nos seguintes pontos:

- <checkpoint 1>
- <checkpoint 2>

---

## 7. Regras de Falha

- <condição de falha>
- <comportamento esperado do agente>
- <quando interromper execução>

Nenhum workaround implícito é permitido.

---

## 8. Regras de Commit e Versionamento

- Commits devem ser pequenos e descritivos
- Commits só podem ocorrer após aprovação humana
- Cada commit deve referenciar a feature associada

---

## 9. Rastreabilidade

Este MCP garante rastreabilidade explícita entre:

PRD → Context → Guidelines → Arquitetura → Action Plan → Execução

---

## Estado do Documento

- **Tipo:** Template de Machine-Consumable Plan (MCP)  
- **Workflow:** AI-Assisted SDLC  
- **Versão:** v0.1  
- **Uso:** Deve ser copiado e preenchido para cada feature executada por agentes
