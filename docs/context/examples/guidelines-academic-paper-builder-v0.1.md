# Guidelines Técnicos — Academic Paper Builder (v0.1)

Este documento define **regras técnicas obrigatórias** para o desenvolvimento do
**Academic Paper Builder**, derivadas do Context Pack e da Feature Intent aprovados.

Estas guidelines funcionam como **guardrails técnicos** para agentes de IA e humanos,
evitando extrapolação de escopo, overengineering ou decisões implícitas.

---

## 1. Linguagem e Runtime

- Linguagem principal: **Python**
- Versão mínima: **Python 3.11**
- Ambiente alvo: **Linux / Ubuntu**
- Interface: **CLI (linha de comando)**

---

## 2. Estrutura do Projeto

- Layout obrigatório: **src layout**

Estrutura base esperada:

```text
academic-paper-builder/
├── pyproject.toml
├── src/
│   └── apb/
│       ├── __init__.py
│       ├── __main__.py
│       └── cli.py
└── tests/

Forma de execução obrigatória:
```text
python -m apb

## 3. Dependências

### Permitidas

- Biblioteca padrão do Python
- `pytest` (exclusivamente para testes)

### Proibidas

- Frameworks web (FastAPI, Flask, Django)
- Bancos de dados
- Serviços cloud
- SDKs externos de IA
- Dependências pesadas ou não essenciais

---

## 4. Interface de Linha de Comando (CLI)

### Requisitos obrigatórios

- Uso de `argparse`
- Argumentos explícitos e documentados
- Em caso de erro:
  - Mensagem clara ao usuário
  - Exit code diferente de zero

### Parâmetros esperados

- `--title` (obrigatório)
- `--topic` (obrigatório, repetível)
- `--guidelines` (opcional)

---

## 5. Validações

### Parâmetro `--title`

- String não vazia
- Trim automático
- Máximo de 200 caracteres

### Parâmetro `--topic`

- Mínimo de 1 item
- Máximo de 20 itens
- Cada item deve ser não vazio após trim

### Em caso de erro

- Execução deve falhar explicitamente
- Nenhuma saída parcial deve ser gerada

---

## 6. Comportamento Permitido da IA

### A IA pode

- Validar inputs
- Organizar dados fornecidos pelo usuário
- Exibir resumos estruturais

### A IA não pode

- Gerar conteúdo acadêmico
- Criar arquivos Markdown do paper
- Inventar referências bibliográficas
- Avaliar qualidade científica
- Tomar decisões de escopo não explicitadas

---

## 7. Testes

- Framework: **pytest**

### Testes mínimos obrigatórios

- Falha sem `--title`
- Falha sem `--topic`
- Falha com título vazio
- Falha com tópico vazio
- Falha com mais de 20 tópicos
- Sucesso com inputs válidos

---

## 8. Qualidade e Manutenibilidade

- Código simples e legível
- Clareza é mais importante que abstração
- Funções pequenas e diretas
- Erros explícitos são preferíveis a falhas silenciosas

---

## 9. Evoluções Futuras (não implementar agora)

Os itens abaixo **não fazem parte desta iteração**, mas são reconhecidos como possíveis evoluções:

- Escrita automática do conteúdo
- Integração com Zotero ou similares
- Exportação para Markdown ou LaTeX
- Templates por tipo de paper
- Validação por normas acadêmicas

---

## Estado do Documento

- **Produto:** Academic Paper Builder  
- **Versão:** v0.1  
- **Derivado de:** Context Pack — Academic Paper Builder (v0.1)  
- **Gerado por:** Tech Guidelines Generator v0.1  
