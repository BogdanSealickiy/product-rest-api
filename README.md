# Product REST API (Spring Boot)

## Overview
This project is a simple REST API created with Spring Boot as a university assignment.  
The application provides basic CRUD operations for managing products.

## Stack
- Java 17  
- Spring Boot  
- Spring Web  
- Spring Data JPA  
- H2 in-memory database  
- Swagger (OpenAPI)  
- Maven  

## How to run
1. Open the project in an IDE (IntelliJ IDEA or VS Code)
2. Run the main application class
3. The server starts on `http://localhost:8080`

## API Testing
Swagger UI is available at:
http://localhost:8080/swagger-ui/index.html


## Available endpoints
- `GET /api/v1/products` – get all products  
- `GET /api/v1/products/{id}` – get product by ID  
- `POST /api/v1/products` – create new product  
- `PUT /api/v1/products/{id}` – update product  
- `DELETE /api/v1/products/{id}` – delete product  

