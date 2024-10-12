# User Service

This is a Spring Boot application that provides a RESTful API for managing users.  It uses Spring Data JPA for database interaction and exposes endpoints for creating, reading, updating, and deleting users.

## Features

* **CRUD operations:** Create, Read, Update, and Delete users.
* **Search by username and email:** Retrieve users by their unique username or email address.
* **Filter by role and active status:** Get a list of users based on their assigned role or active status.
* **Cross-origin support:** Allows requests from `http://localhost:4200`, facilitating frontend development.

## Technologies Used

* **Java 17 (or higher):** The programming language used.
* **Spring Boot:** Framework for building stand-alone, production-grade Spring-based applications.
* **Spring Data JPA:** Simplifies database access and object-relational mapping.
* **Jakarta Persistence API (JPA):** Standard for managing persistence and object-relational mapping in Java.


## Getting Started

1. **Prerequisites:** Ensure you have Java 17 (or compatible) and Maven installed on your system.

2.**Build**
Build the application:

mvn clean install
content_copy
Use code with caution.
Bash

Run the application:

mvn spring-boot:run
content_copy
Use code with caution.
Bash

Access the API: The API will be accessible at http://localhost:8080/api/users.

API Endpoints
Method	Endpoint	Description
GET	/api/users	Retrieves all users.
GET	/api/users/{id}	Retrieves a user by ID.
POST	/api/users	Creates a new user.
PUT	/api/users/{id}	Updates an existing user.
DELETE	/api/users/{id}	Deletes a user by ID.
GET	/api/users/username/{username}	Retrieves a user by username.
GET	/api/users/email/{email}	Retrieves a user by email.
GET	/api/users/role/{role}	Retrieves users by role.
GET	/api/users/active	Retrieves all active users.
Database Configuration

The application uses an embedded H2 database by default. You can configure a different database by modifying the application.properties file.


