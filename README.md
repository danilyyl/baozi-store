# Baozi Store API

API REST desenvolvida para a disciplina de Desenvolvimento Web Back-End, com o objetivo de aplicar na prática conceitos de desenvolvimento de APIs, arquitetura MVC, persistência de dados e operações CRUD utilizando Java e Spring Boot.

O projeto simula o sistema de uma pequena loja de pão chinês, a Baozi Store, permitindo o gerenciamento básico de clientes, produtos e pedidos.

> Projeto acadêmico desenvolvido como atividade prática da disciplina de Desenvolvimento Web Back-End.

---

## Sobre o projeto

A Baozi Store é uma pequena loja que comercializa pão chinês e necessita de uma solução simples para organizar o cadastro de clientes, produtos e pedidos.

A API foi desenvolvida para representar esse cenário de forma prática, permitindo:

- cadastrar clientes;
- consultar clientes;
- cadastrar produtos;
- consultar produtos;
- registrar pedidos;
- consultar pedidos;
- excluir registros.

Cada pedido está relacionado a um cliente, a um produto e à quantidade adquirida.

O projeto utiliza uma arquitetura baseada no padrão MVC do Spring e persistência de dados através do Spring Data JPA e MySQL.

---

## Objetivos

O desenvolvimento teve como principais objetivos:

- compreender a estrutura de uma aplicação REST;
- desenvolver endpoints HTTP utilizando Spring Boot;
- trabalhar com entidades persistentes utilizando JPA;
- realizar operações CRUD;
- integrar uma aplicação Java com um banco de dados relacional;
- utilizar JSON na comunicação entre cliente e API;
- organizar a aplicação utilizando os conceitos do padrão MVC;
- testar os endpoints utilizando o Postman.

---

## Tecnologias utilizadas

| Tecnologia | Utilização |
|---|---|
| Java 21 | Linguagem de programação |
| Spring Boot | Desenvolvimento da aplicação |
| Spring Web | Criação da API REST |
| Spring Data JPA | Persistência e acesso aos dados |
| Hibernate | Implementação JPA utilizada pelo projeto |
| MySQL | Banco de dados relacional |
| Maven | Gerenciamento do projeto e dependências |
| Postman | Testes dos endpoints |
| Eclipse IDE | Ambiente de desenvolvimento |
| Git | Controle de versão |
| GitHub | Hospedagem do código-fonte |

---

## Arquitetura do projeto

O projeto segue uma organização baseada no padrão MVC e está estruturado em pacotes de acordo com suas responsabilidades.

```text
src/
└── main/
    ├── java/
    │   └── com.baozistore/
    │       ├── controller/
    │       │   ├── ClienteController.java
    │       │   ├── ProdutoController.java
    │       │   └── PedidoController.java
    │       │
    │       ├── model/
    │       │   ├── Cliente.java
    │       │   ├── Produto.java
    │       │   └── Pedido.java
    │       │
    │       ├── repository/
    │       │   ├── ClienteRepository.java
    │       │   ├── ProdutoRepository.java
    │       │   └── PedidoRepository.java
    │       │
    │       └── BaoziStoreApplication.java
    │
    └── resources/
        └── application.properties
