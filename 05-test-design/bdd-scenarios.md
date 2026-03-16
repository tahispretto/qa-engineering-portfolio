## Cenários utilizando BDD

BDD (Behavior Driven Development) ajuda a descrever o comportamento esperado do sistema utilizando uma linguagem próxima do negócio, facilitando a comunicação entre QA, desenvolvedores e stakeholders, além de permitir integração com automação usando ferramentas como **Cucumber**.

## Estrutura GHERKIN para BDD

Os cenários BDD são escritos utilizando a linguagem **GHERKIN**. A estrutura básica é:

```gherkin
Given (Dado)   – Estado inicial ou pré-condição
When (Quando)  – Ação realizada pelo usuário
Then (Então)   – Resultado esperado
And (E)        – Passo adicional
But (Mas)      – Exceção ou restrição
Examples       – Parâmetros para criar variações de cenário
```

## Exemplo de cenários BDD
Opção 1: Cenários separados

```gherkin
Feature: Login no sistema

Scenario: Login com credenciais válidas
Given que o usuário está na página de login
When ele informa usuário e senha válidos
And clica no botão entrar
Then o sistema deve permitir o acesso ao sistema

Scenario: Login com senha inválida
Given que o usuário está na página de login
When ele informa um usuário válido
And informa uma senha incorreta
And clica no botão entrar
Then o sistema deve exibir uma mensagem de erro

Scenario: Tentativa de login com campos vazios
Given que o usuário está na página de login
When ele tenta acessar o sistema sem preencher os campos
Then o sistema deve exibir mensagens de validação
```

Opção 2: Scenario Outline com Examples

```gherkin
Feature: Login no sistema

Scenario Outline: Validação do login com diferentes combinações de usuário e senha
Given que o usuário está na página de login
When ele informa "<usuario>" e "<senha>"
And clica no botão entrar
Then o sistema deve "<resultado>"

Examples:
| usuario         | senha          | resultado                        |
| usuario_valido  | senha_valida   | permitir o acesso ao sistema     |
| usuario_valido  | senha_invalida | exibir uma mensagem de erro      |
| vazio           | vazio          | exibir mensagens de validação    |
```