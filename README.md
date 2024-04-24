README FILE
# Registration 

This Spring Boot application provides RESTful APIs for managing user registration.

## Setup

1. **Database Configuration:**

   - Configure your MySQL database connection in the `application.properties` file located at `src/main/resources`.

   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/registerdb
   spring.datasource.username=root
   spring.datasource.password=root
   spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
   spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQL5InnoDBDialect
   spring.jpa.hibernate.ddl-auto=update

2.Dependencies
Spring Boot Starter Web
Spring Boot Starter Data JPA
MySQL Connector Java
Spring Boot Starter Test

3.src/main/java: Java source files
com.example.registration.controller: Controllers handling HTTP requests
com.example.registration.entity: Entity classes representing the data model
com.example.registration.repository: Data repositories
com.example.registration.service: Business logic and services
com.example.registration.Application: Main class with the main method
src/main/resources: Application configuration files
Run the Application:
Run the RegistrationApplication.java file located at src/main/java/com/org/registration

4.The application will start running at http://localhost:8080.
Testing the APIs:
You can use tools like Postman or curl to test the RESTful APIs provided by the application.
API Endpoints
GET /api/register: Get all users.
POST /api/register: Add a new user.
GET /api/register/{id}: Get user by ID.
PUT /api/register/{id}: Update user by ID.
DELETE /apiregister/{id}: Delete user by ID.

