# Employee Management System – Spring Boot MVC Application

## Overview
A Spring Boot MVC–based web application designed to manage employee information with secure,
role-based access. The project demonstrates server-side rendering using Thymeleaf and follows
a layered MVC architecture commonly used in enterprise applications.

## Tech Stack
- Java
- Spring Boot
- Spring MVC
- Spring Security
- Thymeleaf
- MySQL
- JPA / Hibernate
- Maven

## Key Features
- Role-based authentication and authorization (Admin / User)
- Secure form-based login using Spring Security
- Employee CRUD operations
- Server-side rendering with Thymeleaf templates
- Validation and error handling
- Layered architecture (Controller, Service, Repository)

## Architecture
- MVC (Model–View–Controller) architecture
- Controllers handle HTTP requests and responses
- Service layer contains business logic
- Repository layer interacts with the database using JPA/Hibernate

## How to Run Locally

# How to Run Locally

1. Clone the repository
git clone https://github.com/Jash0101/Employee-Management-System-Spring-Boot-MVC-Application.git

2. Open the project in your IDE
(IntelliJ IDEA / Eclipse / VS Code)

3. Create a MySQL database
- Use the SQL script inside sql_scripts
- Make sure MySQL service is running

4. Configure database credentials
- Open src/main/resources/application.properties
- Update the following properties:

spring.datasource.url=jdbc:mysql://localhost:3306/employee_directory
spring.datasource.username=your_username
spring.datasource.password=your_password

5. Build and run the application

Option A: Run using Maven
mvn spring-boot:run

Option B: Build JAR and run
mvn clean package
java -jar target/*.jar

6. Access the application in browser
http://localhost:8080

## Project Structure

```text
Employee-Management-System-Spring-Boot-MVC-Application
├── src/
│   └── main/
│       ├── java/
│       │   └── com/example/ems/
│       │       ├── controller/
│       │       ├── service/
│       │       ├── repository/
│       │       └── model/
│       └── resources/
│           ├── templates/          # Thymeleaf views
│           ├── static/             # CSS/JS (if any)
│           └── application.properties
├── sql_scripts/
│   └── schema.sql                 # MySQL scripts
├── .gitignore
├── README.md
├── mvnw
├── mvnw.cmd
└── pom.xml




