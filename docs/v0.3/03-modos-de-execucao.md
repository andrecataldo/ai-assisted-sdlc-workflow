# 3️⃣ Modos de Execução (Execution Modes)

> **Status:** Normativo  
> **Versão do workflow:** v0.3  
> **Dependência:** Capítulo 2 — Princípios Normativos da Execução Assistida  
> **Autoridade:** Define os modos válidos de execução e suas fronteiras de risco

---

## 3.1 Propósito deste Capítulo

Este capítulo define os **modos de execução reconhecidos e permitidos** na v0.3 do AI-Assisted SDLC Workflow.

Os modos de execução:
- **classificam o nível de risco**
- **explicitam responsabilidades**
- **impedem execução ambígua ou implícita**

Qualquer execução assistida por IA **deve** operar sob **um e apenas um modo explícito**.

---

## 3.2 Princípio da Exclusividade de Modo

Toda interação assistida por IA relacionada à execução deve declarar **explicitamente** seu modo de execução.

- Modos **não podem** ser inferidos
- Modos **não podem** ser combinados
- Modos **não podem** mudar implicitamente ao longo de uma interação

A ausência de declaração explícita de modo implica **No Run** por padrão.

---

## 3.3 Modo No Run

### Definição

**No Run** é o modo padrão e seguro do workflow.

Neste modo:
- não há execução real
- não há alteração de sistemas, código ou estado
- toda atividade é restrita a definição, análise, decisão ou simulação conceitual

### Uso permitido

- elaboração de artefatos
- análise de opções
- discussão de alternativas
- simulações cognitivas ou textuais

### Restrições

Qualquer ação que produza efeitos externos ou persistentes é **proibida** neste modo.

---

## 3.4 Modo Dry Run

### Definição

**Dry Run** é o modo de **simulação executável**, sem efeitos aplicados.

Neste modo:
- a IA pode gerar outputs executáveis
- nenhuma alteração é aplicada
- o objetivo é validar entendimento, forma e impacto potencial

### Intenção normativa

O Dry Run existe para:
- reduzir incerteza
- antecipar riscos
- validar contratos antes da ação

### Limites

- Dry Run **não autoriza** aplicação posterior automática
- Outputs de Dry Run **não têm efeito vinculante**
- A transição para Hot Run exige nova autorização explícita

---

## 3.5 Modo Hot Run

### Definição

**Hot Run** é o modo de execução real e efetiva.

Neste modo:
- ações geram efeitos externos ou persistentes
- há impacto direto em sistemas, código ou dados
- o risco é considerado **aceito conscientemente**

### Natureza excepcional

Hot Run é **excepcional por definição**.

Ele só pode ser considerado quando:
- os modos No Run e Dry Run são insuficientes
- os riscos são conhecidos
- a autorização é explícita e registrada

### Responsabilidade

Toda execução em Hot Run implica:
- responsabilidade humana explícita
- rastreabilidade obrigatória
- possibilidade de rollback conforme definido em capítulos posteriores

---

## 3.6 Proibição de Execução Implícita

É explicitamente proibido:
- iniciar Hot Run a partir de Dry Run sem autorização
- tratar Dry Run como “quase execução”
- permitir que ferramentas ou automações decidam o modo

Qualquer execução não claramente enquadrada em um modo é considerada **execução inválida**.

---

## 3.7 Transições entre Modos

A transição entre modos:
- **não é automática**
- **não é implícita**
- **não é progressiva por padrão**

Cada transição exige:
- reavaliação consciente
- nova autorização, quando aplicável
- registro explícito do modo vigente

---

## 3.8 Precedência do Modo Mais Restritivo

Na presença de ambiguidade, conflito ou dúvida:
- o modo **mais restritivo** prevalece
- No Run tem precedência sobre Dry Run
- Dry Run tem precedência sobre Hot Run

Este princípio protege o workflow contra escalada inadvertida de risco.

---

## 3.9 Relação com Autorização e Guards

Os modos de execução **não autorizam execução por si só**.

Eles:
- classificam o tipo de execução
- definem o nível de risco
- condicionam os guards necessários

A autorização e os guards são tratados no **Capítulo 4**.

---

## 3.10 Violação de Modo

Qualquer violação das regras de modo caracteriza:
- falha de governança
- uso indevido do workflow
- risco sistêmico

Violações **não podem** ser justificadas por:
- sucesso técnico
- urgência
- limitações de ferramenta
- pressão organizacional

---

## 3.11 Encerramento do Capítulo

Os modos de execução existem para **proteger o sistema**, não para acelerar resultados.

> **Se o modo não está claro,  
> a execução está proibida.**
