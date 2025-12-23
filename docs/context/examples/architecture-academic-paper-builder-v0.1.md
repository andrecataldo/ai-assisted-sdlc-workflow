# Visão de Arquitetura — Academic Paper Builder (v0.1)

Este documento descreve a **arquitetura mínima** do produto *Academic Paper Builder*
para a versão v0.1 (MVP CLI), derivada do Context Pack e das Guidelines Técnicos aprovados.

A arquitetura aqui descrita **não é definitiva**, mas suficiente para:
- orientar implementação
- reduzir ambiguidades técnicas
- permitir evolução incremental

---

## 1. Visão Geral da Arquitetura

O Academic Paper Builder é uma **aplicação CLI monolítica**, executada localmente,
sem dependências externas, projetada para rodar como um pacote Python.

A arquitetura segue os princípios:
- simplicidade
- baixo acoplamento
- clareza de responsabilidades
- fácil testabilidade

---

## 2. Estilo Arquitetural

- Estilo: **Monólito simples (CLI)**
- Padrão de organização: **Camadas leves**
- Comunicação externa: **Nenhuma**
- Persistência: **Nenhuma**

Não há uso de:
- arquitetura distribuída
- microserviços
- mensageria
- APIs externas

---

## 3. Componentes Principais

### 3.1 CLI Entry Point

Responsável por:
- inicializar a aplicação
- delegar execução para o parser de argumentos

Arquivo: 
`src/apb/main.py`


---

### 3.2 Argument Parser

Responsável por:
- definir argumentos da CLI
- validar presença e formato básico dos inputs
- exibir mensagens de erro claras

Arquivo:
`src/apb/cli.py`


---

### 3.3 Validação de Domínio

Responsável por:
- validar regras de negócio simples (limites, obrigatoriedade)
- garantir consistência antes da execução

Implementação:
- funções puras
- sem efeitos colaterais

---

### 3.4 Output Formatter

Responsável por:
- organizar e exibir o resumo da execução
- não persistir dados
- não gerar arquivos

Formato de saída:
- texto simples (stdout)

---

## 4. Fluxo de Execução

Fluxo lógico da aplicação:

1. Usuário executa `python -m apb`
2. CLI recebe argumentos
3. Parser valida formato básico
4. Validações de domínio são aplicadas
5. Resumo é exibido no stdout
6. Processo encerra com exit code adequado

---

## 5. Gestão de Erros

- Erros são tratados de forma explícita
- Em caso de erro:
  - mensagem clara no stdout ou stderr
  - exit code ≠ 0
- Não há retries
- Não há fallback automático

---

## 6. Testabilidade

A arquitetura foi pensada para facilitar testes:

- Lógica de validação isolada
- CLI testável via `pytest`
- Sem dependências externas
- Sem mocks complexos

---

## 7. Segurança

- Nenhum dado sensível é tratado
- Nenhuma entrada é persistida
- Nenhuma execução remota ocorre

Riscos de segurança são considerados mínimos nesta versão.

---

## 8. Limitações Arquiteturais Conhecidas

As seguintes limitações são **aceitas conscientemente** nesta versão:

- Ausência de persistência
- Ausência de plugins
- Ausência de extensibilidade formal
- Acoplamento direto CLI → lógica

Essas limitações podem ser revistas em versões futuras.

---

## 9. Evoluções Arquiteturais Futuras (não implementar agora)

Possíveis evoluções reconhecidas, mas fora do escopo atual:

- Camada de domínio mais explícita
- Geração de artefatos (Markdown / LaTeX)
- Integração com gerenciadores de referência
- Suporte a templates configuráveis
- Modularização mais profunda

---

## Estado do Documento

- **Produto:** Academic Paper Builder  
- **Versão:** v0.1  
- **Derivado de:**  
  - Context Pack — Academic Paper Builder (v0.1)  
  - Guidelines Técnicos — Academic Paper Builder (v0.1)  
- **Gerado por:** Architecture Generator v0.1
