# Simple Banking App - Spring Boot REST API

This repository ([SpringBoot-Bankking-App-Service](https://github.com/Sangramjit786/SpringBoot-Bankking-App-Service.git)) demonstrates the development of a **simple banking application** built with **Spring Boot**.  
The project focuses on learning and applying **REST API concepts** in a microservice-like setup, while also experimenting with modern Java features like **Java Records** instead of Lombok for Data Transfer Objects (DTOs).  

A simple banking application built with Spring Boot that demonstrates core REST API concepts for account management. This project serves as an educational example for understanding how to build RESTful web services with Spring Boot.

---

### Simple Banking App with REST APIs
- Built a **Spring Boot project** that simulates basic banking operations (e.g., accounts, transactions, customers).  
- Designed RESTful endpoints (`@RestController`) to expose the core functionalities.  
- Provides a **hands-on learning experience** for understanding REST concepts like:
  - HTTP verbs (`GET`, `POST`, `PUT`, `DELETE`)  
  - Request/response handling  
  - Validation and error responses  
  - Separation of layers (Controller, Service, Repository, DTOs)  

This ensures developers can **strengthen their REST fundamentals** while working on a real-world inspired project.

---

### Using Java Records Instead of Lombok
- Traditionally, projects use **Lombok** annotations (`@Getter`, `@Setter`, `@Builder`, etc.) to reduce boilerplate code in DTOs and entities.  
- In this project, **Java Records (introduced in Java 14, stable in Java 16+)** are used for **DTO classes** instead of Lombok.  

#### Why Java Records?
- **Concise syntax**: A record automatically provides `getter` methods, `equals()`, `hashCode()`, and `toString()`.  
- **Immutable data carrier**: Perfect for DTOs, which should not be modified after creation.  
- **No extra dependencies**: Unlike Lombok, records are part of the JDK.

---

#### Example:
```java
// Traditional DTO with Lombok
@Data
@AllArgsConstructor
@NoArgsConstructor
public class AccountDTO {
    private String accountId;
    private String accountType;
    private double balance;
}

// DTO using Java Record
public record AccountDTO(String accountId, String accountType, double balance) {}
```

---

## 🚀 Key Features

- **RESTful API Endpoints** for account operations
- **Clean Architecture** with clear separation of concerns
- **Modern Java Features** including Java Records for DTOs
- **H2 In-Memory Database** for easy setup and development
- **Spring Data JPA** for database operations
- **Maven** for dependency management

## 🛠 Technical Stack

- **Java 21** (or later)
- **Spring Boot 3.x**
- **Spring Data JPA**
- **H2 Database**
- **Maven**
- **Java Records** (instead of Lombok)

## 🌟 Project Highlights

### 1. Modern Java Records for DTOs

This project leverages Java Records (introduced in Java 14) instead of using Lombok for handling boilerplate code in DTOs. Records provide a concise way to model immutable data in Java.

**Example from the project:**
```java
public record AccountDto(Long id, String accountHolderName, double balance) {
}
```

### 2. REST API Endpoints

The application provides the following REST endpoints:

- `POST /api/accounts` - Create a new account
- `GET /api/accounts/{id}` - Get account by ID
- `GET /api/accounts` - Get all accounts
- `PUT /api/accounts/{id}/deposit` - Deposit money
- `PUT /api/accounts/{id}/withdraw` - Withdraw money
- `DELETE /api/accounts/{id}` - Delete account

## 🚀 Getting Started

### Prerequisites

- Java 17 or later
- Maven 3.6.3 or later

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Sangramjit786/SpringBoot-Bankking-App-Service.git
   cd SpringBoot-Bankking-App-Service
   ```

2. Build the project:
   ```bash
   mvn clean install
   ```

3. Run the application:
   ```bash
   mvn spring-boot:run
   ```

The application will start on `http://localhost:8080`

## 📚 Learning Resources

This project is an excellent resource for learning:
- REST API design principles
- Spring Boot application structure
- Data Transfer Objects (DTOs) with Java Records
- CRUD operations with Spring Data JPA
- Exception handling in Spring Boot

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

Developed with ❤️ for educational purposes
