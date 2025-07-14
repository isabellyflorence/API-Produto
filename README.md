

# 📦 API de Produtos - Sistema de Gestão de Produtos

Este projeto é um sistema simples para a gestão de produtos, desenvolvido com **Java** utilizando **Spring Boot**. Ele permite o **cadastro** e a **listagem de produtos**, armazenando suas informações como nome e preço. O sistema utiliza **H2** como banco de dados em memória e oferece uma interface web básica construída com **Thymeleaf**. **Lombok** é empregado para minimizar o código boilerplate.

---

## 🎯 Funcionalidades

* **Listagem de Produtos**: Visualize todos os produtos cadastrados.
* **Cadastro de Produtos**: Adicione novos produtos com nome e preço.
* **Banco de Dados em Memória**: Utiliza o H2 para uma configuração simples e rápida.
* **Interface Web**: Páginas web básicas para interação com o sistema de produtos.

---

## 🚀 Tecnologias Utilizadas

* **Java 17**: Linguagem principal do projeto
* **Spring Boot**: Framework para o desenvolvimento do backend
* **Spring Web**: Construção de aplicações web
* **Spring Data JPA**: Acesso e persistência de dados
* **H2 Database**: Banco de dados relacional em memória
* **Thymeleaf**: Template engine para renderização da interface web
* **Lombok**: Redução de código repetitivo (getters, setters, etc.)
* **Maven**: Gerenciamento de dependências e automação de builds

---

## 📦 Instalação e Configuração

### 1. Pré-requisitos

Certifique-se de ter instalado:

* Java Development Kit (JDK) 17 ou superior
* Maven 3.9.10 ou superior (ou use o Maven Wrapper incluído)
* Git

### 2. Clonando o Repositório

```bash
git clone https://github.com/Will-firmino/_api_produto
cd _api_produto
```

### 3. Rodando o Projeto

```bash
./mvnw clean install
./mvnw spring-boot:run
```

> No Windows, use `mvnw.cmd` no lugar de `./mvnw`.

A aplicação estará disponível em:
🔗 [http://localhost:8080](http://localhost:8080)

---

## 💻 Interface Web

A aplicação usa **Thymeleaf** para renderização e **Spring MVC** para gerenciamento de requisições.

### Endpoints da Interface Web

* **Listar Produtos**

  * URL: `/`
  * Método: `GET`
  * Exibe a página `listar.html` com todos os produtos

* **Formulário de Cadastro**

  * URL: `/cadastro`
  * Método: `GET`
  * Exibe a página `cadastrar.html` com o formulário

* **Registrar Produto**

  * URL: `/cadastro`
  * Método: `POST`
  * Processa os dados e redireciona para `/`

---

## 🗃️ Banco de Dados H2

Este projeto utiliza o banco de dados H2 em memória. Configuração em `src/main/resources/application.properties`:

```properties
spring.datasource.url=jdbc:h2:mem:produtodb
spring.datasource.driverClassName=org.h2.Driver
spring.datasource.username=sa
spring.datasource.password=
spring.jpa.database-platform=org.hibernate.dialect.H2Dialect
```

⚠️ *Atenção:* os dados são voláteis e serão perdidos ao reiniciar a aplicação.

---

## 🤝 Contribuições

Contribuições são sempre bem-vindas! Fique à vontade para abrir issues ou pull requests.

---

## 📄 Licença

Este projeto está licenciado sob a **MIT License**.



