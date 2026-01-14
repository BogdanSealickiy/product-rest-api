# Product REST API – Spring Boot Project

## Project Description

This project is a RESTful web application developed using **Java** and **Spring Boot**.  
The application provides basic **CRUD operations** (Create, Read, Update, Delete) for managing products via HTTP requests.

All endpoints are documented and can be tested using **Swagger UI**.  
The application uses an **H2 in-memory database**, so no external database configuration is required.


## Technologies Used

- Java 17  
- Spring Boot  
- Spring Data JPA  
- H2 In-Memory Database  
- OpenAPI / Swagger UI  
- Maven  

## How to Run the Application

1. Clone the repository
2. Open the project in an IDE (IntelliJ IDEA / VS Code)
3. Run the main class
4. The application will start on:

   http://localhost:8080/swagger-ui/index.html

   <img width="1280" height="670" alt="image" src="https://github.com/user-attachments/assets/24684238-25b6-4e6e-af9e-218692b635fc" />

Create Product (POST)
POST /api/v1/products

- **Description:**  
Creates a new product and stores it in the database.
- **Request body:**  
JSON containing the product name
- **Response:**  
`201 Created` with the created product and generated ID

<img width="1280" height="679" alt="image" src="https://github.com/user-attachments/assets/db746781-f408-4754-9954-98b4470e5cf6" />
<img width="1280" height="677" alt="image" src="https://github.com/user-attachments/assets/94338262-691a-4ccf-a2b1-735891efbebe" />

### 2. Get All Products (GET)

- **Description:**  
Retrieves a list of all products stored in the database.
- **Response:**  
`200 OK` with a JSON array of products

### 3 Get Product by ID (GET)
GET /api/v1/products/{id}

- **Description:**  
Retrieves a single product by its unique identifier.
- **Response:**  
`200 OK` if found  
`404 Not Found` if the product does not exist
<img width="1280" height="689" alt="image" src="https://github.com/user-attachments/assets/54c097fb-95b0-4ab3-b07e-dec9a32f913b" />
<img width="1280" height="452" alt="image" src="https://github.com/user-attachments/assets/8a447436-2930-48c6-a08d-9018538fd464" />

### 4. Update Product (PUT)
- **Description:**  
Updates the name of an existing product.
- **Input:**  
Product ID in the URL and JSON body with updated name
- **Response:**  
`200 OK` with updated product  
`404 Not Found` if the product does not exist

<img width="1815" height="1015" alt="image" src="https://github.com/user-attachments/assets/c0daa53f-0ac9-4a1f-b1ce-7b51bc383d06" />
<img width="1821" height="518" alt="image" src="https://github.com/user-attachments/assets/d92416f1-48a1-4b16-bb68-8489e7852552" />

### 5 Get Product by ID 
- **Description:**
  Find the product
- **Input:**  
Product ID in the URL and JSON body with updated name
 **Response:**  
`200 OK` with updated product  
`404 Not Found` if the product does not exist
<img width="1280" height="683" alt="image" src="https://github.com/user-attachments/assets/bb0aa03d-32dd-4792-908d-428fff77cd74" />
<img width="1280" height="687" alt="image" src="https://github.com/user-attachments/assets/be656b70-4e2f-4305-995f-e8408ae8cee6" />






