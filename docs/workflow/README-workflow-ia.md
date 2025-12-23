# AI-Assisted SDLC Workflow (v0.1)

Este repositório define um **workflow estruturado para desenvolvimento de software com apoio de IA**, no qual agentes atuam como **executores**, enquanto humanos mantêm **intenção, governança e responsabilidade final**.

O objetivo do workflow é permitir a criação de **produtos, features e experimentos reais**, com:

- clareza de contexto
- controle de escopo
- rastreabilidade de decisões
- execução segura por agentes de IA

---

## Princípio Fundamental

> **IA executa. Humanos decidem.**

A IA nunca opera sem:

- contexto explícito
- regras claras
- limites bem definidos
- checkpoints humanos

---

## Visão Geral do Workflow

O AI-Assisted SDLC é **iterativo e orientado à intenção**, estruturado em torno de artefatos versionáveis e assistentes especializados.

Fluxo conceitual:

```text
PRD-Lite
   ↓
Context Pack
   ↓
Guidelines Técnicos
   ↓
Visão de Arquitetura
   ↓
Action Plan
   ↓
MCP (Machine-Consumable Plan)
   ↓
Execução por IA + Revisão Humana
```


---

## Gramática do Método (Artefatos Canônicos)

O workflow possui uma **gramática explícita**, composta por **templates canônicos**.  
Esses templates definem **a forma obrigatória** dos artefatos, independentemente do produto.

### 📐 Templates Oficiais

Localizados em: `docs/templates/`


Artefatos da gramática:

- **PRD-Lite**  
  Define o problema, objetivos e escopo da iteração.

- **Feature Intent / Intent Spec**  
  Define a intenção exata da feature a ser construída.

- **Context Pack**  
  Consolida o contexto conceitual e operacional do produto.

- **Guidelines Técnicos**  
  Define regras técnicas, guardrails e proibições explícitas.

- **Visão de Arquitetura**  
  Define a arquitetura mínima e consciente para a iteração.

- **MCP (Machine-Consumable Plan)**  
  Define o contrato operacional para execução por agentes de IA.

👉 **Nenhum artefato pode ser criado fora desses formatos.**

---

## Exemplos Reais (Instâncias da Gramática)

Instâncias concretas de produtos e features vivem em: `docs/context/examples/`


Esses arquivos:
- **não definem o método**
- **demonstram o método em uso**
- servem como referência prática

Exemplo:
- *Academic Paper Builder* (case real completo, end-to-end)

---

## Assistentes do Workflow

Os assistentes são **geradores especializados**, responsáveis por produzir artefatos **a partir de templates e inputs aprovados**.

Localização: `docs/agents/`


Assistentes definidos no v0.1:

- **Context Generator**
- **Tech Guidelines Generator**
- **Architecture Generator**
- **Action Plan Generator**
- **MCP Generator**

Cada assistente:
- recebe inputs explícitos
- gera apenas um tipo de artefato
- não toma decisões fora do escopo

---

## Papéis no Workflow

### Human Lead Engineer

Responsável por:
- definir intenção
- aprovar artefatos
- revisar resultados
- assumir responsabilidade técnica final

---

### AI Dev Agent

Responsável por:
- executar planos aprovados
- respeitar escopo e guardrails
- interromper execução em caso de dúvida
- reportar erros explicitamente

---

## Governança e Segurança

O workflow impõe:

- checkpoints humanos obrigatórios
- escopo autorizado vs. proibido
- versionamento de todos os artefatos
- rastreabilidade completa entre decisões e execução

Nenhuma execução autônoma irreversível é permitida.

---

## Estrutura do Repositório

```text
docs/
├── agents/ # Assistentes do workflow
├── templates/ # Gramática canônica do método
├── context/
│ ├── examples/ # Casos reais (instâncias)
│ └── *.md # Templates de contexto
├── workflow/ # Roadmap, README e visão do processo
└── playbook/ # Cheatsheets e guias rápidos
```

---

## Estado do Workflow

- **Versão:** v0.1
- **Status:** Gramática completa e validada
- **Uso recomendado:**  
  - criação de novos produtos
  - experimentos com agentes
  - ensino e replicação do método

---

## Próximos Passos Possíveis

- Evoluir para v0.2 (métricas, feedback loops)
- Criar templates de CI/QA
- Automatizar geração de MCP
- Aplicar o workflow a novos produtos

---

> **Este workflow não é um framework de código.  
> É um método de decisão, execução e governança com IA.**


