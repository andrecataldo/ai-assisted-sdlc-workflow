# MCP — Academic Paper Builder / Feature 01 (v0.1)

Este documento define o **Machine-Consumable Plan (MCP)** para a execução da
**Feature 01 — MVP CLI** do produto *Academic Paper Builder*.

O MCP é um **plano operacional executável por agentes de IA**, derivado
exclusivamente de artefatos aprovados no AI-Assisted SDLC Workflow.

---

## 1. Identificação

- **Produto:** Academic Paper Builder
- **Feature:** Feature 01 — MVP CLI
- **Versão:** v0.1
- **Status:** Aprovado para execução por IA

---

## 2. Artefatos de Origem (Obrigatórios)

Este MCP foi gerado a partir dos seguintes artefatos aprovados:

- PRD-Lite — Academic Paper Builder (v0.1)
- Context Pack — Academic Paper Builder (v0.1)
- Guidelines Técnicos — Academic Paper Builder (v0.1)
- Visão de Arquitetura — Academic Paper Builder (v0.1)
- Action Plan — Feature 01 (v0.1)

Nenhuma decisão fora desses documentos é permitida durante a execução.

---

## 3. Papel dos Atores

### Human Lead Engineer

Responsabilidades:
- Aprovar este MCP
- Selecionar a ferramenta de execução (Codex, Claude Code, etc.)
- Revisar diffs e resultados
- Decidir rollback ou continuação

---

### AI Dev Agent

Responsabilidades:
- Executar exatamente as etapas descritas
- Não extrapolar escopo
- Não introduzir dependências não autorizadas
- Reportar erros explicitamente

---

## 4. Escopo Autorizado

O agente **está autorizado** a:

- Criar e modificar arquivos do projeto
- Implementar a CLI conforme especificado
- Criar testes automatizados
- Executar comandos locais necessários

O agente **não está autorizado** a:

- Criar novas features
- Gerar conteúdo acadêmico
- Introduzir integrações externas
- Alterar arquitetura definida
- Executar ações irreversíveis sem confirmação

---

## 5. Plano de Execução (Resumo)

O agente deve executar as seguintes etapas, **na ordem**:

1. Preparar estrutura do projeto
2. Implementar CLI básica
3. Implementar validações
4. Implementar testes automatizados
5. Executar testes
6. Reportar status final

Cada etapa deve ser considerada **atômica**.

---

## 6. Checkpoints Humanos Obrigatórios

A execução **deve parar** nos seguintes pontos para aprovação humana:

- Após implementação da CLI
- Após criação dos testes
- Antes de qualquer commit final

---

## 7. Regras de Falha

- Qualquer erro de validação → interromper execução
- Falha em testes → interromper execução
- Dúvida de escopo → interromper e pedir instrução

Nenhum workaround implícito é permitido.

---

## 8. Regras de Commit

- Commits devem ser pequenos e descritivos
- Cada commit deve referenciar a Feature 01
- Commits só podem ocorrer após aprovação humana

---

## 9. Rastreabilidade

Este MCP garante rastreabilidade completa entre:

PRD → Context → Guidelines → Arquitetura → Action Plan → Execução

---

## Estado do Documento

- **Tipo:** Machine-Consumable Plan (MCP)
- **Produto:** Academic Paper Builder
- **Feature:** Feature 01
- **Versão:** v0.1
- **Gerado por:** MCP Generator v0.1
