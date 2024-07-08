# Inventory Management System Backend

This project provides backend services for an inventory management system developed in Java using Spring Boot. It includes RESTful APIs for managing products, allowing CRUD operations and interacting with a MySQL database.

## Features

-   **RESTful API**: Provides endpoints for managing products.
-   **CRUD Operations**: Supports Create, Read, Update, and Delete operations for products.
-   **Logging**: Utilizes SLF4J for logging API operations.
-   **Cross-Origin Resource Sharing (CORS)**: Configured to allow requests from `http://localhost:4200`.

## Technologies Used

-   **Java**: Programming language used for backend development.
-   **Spring Boot**: Framework for creating Java applications.
-   **MySQL**: Database management system for storing product data.
-   **Maven**: Build automation tool for managing dependencies.

## Getting Started

To run this application locally, follow these steps:

### Prerequisites

-   JDK 11 or higher
-   Maven
-   MySQL

### Installation

1.  **Clone the repository:**
    
   ### Installation

1.  **Clone the repository:**
   
```
     git clone https://github.com/your-username/inventory-management-backend.git cd inventory-management-backend
```
2. **Set up the database:**

-   Create a MySQL database.
-   Import the database schema using `database.sql` located in the `sql` directory.

    mysql -u your-username -p your-database < sql/database.sql
    
3. **Configure database credentials:**

	Update the `application.properties` file located in `src/main/resources/` with your database credentials:
```
    spring.datasource.url=jdbc:mysql://localhost:3306/your-database 
    spring.datasource.username=your-username  
    spring.datasource.password=your-password 
    spring.jpa.hibernate.ddl-auto=update
```
    
4. Build and run the application:
```
    mvn clean install 
    mvn spring-boot:run
```
### Usage

Once the application is running, you can interact with the API using tools like Postman or cURL:

-   **GET `/inventario-app/productos`**: Retrieve all products.
-   **GET `/inventario-app/productos/{id}`**: Retrieve a product by ID.
-   **POST `/inventario-app/productos`**: Add a new product.
-   **PUT `/inventario-app/productos/{id}`**: Update a product.
-   **DELETE `/inventario-app/productos/{id}`**: Delete a product.

### Contributing

Contributions are welcome! If you want to contribute to this project, please follow these steps:

1.  Fork the repository on GitHub.
2.  Create a new branch with a descriptive name (`git checkout -b feature/new-feature`).
3.  Commit your changes (`git commit -am 'Add new feature'`).
4.  Push to the branch (`git push origin feature/new-feature`).
5.  Create a new Pull Request.

### License

This project is licensed under the MIT License - see the LICENSE file for details.
