# MCP+ — Academic Paper Builder / Feature 01

## Feature

Transformar uma ideia ou tema em uma estrutura inicial de paper acadêmico.

---

## Intenção

Reduzir o custo cognitivo inicial da escrita acadêmica,
apoiando a criação de uma estrutura clara, coerente e organizada.

---

## Entradas

- tema ou ideia central do paper
- área de conhecimento (opcional)
- tipo de artigo (ex.: teórico, empírico, revisão)
- público-alvo (opcional)

---

## Saídas Esperadas

- título provisório
- lista de seções principais
- breve descrição do objetivo de cada seção
- fluxo lógico entre seções
- escopo explicitado

---

## Decisões Bloqueadas (Decision Locks)

- IA **não escreve** o conteúdo completo
- IA **não avalia** qualidade científica
- Estrutura gerada é **proposta**, não decisão final
- Alterações estruturais exigem validação humana

---

## Definition of Ready

- problema claramente descrito
- escopo IN/OUT definido
- contexto de uso conhecido
- limites cognitivos explícitos

---

## Definition of Stop

- estrutura inicial completa entregue
- escopo explicitado
- não há nova informação relevante
- novas iterações seriam apenas variações cosméticas

---

## Riscos Conhecidos

- gerar estrutura genérica demais
- escopo excessivamente amplo
- usuário aceitar estrutura sem reflexão

Mitigação:
- explicitar suposições
- incentivar revisão humana
