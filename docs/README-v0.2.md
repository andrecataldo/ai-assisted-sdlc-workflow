> 📘 **Checkpoints oficiais**
>
> Os checkpoints da versão vivem em `docs/checkpoints/` e são a fonte de verdade
> para retomada e continuidade do workflow.


# 📘 AI-Assisted SDLC Workflow — v0.2

## 1. Visão Geral

A versão **v0.2** do AI-Assisted SDLC Workflow introduz **contratos explícitos,
regras de consistência e memória operacional formal**, com o objetivo de tornar
o uso de IA:

- previsível
- rastreável
- resistente a loops improdutivos
- fiel à intenção humana ao longo do tempo

> 📌 A v0.2 não executa código.  
> Ela torna **seguro e controlável** executar no futuro.

---

## 2. Objetivo da v0.2

A v0.2 existe para resolver problemas comuns em workflows assistidos por IA:

- reabertura de decisões já tomadas
- renegociação implícita de escopo
- divergência entre documentos
- perda de contexto entre chats/agentes
- refinamento infinito sem avanço real

Ela transforma a gramática da v0.1 em um **sistema operacional cognitivo**.

---

## 3. O que mudou em relação à v0.1

### v0.1 — Gramática
- define *quais* artefatos existem
- define *como* eles se relacionam
- foca em estrutura e clareza

### v0.2 — Contratos e Memória
- define *quem manda quando há conflito*
- define *quando avançar e quando parar*
- define *como decisões são congeladas*
- define *como o estado é preservado*

---

## 4. Artefatos Canônicos da v0.2

### 4.1 Templates (normativos)

📁 `docs/templates/`

- `mcp-template.md`  
  > MCP básico (v0.1) — uso exploratório

- `mcp-plus-template.md`  
  > MCP+ (v0.2) — contrato forte por iteração

- `checkpoint-template.md`  
  > Template oficial de checkpoint (memória operacional)

---

### 4.2 Playbooks (regras do método)

📁 `docs/playbook/`

- `decision-locks.md`  
  > Congelamento explícito de decisões humanas

- `artifact-precedence.md`  
  > Matriz de autoridade entre artefatos

- `definition-of-ready.md`  
  > Critérios mínimos para avançar

- `definition-of-stop.md`  
  > Critérios explícitos de parada

- `checkpoint-strategy.md`  
  > Quando e por que criar checkpoints

---

### 4.3 Checkpoints (estado consolidado)

📁 `docs/checkpoints/`

- `checkpoint-v0.1-grammar.md`  
  > Fechamento da gramática inicial

- *(futuros)* `checkpoint-v0.2-*.md`

> 📌 Checkpoints são fonte de verdade para retomada.

---

## 5. Fluxo lógico da v0.2

1. Criar / revisar artefatos da v0.1 (PRD, Context, etc.)
2. Criar **MCP+** para a iteração
3. Definir **Decision Locks**
4. Validar **Definition of Ready**
5. Executar a iteração (sem código)
6. Parar segundo **Definition of Stop**
7. Criar **Checkpoint**
8. Decidir próximo passo conscientemente

---

## 6. Regras fundamentais da v0.2

- Nenhuma iteração relevante ocorre sem MCP+
- Decision Locks não são reabertos sem versionar
- Conflitos entre artefatos obedecem precedência
- Avançar sem DoR é violação do método
- Continuar sem objetivo claro é erro
- Sem checkpoint, não há retomada confiável

---

## 7. O que a v0.2 NÃO é

- não é execução de código
- não é CI/CD
- não é arquitetura de produto
- não é prompt engineering artesanal
- não substitui julgamento humano

---

## 8. Preparação para versões futuras

A v0.2 prepara explicitamente o terreno para:

- v0.3: preparação para execução controlada
- Hot Run com critérios claros
- múltiplos agentes e sessões
- uso por outros humanos além do autor

---

## 9. Como usar este README

- Leia este arquivo primeiro
- Em seguida, leia os playbooks
- Use os templates como contratos
- Use checkpoints para retomada
- Não pule etapas “porque a IA consegue”

---

## 10. Regra final

> **A IA pode acelerar o trabalho.  
> O método existe para impedir que ele descarrile.**
