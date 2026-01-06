> 📘 **Versão do Workflow**
>
> Este workflow está atualmente na versão **v0.2 (vigente)**.  
> A v0.2 introduz contratos explícitos, regras de precedência e memória operacional
> para reduzir loops, drift e decisões implícitas em interações com IA.
>
> 👉 Para detalhes completos da versão vigente, veja:  
> [`../README-v0.2.md`](../README-v0.2.md)
>
> ---
>
> 🧭 Nota sobre a v0.3
>
> A versão **v0.3** encontra-se **normativamente definida e encerrada**,
> com foco conceitual em governança da execução assistida por IA.
>
> A v0.3 **não é vigente**, **não substitui a v0.2** e **não autoriza execução ou automação**.
> Seu conteúdo está disponível em `docs/v0.3/` **exclusivamente para leitura e referência conceitual**,
> conforme registrado no checkpoint de encerramento normativo.
>
> ---

# AI-Assisted SDLC Workflow — Visão Operacional

Este diretório descreve a **visão operacional do AI-Assisted SDLC Workflow**, isto é,
**como o método é usado no dia a dia** para estruturar pensamento, decisões e planejamento
com apoio de IA.

O workflow **não é um pipeline de execução automática**.  
Ele é um **método de governança cognitiva**, no qual:

- humanos mantêm intenção, decisão e responsabilidade
- IA atua como agente executor **dentro de limites explícitos**
- decisões são registradas, congeladas e retomáveis

---

## Princípio Fundamental

> **IA auxilia e executa dentro de limites.  
> Humanos decidem, autorizam e encerram.**

A IA nunca opera sem:
- contexto explícito
- intenção clara
- limites definidos
- checkpoints humanos

---

## Visão Geral do Workflow (conceitual)

O AI-Assisted SDLC é **iterativo e orientado à intenção**, estruturado em torno de
artefatos versionáveis e contratos explícitos.

Fluxo conceitual típico (sem execução automática):

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
MCP / MCP+
   ↓
Trabalho assistido por IA + Revisão Humana
```

> ⚠️ Este diagrama não representa um pipeline técnico nem autoriza execução automática.

## Gramática do Método (Artefatos Canônicos)

O workflow possui uma gramática explícita, composta por templates canônicos.
Esses templates definem a forma dos artefatos, não sua execução.

📁 Localização: `docs/templates/`


### Artefatos da gramática

- **PRD-Lite:** Define problema, objetivo e escopo da iteração.

- **Feature Intent / Intent Spec:** Define a intenção exata da feature ou experimento.

- **Context Pack:** Consolida o contexto conceitual e operacional relevante.

- **Guidelines Técnicos:** Define regras técnicas, guardrails e proibições explícitas.

- **Visão de Arquitetura:** Define a arquitetura mínima e consciente da iteração.

- **MCP / MCP+:** Define o contrato cognitivo e operacional da iteração.

👉 Nenhum artefato relevante deve existir fora desses formatos.


## Exemplos Reais (Instâncias da Gramática)

Instâncias concretas vivem em: `docs/context/examples/`


**Esses arquivos:**

- não definem o método
- demonstram o método em uso
- servem como referência prática e didática

**Incluem:**

- exemplos bem-sucedidos
- anti-exemplos
- loops não interrompidos
- stop tardio

## Assistentes do Workflow (Agents)

Os assistentes são geradores especializados de artefatos,
sempre subordinados à governança humana.

📁 Localização: `docs/agents/`


**Características dos assistentes:**

- recebem inputs explícitos
- produzem apenas um tipo de artefato
- não tomam decisões fora do escopo
- não elevam autoridade normativa

## Papéis no Workflow
### 👤 Humano (Lead / Responsável)

**Responsável por:**

- definir intenção
- autorizar escopo
- validar artefatos
- criar Decision Locks
- encerrar iterações conscientemente


### 🤖 IA (Agente Assistido)

**Responsável por:**

- gerar conteúdo conforme contratos aprovados
- respeitar limites e guardrails
- sinalizar ambiguidades ou inconsistências
- interromper quando não houver autorização clara


## Governança e Segurança

**O workflow impõe:**

- checkpoints humanos obrigatórios
- precedência explícita entre artefatos
- versionamento consciente
- rastreabilidade entre decisão e trabalho assistido
- Nenhuma execução autônoma irreversível é permitida.

## Estrutura do Repositório (visão prática)

```
docs/
├── agents/        # Assistentes do workflow
├── templates/     # Gramática canônica
├── context/
│   └── examples/  # Casos reais e anti-exemplos
├── playbook/      # Guias operacionais (não normativos)
├── workflow/      # Visão operacional, roadmap e mapas
└── checkpoints/   # Memória institucional
```
## Estado Atual do Workflow

- **Versão vigente:** v0.2
- **Status:** estável para adoção interna controlada
- **Porta de entrada recomendada:** 👉 `docs/playbook/method-adoption-guide.md`

## Próximos Passos Possíveis (não automáticos)

- Usar o workflow com novos usuários (Nível Light)
- Observar falhas e fricções reais
- Registrar aprendizados em checkpoints
- Refinar playbooks (sem elevar autoridade)
- Somente depois: avaliar novas versões

---

> **Este workflow não é um framework de código. 
> É um método de decisão, governança e uso consciente de IA.**

