# API REST con Spring Boot y MySQL

## Descripción

Esta es una API RESTful creada utilizando **Spring Boot**. La API interactúa con una base de datos **MySQL** para realizar operaciones CRUD (Crear, Leer, Actualizar, Eliminar). Está pensada para ser usada en aplicaciones que requieren la gestión de datos mediante un backend robusto y flexible.

## Características

- **Framework**: Spring Boot 3.3.1
- **Base de datos**: MySQL
- **Persistencia de datos**: Spring Data JPA
- **Dependencias**:
  - `spring-boot-starter-data-jpa`: Para la interacción con la base de datos mediante JPA.
  - `spring-boot-starter-web`: Para la creación de endpoints RESTful.
  - `mysql-connector-j`: Conector para la base de datos MySQL.
  - `spring-boot-devtools`: Herramientas para desarrollo.
  - `spring-boot-starter-test`: Para pruebas unitarias.

## Requisitos Previos

Antes de ejecutar este proyecto, asegúrate de tener instalado lo siguiente:

- **Java 17** o superior
- **Maven** (para la gestión de dependencias y compilación)
- **MySQL** (con una base de datos creada)
  
### Configuración de MySQL

Asegúrate de tener una base de datos MySQL configurada. Puedes modificar los detalles de la conexión en el archivo `application.properties` de tu proyecto:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/tu_base_de_datos
spring.datasource.username=tu_usuario
spring.datasource.password=tu_contraseña
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
