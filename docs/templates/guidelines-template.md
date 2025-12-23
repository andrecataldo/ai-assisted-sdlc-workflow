# Guidelines Técnicos — <Nome do Produto> (v<versão>)

Este documento define as **regras técnicas obrigatórias** para o desenvolvimento do
produto **<Nome do Produto>**, no contexto do **AI-Assisted SDLC Workflow**.

As guidelines funcionam como **guardrails técnicos**, garantindo consistência,
governança e controle de escopo durante a execução por agentes de IA e humanos.

---

## 1. Linguagem e Runtime

- Linguagem principal: <definir>
- Versão mínima: <definir>
- Ambiente alvo: <definir>
- Tipo de aplicação: <CLI | serviço | biblioteca | outro>

---

## 2. Estrutura do Projeto

- Layout do projeto: <definir>

Estrutura base esperada:

```text
<estrutura-base-do-projeto>
```
Forma de execução principal:

```text
<comando-principal>
```
## 3. Dependências

### Permitidas

- <listar dependências permitidas>
- <biblioteca padrão, se aplicável>

### Proibidas

- <listar explicitamente o que não pode ser usado>
- <frameworks, serviços, integrações não autorizadas>

---

## 4. Interface (CLI / API / UI)

### Requisitos obrigatórios

- <regras de entrada>
- <regras de validação>
- <comportamento esperado em erro>

### Parâmetros / Inputs esperados

- <parâmetro 1> — <obrigatório | opcional>
- <parâmetro 2> — <descrição>

---

## 5. Validações

### Regras obrigatórias

- <regra 1>
- <regra 2>

### Em caso de erro

- <comportamento esperado>
- <exit code / retorno esperado>

---

## 6. Comportamento Permitido da IA

### A IA pode

- <ações explicitamente permitidas>
- <ações de apoio>

### A IA não pode

- <ações proibidas>
- <decisões que exigem aprovação humana>

---

## 7. Testes

- Framework de testes: <definir>

### Testes mínimos obrigatórios

- <cenário de falha>
- <cenário de sucesso>
- <cenário limite>

---

## 8. Qualidade e Manutenibilidade

- <princípios de código>
- <restrições de complexidade>
- <boas práticas esperadas>

---

## 9. Evoluções Futuras (não implementar agora)

Os itens abaixo **não fazem parte desta iteração**, mas são reconhecidos como possíveis
evoluções futuras do produto:

- <evolução futura 1>
- <evolução futura 2>

---

## Estado do Documento

- **Tipo:** Template de Guidelines Técnicos  
- **Workflow:** AI-Assisted SDLC  
- **Versão:** v0.1  
- **Uso:** Deve ser copiado e preenchido para cada produto ou feature
