> 📘 **Checkpoints oficiais**
>
> Os checkpoints vivem em `docs/checkpoints/` e são a **fonte de verdade**
> para retomada, continuidade e governança do workflow.

# 📘 AI-Assisted SDLC Workflow — v0.2 (Versão Vigente)

## 🧭 Status da v0.2

- **Status:** versão vigente do método  
- **Uso autorizado:** adoção interna controlada  
- **Escopo:** governança cognitiva, contratos explícitos e memória operacional  
- **Execução de código / automação:** fora do escopo  

> ⚠️ A v0.2 **não executa código**.  
> Ela torna o trabalho **seguro, controlável e retomável**.

---

## 1. Visão Geral

A versão **v0.2** do AI-Assisted SDLC Workflow introduz **contratos explícitos,
regras de consistência e memória operacional formal**, com o objetivo de tornar
o uso de IA:

- previsível
- rastreável
- resistente a loops improdutivos
- fiel à intenção humana ao longo do tempo

Ela estabelece a **base estável do método**.

---

## 2. Objetivo da v0.2

A v0.2 existe para resolver problemas recorrentes em workflows assistidos por IA:

- reabertura silenciosa de decisões
- renegociação implícita de escopo
- divergência entre documentos
- perda de contexto entre sessões ou agentes
- refinamento infinito sem avanço real

Ela transforma a gramática da v0.1 em um **sistema operacional cognitivo**,
com regras claras de autoridade, avanço e parada.

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
- define *como o estado é preservado ao longo do tempo*

---

## 4. Artefatos Canônicos da v0.2

### 4.1 Templates (normativos para a v0.2)

📁 `docs/templates/`

- `mcp-template.md`  
  > MCP básico (v0.1) — uso exploratório

- `mcp-plus-template.md`  
  > MCP+ (v0.2) — contrato forte por iteração

- `checkpoint-template.md`  
  > Template oficial de checkpoint (memória operacional)

> ⚠️ Templates **não são opcionais** quando aplicáveis à v0.2.

---

### 4.2 Playbooks (apoio operacional)

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

> Playbooks **não criam norma nova**  
> e **não podem contradizer** a v0.2 ou checkpoints.

---

### 4.3 Checkpoints (estado consolidado)

📁 `docs/checkpoints/`

- `checkpoint-v0.1-grammar.md`  
  > Fechamento da gramática inicial

- `checkpoint-v0.2-*.md`  
  > Uso real, ajustes e consolidações da v0.2

> 📌 **Checkpoints são a fonte de verdade para retomada.**  
> Sem checkpoint, não há continuidade confiável.

---

## 5. Fluxo lógico da v0.2

1. Criar / revisar artefatos da v0.1 (PRD-Lite, Context Pack, etc.)
2. Criar **MCP+** para a iteração
3. Definir **Decision Locks**
4. Validar **Definition of Ready**
5. Executar a iteração (sem código)
6. Parar segundo **Definition of Stop**
7. Criar **Checkpoint**
8. Decidir conscientemente o próximo passo

---

## 6. Regras fundamentais da v0.2

- Nenhuma iteração relevante ocorre sem MCP+
- Decision Locks não são reabertos sem versionamento
- Conflitos entre artefatos obedecem precedência explícita
- Avançar sem DoR é violação do método
- Continuar sem objetivo claro é erro
- Sem checkpoint, não há retomada confiável

---

## 7. O que a v0.2 NÃO é

- não é execução de código
- não é CI/CD
- não é automação
- não é arquitetura de produto
- não é prompt engineering artesanal
- não substitui julgamento humano

---

## 8. Relação com versões futuras

A v0.2:

- é **estável e vigente**
- prepara conceitualmente o terreno para versões futuras
- **não autoriza** evolução normativa por si só

Qualquer evolução (ex.: v0.4) depende de:
- evidência multi-humano
- evidência multi-produto
- checkpoints explícitos

---

## 9. Como usar este documento

- Leia este arquivo como referência principal da versão vigente
- Consulte os playbooks para apoio operacional
- Use os templates como contratos explícitos
- Registre checkpoints sempre que houver avanço relevante
- Não pule etapas “porque a IA consegue”

---

## 10. Regra final

> **A IA pode acelerar o trabalho.  
> O método existe para impedir que ele descarrile.**

---
