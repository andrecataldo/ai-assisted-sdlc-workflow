# 🔖 CHECKPOINT — Consolidação Geral (Axioma + v0.2 aplicada + v0.3 encerrada)

<!-- CHECKPOINT OFICIAL -->

Projeto: ai-assisted-sdlc-workflow  
Produto de referência: Academic Paper Builder  
Data: 2025-12-29  
Responsável humano: Andre Cataldo  
Objetivo do checkpoint: Consolidar o estado atual do workflow, permitindo retomada segura em outro contexto ou chat.

---

## 1. Estado Geral do Workflow

O AI-Assisted SDLC Workflow encontra-se no seguinte estado consolidado:

- **Diretriz Primária** definida (Camada 0)
- **v0.2** vigente e aplicada em produto real
- **v0.3** normativamente definida e encerrada
- Separação clara entre:
  - norma
  - exemplos
  - agentes
  - playbooks
  - guias de leitura

Este checkpoint marca um **ponto estável e auditável** do método.

---

## 2. Diretriz Primária (Camada 0)

A Diretriz Primária governa todo o workflow, acima de versões.

### Axioma Central (imutável)

> **IA acelera pensamento e execução, mas nunca substitui responsabilidade humana.**

### Axiomas Derivados

1. **Governança precede velocidade**  
   Velocidade sem governança transfere risco; governança habilita velocidade sustentável.

2. **Norma precede automação**  
   Nenhuma automação é válida sem norma explícita que a governe.

3. **Decisão só existe quando é explícita**  
   Decisões só existem quando são explicitadas, registradas e bloqueadas.

4. **Evolução exige evidência**  
   O workflow só evolui com base em evidência empírica, nunca por hipótese ou entusiasmo.

---

## 3. v0.2 — Versão Vigente (Aplicada)

A **v0.2** é a versão vigente do workflow.

Características principais:
- contratos explícitos
- regras de precedência entre artefatos
- MCP+ como contrato forte
- Decision Locks
- Definition of Ready / Definition of Stop
- Checkpoints obrigatórios

### Aplicação real registrada

Produto: **Academic Paper Builder**

Artefatos criados (uso real, sem execução):
- PRD-Lite (v0.2)
- Context Pack (v0.2)
- MCP+ (v0.2)
- Checkpoint de uso da v0.2

Resultado:
- v0.2 validada como adequada para organizar pensamento e reduzir drift
- limites cognitivos respeitados
- base concreta criada para Dry Run v0.3

---

## 4. v0.3 — Norma Encerrada (não vigente)

A **v0.3** encontra-se **normativamente definida e encerrada**, mas **não é vigente**.

Objetivo da v0.3:
- governar execução assistida por IA
- definir modos de execução
- estabelecer guards, contrato de qualidade, observabilidade e rollback

Estado atual:
- capítulos normativos completos (`docs/v0.3/`)
- índice normativo definido (`INDEX.md`)
- encerramento formal registrado em checkpoint
- guia oficial de leitura criado (`docs/v0.3/README.md`)
- documento conceitual separado (`README-v0.3-draft.md`)

A v0.3 **não define automação nem CI/CD**.

---

## 5. Exemplos e Agentes

- `/docs/context/examples` contém exemplos:
  - v0.1 → exploratórios (ensinam o método)
  - v0.2 → aplicações reais (aplicam o método)

- `/docs/agents` contém artefatos operacionais:
  - não normativos
  - subordinados à Diretriz Primária e à v0.2
  - com README de governança e headers de status

---

## 6. Hierarquia de Autoridade Consolidada

1. **Diretriz Primária**
2. **Checkpoints**
3. **Versão vigente (v0.2)**
4. **Versões normativas encerradas (v0.3)**
5. **Playbooks e Templates**
6. **Agents e Exemplos**

Itens de nível inferior **não podem contradizer** níveis superiores.

---

## 7. Próximo Passo Autorizado

Com base neste checkpoint, os próximos passos válidos são:

- Rodar **Dry Run da v0.3** sobre o Academic Paper Builder
- Criar indicadores simples (ex.: “Estamos em loop?”)
- Derivar playbooks e MCP+ light **após evidência**
- Planejar v0.4 **somente após uso real documentado**

---

## 🏷️ TAG DE RETOMADA

RETOMADA:  
Workflow consolidado com Diretriz Primária definida, v0.2 aplicada em produto real e v0.3 normativamente encerrada.
