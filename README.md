# Gestión de Inventarios (Backend)

Description

This is a backend project for inventory management developed in Java using Spring Boot. The application allows users to manage products, track inventory, and generate reports on its status. The frontend of the application is located in a separate repository.
Features

    RESTful API for inventory management.
    Endpoints to add, edit, and delete products.
    Endpoints to query available inventory.
    Detailed inventory report generation.
    Advanced product search.

Technologies Used

    Programming Language: Java
    Framework: Spring Boot
    Libraries: Lombok, Jakarta
    Database: MySQL (or any other database management system)
    Build Tool: Maven

Requirements

    JDK 11 or higher
    Maven
    MySQL (or any other database management system)

Installation
1. Clone the repository

bash

git clone https://github.com/your-username/inventory-management-backend.git
cd inventory-management-backend

2. Set up the database

    Create a database in MySQL.
    Import the database script database.sql located in the sql directory.

bash

mysql -u your-username -p your-database < sql/database.sql

3. Configure database credentials

Edit the src/main/resources/application.properties file with your database credentials.

properties

spring.datasource.url=jdbc:mysql://localhost:3306/your-database
spring.datasource.username=your-username
spring.datasource.password=your-password
spring.jpa.hibernate.ddl-auto=update

4. Build the project

bash

mvn clean install

Usage
1. Run the application

bash

mvn spring-boot:run

2. Interact with the API

You can interact with the API using tools like Postman or cURL. The available endpoints are:

    GET /api/products - Get all products
    GET /api/products/{id} - Get a product by ID
    POST /api/products - Add a new product
    PUT /api/products/{id} - Update a product
    DELETE /api/products/{id} - Delete a product

Contributions

Contributions are welcome. Please follow these steps to contribute:

    Fork the project.
    Create a new branch (git checkout -b feature/new-feature).
    Make necessary changes and commit (git commit -am 'Add new feature').
    Push changes to your repository (git push origin feature/new-feature).
    Create a new Pull Request.

License

This project is licensed under the MIT License. For more details, see the LICENSE file.
