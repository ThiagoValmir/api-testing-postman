# API Testing with Postman

Projeto desenvolvido para praticar e demonstrar conhecimentos em **testes de APIs REST utilizando Postman**.

Durante o desenvolvimento deste projeto, foram realizados testes em diferentes APIs e cenários, explorando desde requisições básicas até a utilização de variáveis, scripts e validações automatizadas.

O objetivo é consolidar conhecimentos em **API Testing** e demonstrar, na prática, conceitos importantes utilizados na rotina de um profissional de QA.

---

## Sobre o projeto

Neste projeto foram criados e executados diferentes cenários de testes utilizando o Postman.

Além da execução manual das requisições, foram utilizados recursos do Postman para automatizar validações e facilitar o encadeamento entre diferentes requisições.

### Principais conhecimentos praticados

- Testes de APIs REST
- Métodos HTTP
- Status Codes
- Request e Response
- Headers
- Body
- Query Parameters
- Path Parameters
- Variáveis
- Environment Variables
- Collection Variables
- Pre-request Scripts
- Post-response Scripts
- Test Scripts
- Assertions
- Autenticação
- Tokens
- Encadeamento de requisições
- Cenários positivos e negativos
- Validação de respostas da API

---

## Ferramentas utilizadas

- **Postman**
- **JavaScript** para scripts e validações
- **Git / GitHub** para versionamento e documentação

---

## Estrutura dos testes

Os testes foram organizados em diferentes collections e cenários para praticar funcionalidades específicas do Postman.

### Sign Up

Cenários relacionados ao cadastro de usuários.

- Cadastro com dados válidos
- Cadastro utilizando variáveis
- Cadastro com e-mail já existente
- Cadastro com username já existente
- Validação do status code
- Validação do response body
- Validação das mensagens retornadas pela API

### Sign In

Cenários relacionados à autenticação de usuários.

- Login com credenciais válidas
- Login com e-mail inexistente
- Login com credenciais inválidas
- Validação do status code
- Validação do token retornado
- Utilização do token em requisições posteriores

### Users

Cenários relacionados ao gerenciamento de usuários.

- Atualização de usuário
- Follow de usuário
- Unfollow de usuário
- Validação das respostas da API

### Articles

Cenários relacionados à criação e gerenciamento de artigos.

- Criação de artigo
- Criação utilizando autenticação
- Validação dos dados enviados
- Validação da resposta
- Exclusão de artigo
- Validação do status code

### Comments

Cenários relacionados a comentários.

- Criação de comentário
- Validação da resposta
- Exclusão de comentário
- Validação do status code

---

# Variáveis

Durante os testes foram utilizadas variáveis do Postman para evitar a necessidade de inserir os mesmos valores manualmente em diferentes requisições.

### Exemplos de utilização

- URL base da API (BASE_URL)
- E-mail (emailConduit)
- Senha (passwordConduit)
- Username (username)
- Token (tokenConduit)
- IDs de artigos (slugConduit)
- IDs de comentários (commentId) 

As variáveis também foram utilizadas para criar um fluxo entre diferentes requisições.

Por exemplo:

```text
Login
   ↓
Recebe token
   ↓
Armazena token em uma variável
   ↓
Utiliza token em outra requisição
   ↓
Cria artigo autenticado
