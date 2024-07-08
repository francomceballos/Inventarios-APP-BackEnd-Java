# Gestión de Inventarios (Backend)

## Descripción

Este es un proyecto de backend para la gestión de inventarios desarrollado en Java utilizando Spring Boot. La aplicación permite a los usuarios gestionar productos, realizar seguimiento del inventario, y generar reportes sobre el estado del mismo. El frontend de la aplicación se encuentra en un repositorio separado.
Características

    API RESTful para la gestión de inventarios.
    Endpoints para añadir, editar y eliminar productos.
    Endpoints para consultar el inventario disponible.
    Generación de reportes detallados de inventario.
    Búsqueda avanzada de productos.

## Tecnologías Utilizadas

    Lenguaje de Programación: Java
    Framework: Spring Boot
    Librerías: Lombok, Jakarta
    Base de Datos: MySQL (o cualquier otro sistema de gestión de bases de datos)
    Herramienta de Construcción: Maven

## Requisitos

    JDK 11 o superior
    Maven
    MySQL (o cualquier otro sistema de gestión de bases de datos)

## Instalación
1. Clonar el repositorio

bash

git clone https://github.com/tu-usuario/gestion-inventarios-backend.git
cd gestion-inventarios-backend

2. Configurar la base de datos

    Crear una base de datos en MySQL.
    Importar el script de la base de datos database.sql que se encuentra en el directorio sql.

bash

mysql -u tu-usuario -p tu-base-de-datos < sql/database.sql

3. Configurar las credenciales de la base de datos

Editar el archivo src/main/resources/application.properties con las credenciales de tu base de datos.

properties

spring.datasource.url=jdbc:mysql://localhost:3306/tu-base-de-datos
spring.datasource.username=tu-usuario
spring.datasource.password=tu-contraseña
spring.jpa.hibernate.ddl-auto=update

4. Construir el proyecto

bash

mvn clean install

Uso
1. Ejecutar la aplicación

bash

mvn spring-boot:run

2. Interacción con la API

Puedes interactuar con la API utilizando herramientas como Postman o cURL. Los endpoints disponibles son:

    GET /api/products - Obtener todos los productos
    GET /api/products/{id} - Obtener un producto por ID
    POST /api/products - Añadir un nuevo producto
    PUT /api/products/{id} - Actualizar un producto
    DELETE /api/products/{id} - Eliminar un producto

Contribuciones

Las contribuciones son bienvenidas. Por favor, sigue los siguientes pasos para contribuir:

    Realiza un fork del proyecto.
    Crea una nueva rama (git checkout -b feature/nueva-funcionalidad).
    Realiza los cambios necesarios y realiza un commit (git commit -am 'Añadir nueva funcionalidad').
    Sube los cambios a tu repositorio (git push origin feature/nueva-funcionalidad).
    Crea un nuevo Pull Request.

Licencia

Este proyecto está bajo la licencia MIT. Para más detalles, consulta el archivo LICENSE.
