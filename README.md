# Projeto Loja de Games - Backend

Este projeto é uma API REST desenvolvida durante o bootcamp Java Full Stack, focada na gestão de uma loja de jogos. O sistema permite o gerenciamento completo (CRUD) de produtos e categorias, estabelecendo um relacionamento entre eles.

## 🛠️ Tecnologias Utilizadas

* **Node.js** & **NestJS** (Framework)
* **TypeScript**
* **TypeORM** (Integração com banco de dados)
* **MySQL** (Banco de dados relacional)
* **Class-Validator** & **Class-Transformer** (Validação de dados)

## 📋 Funcionalidades

### Categoria
* `GET /categorias`: Lista todas as categorias.
* `GET /categorias/:id`: Busca categoria por ID.
* `GET /categorias/descricao/:descricao`: Busca categorias por descrição.
* `POST /categorias`: Cadastra nova categoria.
* `PUT /categorias`: Atualiza uma categoria existente.
* `DELETE /categorias/:id`: Remove uma categoria.

### Produto
* `GET /produtos`: Lista todos os produtos (incluindo a categoria associada).
* `GET /produtos/:id`: Busca produto por ID.
* `GET /produtos/nome/:nome`: Busca produtos por nome.
* `POST /produtos`: Cadastra novo produto vinculado a uma categoria.
* `PUT /produtos`: Atualiza dados do produto.
* `DELETE /produtos/:id`: Remove um produto.

## 🚀 Como Executar o Projeto

1.  Certifique-se de ter o **Node.js** e o **MySQL** instalados em sua máquina (Projeto desenvolvido em ambiente Fedora Linux).
2.  Clone o repositório:
    ```bash
    git clone [https://github.com/Duartetais/Loja-de-Game.git](https://github.com/Duartetais/Loja-de-Game.git)
    ```
3.  Instale as dependências:
    ```bash
    npm install
    ```
4.  Configure as credenciais do seu banco de dados no arquivo `src/app.module.ts`.
5.  Execute a aplicação em modo de desenvolvimento:
    ```bash
    npm run start:dev
    ```
6.  A aplicação estará disponível em: `http://localhost:4000`

---
Desenvolvido por **Tais Duarte Bernardi**.