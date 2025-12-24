# 📘 Checkpoint Strategy — Playbook (v0.2)

## 1. O papel dos checkpoints no workflow

Checkpoints são a **memória operacional formal** do AI-Assisted SDLC Workflow.

Eles existem para:
- preservar decisões humanas ao longo do tempo
- permitir retomada exata em novos chats/sessões
- evitar reinterpretação ou perda de contexto
- tornar o método auditável e reprodutível

> 📌 Checkpoint não é documentação histórica.  
> É **estado consolidado**.

---

## 2. Tipos oficiais de checkpoint

### 2.1 Checkpoint de Gramática
Criado quando:
- uma versão do workflow é estabilizada
- templates/playbooks são consolidados

Exemplo:
- `checkpoint-v0.1-grammar.md`
- `checkpoint-v0.2-contracts-and-memory.md`

---

### 2.2 Checkpoint de Iteração
Criado quando:
- uma iteração relevante termina
- um MCP+ deixa de ser válido
- um conjunto de decisões é fechado

---

### 2.3 Checkpoint de Decisão Crítica
Criado quando:
- decisões estruturais são tomadas
- há alto custo de reversão
- múltiplos artefatos são impactados

---

### 2.4 Checkpoint de Experimento
Criado quando:
- um experimento (ex.: hot run futuro) é encerrado
- aprendizados precisam ser consolidados

---

## 3. Quando criar um checkpoint (regras claras)

Um checkpoint **deve ser criado** quando:

- um MCP+ é encerrado
- critérios de parada (DoS) são atingidos
- decisões bloqueadas mudam de versão
- há troca de contexto (tempo, pessoa, chat, agente)
- antes de iniciar execução de código
- antes de mudar de fase do workflow

---

## 4. Quando NÃO criar um checkpoint

Não criar checkpoint para:
- ajustes triviais de texto
- correções locais sem impacto
- brainstorming exploratório inicial

Checkpoint demais gera ruído.  
Checkpoint de menos gera amnésia.

---

## 5. Relação com MCP+ e Decision Locks

- MCP+ governa a **iteração**
- Decision Locks congelam **decisões**
- Checkpoints congelam **o estado completo**

📌 Checkpoint é sempre **posterior** ao MCP+.

---

## 6. Regras de ouro

- sempre versionar checkpoints
- nunca sobrescrever checkpoints antigos
- tratar checkpoint como fonte de verdade
- usar checkpoints para retomada — não memória informal

---

## 7. Regra final

> **Sem checkpoint, não há continuidade confiável.**
