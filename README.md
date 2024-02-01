# registration
Project Structure
The project follows a standard Spring Boot application structure:

src/main/java: Java source files
com.example.registration.controller: Controllers handling HTTP requests
com.example.registration.entity: Entity classes representing the data model
com.example.registration.repository: Data repositories
com.example.registration.service: Business logic and services
com.example.registration.Application: Main class with the main method
src/main/resources: Application configuration files
Running the Application
Configure the database in src/main/resources/application.properties:

properties
Copy code
spring.datasource.url=jdbc:mysql://localhost:3306/your_database_name
spring.datasource.username=your_database_username
spring.datasource.password=your_database_password
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
Run the Spring Boot application:

bash
Copy code
./mvnw spring-boot:run
Or run it from your IDE.

The application should start on http://localhost:8080.

Testing with Postman
Use Postman to test the CRUD operations:

GET All Registrations: GET http://localhost:8080/registrations
GET Single Registration: GET http://localhost:8080/registrations/{id}
CREATE Registration: POST http://localhost:8080/registrations (with JSON body)
UPDATE Registration: PUT http://localhost:8080/registrations/{id} (with JSON body)
DELETE Registration: DELETE http://localhost:8080/registrations/{id}
API Endpoints
GET /registrations: Get all registrations.
GET /registrations/{id}: Get a single registration by ID.
POST /registrations: Create a new registration (JSON body required).
PUT /registrations/{id}: Update an existing registration by ID (JSON body required).
DELETE /registrations/{id}: Delete a registration by ID.
