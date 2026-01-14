Product REST API (Spring Boot)
Project Overview

This application is a simple RESTful API developed with Java and Spring Boot.
Its purpose is to provide basic product management functionality using standard CRUD operations (create, read, update and delete).
The data is stored in an H2 in-memory database, and all endpoints can be explored and tested via Swagger UI.

Technologies
The project was built using the following tools and frameworks:

Java 17
Spring Boot 3.3.5
Spring Data JPA
H2 In-Memory Database
OpenAPI / Swagger UI
Maven
API Documentation

All available endpoints are documented using Swagger UI.
You can access it after starting the application:

Swagger UI:
http://localhost:8080/swagger-ui/index.html

Application Functionality
Below is a brief explanation of how the API works and what operations are supported.

1. Swagger UI Overview
Swagger UI displays all REST endpoints exposed by the Product Controller and allows testing them directly from the browser.

2. Create Product
Method: POST
Endpoint: /api/v1/products
Creates a new product and saves it in the database.
Request body: JSON with product name
Response: HTTP 201 (Created) with the saved product and generated ID

4. Get All Products
Method: GET
Endpoint: /api/v1/products
Returns a list of all products stored in the database.

5. Get Product by ID
Method: GET
Endpoint: /api/v1/products/{id}
Fetches a single product based on its identifier.

6. Update Product
Method: PUT
Endpoint: /api/v1/products/{id}
Updates the name of an existing product.
Input: product ID in the URL and JSON body with updated data
Response: HTTP 200 (OK) with modified product

7. Delete Product
Method: DELETE
Endpoint: /api/v1/products/{id}
Deletes a product from the database.
Response: HTTP 204 (No Content)

8. Error Handling
If a product with the given ID does not exist, the API responds with an error message and HTTP status 404 (Not Found).

Database (H2 Console)
To confirm that data is correctly stored, the H2 database console can be used.

Console URL: http://localhost:8080/console

JDBC URL: jdbc:h2:mem:testdb
