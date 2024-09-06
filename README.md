RESTful Book Management Application
This is a simple RESTful API for managing a collection of books using Spring Boot and SQLite. The application supports basic CRUD operations such as creating, reading, updating, and deleting books.

Features
CRUD Operations: Create, Read, Update, Delete books.
REST API Endpoints: Provides RESTful endpoints for managing books.
SQLite Database: Uses SQLite as the database for storing book data.
Technologies Used
Java 17
Spring Boot 3.x
Spring Data JPA
SQLite Database
Maven for dependency management
Getting Started
Follow these instructions to set up and run the project on your local machine.

Prerequisites
Java 17 or higher installed
Maven installed
An IDE like IntelliJ IDEA or Eclipse
Configure Database:

The project uses SQLite. No additional setup is needed as the books.db file will be created automatically in the project root.

Update application.properties
Build and Run the Application:

Use Maven to build and run the project:

bash
Copy code
mvn clean install
mvn spring-boot:run

The application will start and run on http://localhost:8080.

Add a New Book:

POST /api/books

json
Copy code
{
"title": "The Great Gatsby",
"author": "F. Scott Fitzgerald",
"publicationYear": 1925
}