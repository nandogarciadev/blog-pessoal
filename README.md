# Blog Pessoal API

![Java](https://img.shields.io/badge/Java-21-orange)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-4.x-green)
![MySQL](https://img.shields.io/badge/MySQL-8-blue)
![License](https://img.shields.io/badge/Status-Em_Desenvolvimento-success)

API REST desenvolvida com Java e Spring Boot durante o Bootcamp Java Full Stack da Generation Brasil.

## 📋 Sobre o Projeto

O Blog Pessoal é uma aplicação backend que permite o gerenciamento de:

* Usuários
* Postagens
* Temas

Além das operações CRUD, o projeto conta com autenticação e autorização utilizando Spring Security.

---

## 🚀 Tecnologias Utilizadas

* Java 21
* Spring Boot
* Spring Web
* Spring Data JPA
* Spring Security
* MySQL
* Maven
* Hibernate
* Validation
* BCrypt
* Insomnia (testes da API)

---

## 📁 Estrutura do Projeto

```text
src/main/java
│
├── configuration
├── controller
├── model
├── repository
├── security
└── service
```

### Camadas

* **Model** → Entidades da aplicação.
* **Repository** → Comunicação com o banco de dados.
* **Service** → Regras de negócio.
* **Controller** → Endpoints da API.
* **Security** → Autenticação e autorização.
* **Configuration** → Configurações gerais da aplicação.

---

## 🗄️ Banco de Dados

Banco utilizado:

```sql
db_blogpessoal
```

Principais tabelas:

* tb_usuarios
* tb_postagens
* tb_temas

---

## 🔗 Relacionamentos

### Tema → Postagem

* Um Tema possui várias Postagens.
* Uma Postagem pertence a um Tema.

### Usuário → Postagem

* Um Usuário pode criar várias Postagens.
* Uma Postagem pertence a um Usuário.

---

## 🔒 Segurança

A aplicação utiliza:

* Spring Security
* BCrypt Password Encoder
* Basic Authentication

As senhas são armazenadas de forma criptografada no banco de dados.

---

## ▶️ Executando o Projeto

### Clonar o repositório

```bash
git clone URL_DO_REPOSITORIO
```

### Configurar o banco de dados

No arquivo:

```properties
src/main/resources/application.properties
```

Configure:

```properties
spring.datasource.url=jdbc:mysql://localhost/db_blogpessoal
spring.datasource.username=root
spring.datasource.password=sua_senha
```

### Executar a aplicação

```bash
mvn spring-boot:run
```

ou execute a classe:

```java
BlogpessoalApplication
```

---

## 🧪 Testes

Os endpoints podem ser testados utilizando:

* Insomnia
* Postman

---

## 👨‍💻 Autor

Fernando Garcia Cabeceiro

Desenvolvido durante o Bootcamp Java Full Stack da Generation Brasil.
