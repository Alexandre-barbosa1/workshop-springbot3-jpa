# 🛠️ Projeto Workshop Spring Boot 3 + JPA
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/Alexandre-barbosa1/workshop-springbot3-jpa/blob/main/LICENSE)

# Sobre o projeto
Este é um projeto backend desenvolvido com **Spring Boot 3**, com o objetivo de praticar conceitos de **API RESTful**, **JPA/Hibernate**, **banco de dados relacional** e **boas práticas de desenvolvimento em camadas**.

A aplicação simula um sistema simples de e-commerce, com cadastro de usuários, produtos e pedidos.

## Layout
Este projeto não possui interface gráfica, sendo acessado por meio de **endpoints REST**, que podem ser testados com ferramentas como **Postman**, **Insomnia** ou diretamente no navegador (para requisições GET).

## Modelo conceitual
- Cadastro de **Usuários** (nome, email, telefone)
- Cadastro de **Produtos** (nome, descrição, preço)
- Registro de **Pedidos** com:
  - Data e hora do pedido
  - Status (PAID, WAITING_PAYMENT, etc.)
  - Associação ao usuário
  - Lista de itens do pedido com quantidade e preço
- Relacionamentos:
  - Um usuário pode ter vários pedidos (1:N)
  - Um pedido possui vários itens (1:N)
  - Um item referencia um produto (N:1)

# Tecnologias utilizadas

## Back end
- Java 17+
- Spring Boot 3
- Spring Data JPA
- H2 Database
- Maven
- IntelliJ

# Como executar o projeto

### Pré-requisitos
Java 17 ou superior e Maven instalados

## Back end

```bash
# Clone o repositório
git clone https://github.com/Alexandre-barbosa1/workshop-springbot3-jpa

# Acesse a pasta do projeto
cd workshop-springbot3-jpa

# Execute o projeto com Maven
./mvnw spring-boot:run
Acesse os endpoints no navegador ou via Postman:

http://localhost:8080/users

http://localhost:8080/orders

http://localhost:8080/products
```
Autor
👨‍💻 Alexandre Barbosa
www.linkedin.com/in/alexandrebarbosa01
