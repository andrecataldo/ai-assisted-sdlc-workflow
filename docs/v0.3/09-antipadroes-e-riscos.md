# 9️⃣ Anti-padrões e Riscos Conhecidos

> **Status:** Normativo (preventivo)  
> **Versão do workflow:** v0.3  
> **Dependência:**  
> - Capítulo 2 — Princípios Normativos da Execução Assistida  
> - Capítulo 3 — Modos de Execução  
> - Capítulo 4 — Autorização e Guards de Execução  
> - Capítulo 5 — Contrato de Qualidade para Execução  
> - Capítulo 6 — Autoridade, Responsabilidade e Limites da IA  
> - Capítulo 7 — Observabilidade Cognitiva e Rastreabilidade  
> - Capítulo 8 — Rollback, Invalidação e Recovery Cognitivo  
> **Autoridade:** Define comportamentos proibidos e riscos sistêmicos conhecidos da execução assistida por IA

---

## 9.1 Propósito deste Capítulo

Este capítulo documenta **anti-padrões explícitos e riscos conhecidos** associados ao uso da execução assistida por IA no AI-Assisted SDLC Workflow.

Seu objetivo é:
- prevenir usos indevidos do método
- evitar distorções por pressão organizacional ou entusiasmo técnico
- tornar explícito o que **não deve ser feito**, mesmo quando tecnicamente possível

Anti-padrões não são falhas acidentais.  
São **desvios previsíveis que precisam ser bloqueados por norma**.

---

## 9.2 Anti-padrão: Execução Implícita

### Descrição
Iniciar execução sem declaração explícita de modo, autorização ou contrato de qualidade.

### Por que é proibido
- elimina governança
- cria risco sistêmico invisível
- impede auditoria posterior

Qualquer execução implícita é considerada **execução inválida**.

---

## 9.3 Anti-padrão: Escalada Silenciosa de Modo

### Descrição
Tratar Dry Run como “quase Hot Run” ou permitir que a execução escale gradualmente sem nova autorização.

### Por que é proibido
- contorna guards
- mascara aumento de risco
- transfere responsabilidade sem consentimento

Mudança de modo **sempre exige reavaliação e autorização explícita**.

---

## 9.4 Anti-padrão: Autorização Genérica ou Permanente

### Descrição
Autorizações amplas, vagas ou sem validade temporal definida.

### Por que é proibido
- ignora contexto
- cria execução por inércia
- dilui responsabilidade

Autorizações devem ser **específicas, contextuais e temporais**.

---

## 9.5 Anti-padrão: Qualidade Assumida por Otimismo

### Descrição
Executar com base em confiança subjetiva, histórico de acerto da IA ou urgência percebida.

### Por que é proibido
- substitui contrato por fé
- normaliza risco não assumido
- incentiva execução prematura

Qualidade deve ser **explicitamente avaliada e aceita**, nunca presumida.

---

## 9.6 Anti-padrão: Delegação Implícita de Autoridade à IA

### Descrição
Permitir que a IA:
- decida quando executar
- aceite riscos
- relativize limites
- imponha bloqueios

### Por que é proibido
- rompe soberania humana
- cria ambiguidade de responsabilidade
- antropomorfiza a IA operacionalmente

A IA **não decide**, mesmo quando executa.

---

## 9.7 Anti-padrão: Execução Opaca

### Descrição
Executar sem garantir observabilidade cognitiva suficiente.

### Por que é proibido
- impede aprendizado
- inviabiliza auditoria
- oculta erro sistêmico

Execução sem explicabilidade posterior é considerada **falha de governança**.

---

## 9.8 Anti-padrão: Rollback Silencioso ou Informal

### Descrição
Desfazer execução ou decisão sem invalidação explícita e registro consciente.

### Por que é proibido
- apaga aprendizado
- oculta responsabilidade
- cria histórico falso de sucesso

Rollback deve ser **explícito, registrado e rastreável**.

---

## 9.9 Risco Conhecido: Uso Político do Workflow

### Descrição
Uso do workflow para:
- legitimar decisões já tomadas
- transferir responsabilidade
- criar aparência de controle sem governança real

### Mitigação
- reforço dos princípios normativos
- exigência de rastreabilidade
- checkpoints como fonte de verdade

---

## 9.10 Risco Conhecido: Burocratização Excessiva

### Descrição
Transformar normas em barreiras artificiais que inviabilizam o uso prático.

### Mitigação
- proporcionalidade ao risco
- revisão consciente de playbooks
- foco em governança, não em papelada

---

## 9.11 Risco Conhecido: Automatização Prematura

### Descrição
Converter normas diretamente em automação sem validação empírica suficiente.

### Mitigação
- separação entre norma e mecanismo
- evolução incremental
- uso de Dry Run como etapa intermediária

---

## 9.12 Violação de Anti-padrões e Riscos

A ocorrência de qualquer anti-padrão descrito neste capítulo caracteriza:

- uso indevido do workflow
- falha de governança
- risco sistêmico não autorizado

Resultados positivos **não legitimam** a adoção de anti-padrões.

---

## 9.13 Encerramento do Capítulo

Este capítulo existe para lembrar que:

- nem tudo que é possível é aceitável
- governança falha tende a se repetir
- riscos conhecidos ignorados voltam como incidentes

> **Se o método pode ser usado contra seus próprios princípios,  
> ele precisa declarar isso explicitamente.**
