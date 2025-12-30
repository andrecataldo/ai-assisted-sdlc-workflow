# 🤖 Agents — Artefatos Operacionais (não normativos)

Este diretório contém **prompts/roteiros de agentes** usados para apoiar a criação de artefatos do workflow.

## Princípio de Autoridade

**Norma governa agente. Agente não governa norma.**

- A **versão vigente** do workflow é a **v0.2**: `docs/README-v0.2.md`
- A **v0.3** está **normativamente definida e encerrada** (não vigente): `docs/v0.3/`
- Agentes são **mecanismos operacionais** que devem obedecer às normas e contratos definidos.

Quando houver conflito entre o comportamento de um agente e os documentos normativos,
**prevalece o documento normativo**.

---

## O que agentes podem (e não podem)

### Agentes podem
- gerar rascunhos de artefatos (PRD-Lite, Context Pack, MCP+, etc.)
- sugerir estrutura e preenchimento guiado
- propor perguntas e checagens de consistência
- resumir contexto e registrar decisões (quando solicitado)

### Agentes não podem
- criar “novas regras” do workflow
- flexibilizar limites normativos por conta própria
- reabrir decisões bloqueadas sem novo MCP+
- executar código ou sugerir execução quando o modo não permitir

---

## Compatibilidade por versão

- **v0.2 (vigente):** agentes podem ser usados para criar artefatos e apoiar consistência, sem execução.
- **v0.3 (normativa encerrada):** agentes podem ser usados para simulações e checagens, respeitando modos/guards (quando aplicável).
- **v0.1:** arquivos legacy podem existir por histórico, mas não devem governar uso atual.

---

## Arquivos neste diretório

- `context-generator.md`  
  Agente operacional recomendado para v0.2+ (Context Pack).
- `action-plan-generator.md`  
  Agente operacional recomendado para planos de ação (uso auxiliar).
- `context-generator-v0.1.md`  
  **Legacy** (preservado por histórico). Não recomendado para uso atual.

---

## Como evoluir agentes com segurança

Ao alterar um agente:
1. manter o header de status atualizado
2. declarar compatibilidade com v0.2/v0.3
3. nunca introduzir regras novas (isso exige capítulos/README/checkpoint)
4. se o agente mudar comportamento de forma relevante, registrar em checkpoint (quando fizer sentido)

---

## Nota

Agentes são úteis para reduzir fricção e padronizar geração de artefatos,
mas não substituem julgamento humano nem o corpo normativo do workflow.
