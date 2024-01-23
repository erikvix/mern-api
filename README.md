# API CRUD com Node.js, Express.js, e MongoDB

Esta é uma API de CRUD (Create, Read, Update, Delete) desenvolvida com Node.js, Express.js, e MongoDB. Além das operações CRUD básicas, a API também incorpora funcionalidades de middleware para melhorar a segurança e modularidade do código.

## Funcionalidades

- **Criação (Create):** Adiciona um novo recurso ao banco de dados.
- **Leitura (Read):** Recupera informações sobre um recurso ou todos os recursos.
- **Atualização (Update):** Modifica informações existentes de um recurso.
- **Exclusão (Delete):** Remove um recurso do banco de dados.
- **Middleware de Validação com Yup:** Utiliza o Yup para validar as requisições antes de processá-las.
- **Criptografia de Senha com Bcrypt.js:** Protege as senhas dos usuários por meio de criptografia.
- **Modularização das Rotas com Router do Express:** Organiza as rotas da API de maneira modular.

## Tecnologias Utilizadas

- Node.js
- Express.js
- MongoDB (ou outra base de dados à sua escolha)
- Yup (para validação)
- Bcrypt.js (para criptografia de senha)
- Mongoose (para modelos e interação com o MongoDB)

## Instalação

1. Clone o repositório:

   ```bash
   git clone https://github.com/seu-usuario/nome-do-repositorio.git

2. Acesse o diretório do projeto:

    ```bash
    cd nome-do-repositorio
    ```

3. Instale as dependências:

    ```bash
    npm install
    ```
4. Configure o banco de dados no arquivo .env (crie um arquivo .env na raiz do projeto e adicione as variáveis necessárias).

5. Inicie o servidor:
    ```bash
    npm start
    ```

A API estará disponível em http://localhost:3000 (ou a porta configurada).

## Estrutura do Projeto

- /middlewares: Contém middleware de validação.
- /models: Armazena os modelos do Mongoose para os recursos da API.
- /routes: Rotas modularizadas utilizando o Router do Express.

## Rotas da API

- GET /users: Retorna todos os usuários.
- GET /user: Retorna um usuário específico.
- POST /user: Cria um novo recurso.
- PUT /user/:_id: Atualiza um usuário existente.
- DELETE /user/:_id: Remove um usuário.
