# Spring Boot CRUD API

## Sobre o projeto

API REST desenvolvida com Java e Spring Boot para gerenciamento de clientes, implementando operações completas de CRUD (Create, Read, Update, Delete).

O projeto foi estruturado seguindo boas práticas de desenvolvimento backend, com arquitetura em camadas, tratamento de exceções e validações, simulando um cenário real de aplicação corporativa.

---

## Tecnologias utilizadas

* Java
* Spring Boot
* Spring Data JPA
* Hibernate
* Banco de dados H2
* Maven

---

## Conceitos aplicados

* Arquitetura em camadas (Controller, Service, Repository)
* Padrão DTO para transferência de dados
* Tratamento global de exceções
* Validação de dados com Bean Validation
* CRUD completo com boas práticas REST
* Uso de ResponseEntity para controle de respostas HTTP
* Organização de código seguindo Clean Code e SOLID

---

## Funcionalidades

A API permite o gerenciamento completo de clientes:

* Criar um cliente
* Listar todos os clientes
* Buscar cliente por ID
* Atualizar dados de cliente
* Deletar cliente

---

## Endpoints principais

### Clientes

* GET /clients
* GET /clients/{id}
* POST /clients
* PUT /clients/{id}
* DELETE /clients/{id}

---

## Exemplo de requisição

### Criar cliente (POST /clients)

```json id="exemplo-json"}
{
  "name": "Maria Silva",
  "email": "maria@email.com",
  "phone": "11999999999"
}
```

---

## Como executar o projeto

```bash id="execucao-projeto"}
# Clonar repositório
git clone https://github.com/RODR1GU3S/spring-boot-crud-api

# Entrar na pasta
cd spring-boot-crud-api

# Executar o projeto
./mvnw spring-boot:run
```

A aplicação estará disponível em:
http://localhost:8080

---

## 🧪 Banco de dados H2

Acesse o console do banco em:
http://localhost:8080/h2-console

---

## Tratamento de erros

A API possui tratamento de exceções customizado, retornando respostas padronizadas com:

* Código HTTP adequado
* Mensagem de erro
* Timestamp
* Caminho da requisição

---

## Documentação

Você pode adicionar aqui:

* Swagger/OpenAPI (recomendado)
* Prints das requisições (Postman/Insomnia)

---

## Objetivo do projeto

Este projeto foi desenvolvido com o objetivo de consolidar conhecimentos em APIs REST utilizando Spring Boot, aplicando padrões de mercado para construção de aplicações backend robustas e bem estruturadas.

---

## Contexto profissional

O desenvolvimento deste projeto também reflete a aplicação de análise de regras de negócio e validação de dados, habilidades adquiridas ao longo da experiência profissional em ambientes corporativos.

---

## Melhorias futuras

* Implementação de autenticação com JWT
* Integração com PostgreSQL
* Documentação com Swagger/OpenAPI
* Deploy em ambiente cloud

---

## Autor

Ronaldo Rodrigues
Desenvolvedor Backend Java

* LinkedIn: https://www.linkedin.com/in/ronaldo-rodr1gu3s
* GitHub: https://github.com/RODR1GU3S
