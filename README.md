# Simple Banking App - Spring Boot REST API

A simple banking application built with Spring Boot that demonstrates core REST API concepts for account management. This project serves as an educational example for understanding how to build RESTful web services with Spring Boot.

## 🚀 Key Features

- **RESTful API Endpoints** for account operations
- **Clean Architecture** with clear separation of concerns
- **Modern Java Features** including Java Records for DTOs
- **H2 In-Memory Database** for easy setup and development
- **Spring Data JPA** for database operations
- **Maven** for dependency management

## 🛠 Technical Stack

- **Java 17** (or later)
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
