# Product API - Spring Boot

Esta é uma API REST de gerenciamento de produtos desenvolvida com o framework **Spring Boot**. A aplicação realiza operações básicas de CRUD (Create, Read, Update, Delete) e utiliza o banco de dados **H2**, que é leve, embutido e ideal para testes e desenvolvimento.

## 🚀 Tecnologias Utilizadas

- **Java 21**
- **Spring Boot**
- **Spring Data JPA**
- **H2 Database**
- **Lombok**
- **Maven**

## 📦 Funcionalidades

A API permite realizar as seguintes operações com produtos:

- **GET /products** — Retorna a lista de todos os produtos cadastrados.
- **GET /products/{id}** — Retorna os detalhes de um produto específico.
- **POST /products** — Cadastra um novo produto.
- **PUT /products/{id}** — Atualiza um produto existente.
- **DELETE /products/{id}** — Remove um produto do sistema.

## 💾 Banco de Dados H2

A aplicação utiliza o banco de dados em memória H2, que pode ser acessado através do console web:

- **URL:** `http://localhost:8080/h2-console`
- **JDBC URL:** `jdbc:h2:mem:testdb`
- **User:** `sa`
- **Password:** *(em branco)*

## 📌 Requisitos

- Java 17 ou superior
- Maven 3.x

## ▶️ Como Executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/Beletatti/productapi-springboot.git
2. Compile o projeto:
   ```bash
   mvn clean install
3. Execute a aplicação:
   ```bash
   mvn spring-boot:run
4. Acesse a API em:
   ```bash
   http://localhost:8080/products

## 📬 Exemplos de Requisições

Criar Produto (POST):
```bash
  POST /products
  Content-Type: application/json

  {
    "name": "Notebook Dell",
    "description": "Modelo XPS 13 com 16GB RAM",
    "price": 6500.00
  }
```
Atualizar Produto (PUT):
```bash
PUT /products/1
Content-Type: application/json

{
  "name": "Notebook Dell Atualizado",
  "description": "Modelo XPS 13 com 32GB RAM",
  "price": 7500.00
}
```
## ✅ Testes
A aplicação pode ser facilmente testada via ferramentas como Postman, Insomnia ou diretamente pelo Swagger, caso seja adicionado.





