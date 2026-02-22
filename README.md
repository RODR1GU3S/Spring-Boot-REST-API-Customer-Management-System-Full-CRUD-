# Spring Boot REST API – Customer Management System (Full CRUD)

A professional RESTful backend API built using **Java** and **Spring Boot**, following clean layered architecture principles.

This project demonstrates a complete customer management system with:

- Full CRUD operations
- Pagination and sorting
- DTO pattern
- Bean Validation
- Custom exception handling
- JPA/Hibernate integration
- PostgreSQL configuration

---

## 🚀 Technologies

- Java 11+
- Spring Boot
- Spring Data JPA
- Hibernate
- PostgreSQL
- Maven
- Bean Validation
- DTO Pattern

---

## 📁 Project Structure

```
src/
└── main/
    └── java/
        └── com.devsuperior.desafioCRUDdeClientes
            ├── controllers
            │   ├── ClientController.java
            │   └── handlers/
            │       └── ControllerExceptionHandler.java
            ├── services
            │   ├── ClientService.java
            │   └── exceptions/
            │       └── ResourceNotFoundException.java
            ├── repositories
            │   └── ClientRepository.java
            ├── entities
            │   └── Client.java
            └── dto
                ├── ClientDTO.java
                ├── FieldMessage.java
                └── ValidationError.java
```

---

## 📌 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET    | `/clients` | List clients (pagination supported) |
| GET    | `/clients/{id}` | Get client by ID |
| POST   | `/clients` | Create new client |
| PUT    | `/clients/{id}` | Update client |
| DELETE | `/clients/{id}` | Delete client |

---

## 📄 Example Requests

### 🔎 GET Clients (Paginated)

```http
GET http://localhost:8080/clients?page=0&size=10&sort=id
```

---

### ➕ POST Create Client

```http
POST http://localhost:8080/clients
```

```json
{
  "name": "Maria Silva",
  "cpf": "12345678901",
  "income": 6500.0,
  "birthDate": "1985-12-08",
  "children": 2
}
```

---

## ⚙️ How to Run the Project

### 1️⃣ Clone the repository

```bash
git clone https://github.com/RODR1GU3S/Spring-Boot-REST-API-Customer-Management-System-Full-CRUD-
```

### 2️⃣ Configure Database

Edit `application.properties` and configure your PostgreSQL connection:

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/your_database
spring.datasource.username=your_username
spring.datasource.password=your_password
```

### 3️⃣ Run the application

```bash
mvn spring-boot:run
```

The API will start at:

```
http://localhost:8080
```

---

## 🧠 Key Backend Concepts Demonstrated

- Clean layered architecture
- Separation of concerns
- DTO-based data transfer
- RESTful design standards
- Centralized exception handling
- Structured validation error responses
- Pagination and sorting
- Database persistence with Spring Data JPA

---

## 🎯 Purpose

This project was developed to demonstrate professional backend API development using Spring Boot, aligned with real-world business logic and scalable system design.

---

## 👨‍💻 Author

Ronaldo Rodrigues  
Backend Java & Spring Boot Developer
