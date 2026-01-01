# Secure API Demo

A secure REST API built with Spring Boot using JWT authentication and Swagger (OpenAPI) documentation.  
This project demonstrates stateless authentication, protected endpoints, and clean backend architecture suitable for a professional portfolio.

## Features
- User registration and login
- JWT (JSON Web Token) authentication
- Stateless security with Spring Security
- Protected REST API endpoints
- Swagger (OpenAPI) documentation
- H2 in-memory database for development

## Tech Stack
- Java 17+
- Spring Boot
- Spring Security
- JWT (jjwt)
- Swagger / OpenAPI (springdoc)
- H2 Database
- Maven

## Project Structure
```
src/main/java/com/example/secure_api_demo
├── controller
│   ├── AuthController.java
│   └── HelloController.java
├── model
│   └── User.java
├── repository
│   └── UserRepository.java
├── security
│   ├── JwtAuthenticationFilter.java
│   ├── JwtUtil.java
│   └── SecurityConfig.java
├── config
│   └── OpenApiConfig.java
└── SecureApiDemoApplication.java
```

## Authentication Overview
- Users authenticate using username and password
- Passwords are securely hashed using BCrypt
- Successful authentication returns a signed JWT
- JWT is required to access protected endpoints
- A custom Spring Security filter validates tokens on each request

## API Documentation
Swagger UI is available once the application is running:
```
http://localhost:8080/swagger-ui.html
```

## Running the Application
```bash
git clone https://github.com/Nbennacer/secure-api-demo.git
cd secure-api-demo
mvn spring-boot:run
```

## Purpose
This project was built to demonstrate secure backend development with Spring Boot, JWT-based authentication, and clean REST API design. It is intended for learning and portfolio presentation.

## Author
Nour Bennacer  
https://github.com/Nbennacer
