# Desafio Técnico - Desenvolvedor(a) Frontend React

## Objetivo

Desenvolver uma aplicação **Frontend** utilizando **React**, com um fluxo de autenticação simples e uma interface para cadastro e gerenciamento de vagas de emprego.

---

## Funcionalidades Requeridas

### 1. Tela de Login
- Campos obrigatórios:
  - **E-mail**
  - **Senha**
- Regras:
  - Após o login bem-sucedido, o usuário deve receber um **token**.
  - O **token** deve ser armazenado no `localStorage ou sessão` (ou outro método de sua escolha).
  - O usuário deve ser redirecionado para a tela de **listagem de vagas**.
  - Deve haver a opção de **logout**, que apague o token e redirecione para o login.
  - Todas as rotas do CRUD, estão protegidas, sendo necessário mandar o JWT Bearer no Header
---

### 2. Tela de Cadastro de Vagas
- Criar um formulário com os seguintes campos:

| Campo     | Tipo     | Descrição                                          |
|-----------|----------|----------------------------------------------------|
| `role`    | string   | Cargo ou função da vaga                            |
| `company` | string   | Nome da empresa                                    |
| `location`| string   | Localização da vaga                                |
| `remote`  | boolean  | Indicar se a vaga é remota (`true` ou `false`)     |
| `link`    | string   | Link para candidatura ou mais informações          |
| `salary`  | int64    | Salário oferecido (apresentado no formato monetário)|

---

### 3. Funcionalidades CRUD
- **Criar vaga**: Através do formulário de cadastro.
- **Listar vagas**: Listagem de todas as vagas cadastradas.
- **Visualizar vaga (Show)**: Exibir detalhes completos ao selecionar uma vaga.
- **Editar vaga**: Permitir atualização dos campos de uma vaga.
- **Excluir vaga**: Remover uma vaga da listagem.

---

### 4. Controle de Sessão
- Todas as operações de CRUD devem estar protegidas.
- O usuário **deve estar autenticado** para acessar as telas protegidas.
- Caso não haja um token válido, o usuário deve ser redirecionado automaticamente para a tela de **login**.

---

## Diferenciais (Extras)
Os itens abaixo **não são obrigatórios**, mas serão considerados diferenciais:

- Utilização de **TypeScript**.
- Dockerização da aplicação.
- Boas práticas de organização de código e estrutura de pastas.
- Responsividade e uma boa interface de usuário (UX/UI).

---

## Requisitos Técnicos
- **React** (pode usar Vite ou Create React App).
- **Gerenciamento de estado** (useState, useReducer, Context API ou alguma biblioteca externa).
- **Persistência de dados** API

---

## Instruções de Entrega
1. Subir o código em um repositório público no **GitHub** ou **GitLab**.
2. Caso utilize **Docker**, inclua as instruções de execução.
3. Incluir um **README.md** com:
   - Passos para executar a aplicação localmente.
   - Tecnologias utilizadas.
   - Diferenciais implementados (caso tenha).

---

## Critérios de Avaliação
- Organização e estrutura do código.
- Clareza e objetividade nas funcionalidades.
- Uso correto dos hooks do React e gerenciamento de estado.
- Controle de autenticação e fluxo de sessão.
- Documentação e instruções de execução.
