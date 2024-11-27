X2-Employee Management System (Spring Boot)
This is an Employee Management System built using Spring Boot, which allows users to manage employee data including adding, updating, deleting, and viewing employee details. The application also includes a simple web interface for interacting with employee records.

Features
Home Page: Displays a list of all employees.
Add Employee: Form to add a new employee.
Edit Employee: Allows editing employee details.
Delete Employee: Deletes an employee record.
Employee Search: (This feature is currently commented out in the code but can be implemented).

Technologies Used
Spring Boot: Backend framework for building RESTful web services.
Thymeleaf: Templating engine for rendering HTML views.
Spring Data JPA: For database interaction.
H2 Database: In-memory database for storing employee information (can be changed to any other database).
Maven: Dependency management and build tool.


Getting Started

Prerequisites
To run this project locally, you need to have the following tools installed:

Java 23 or higher
Maven
IDE (e.g., IntelliJ IDEA, Eclipse)
Steps to Run Locally
Clone this repository:

bash
Copy code
git clone https://github.com/atulshivaan/base.git
Navigate to the project directory:

bash
Copy code
cd X2
Build the project with Maven:

bash
Copy code
mvn clean install
Run the Spring Boot application:

bash
Copy code
mvn spring-boot:run
Open your browser and go to http://localhost:8080 to access the application.

Endpoints
GET /: Displays a list of all employees.
GET /add-emp: Displays the form to add a new employee.
POST /register: Adds a new employee to the system.
GET /edit/{id}: Displays the form to edit an employee's details.
POST /update: Updates an existing employee's information.
GET /delete/{id}: Deletes an employee by ID.

Project Structure
src/main/java/com/eX2/X2/controller: Contains the main controller (xcontroller) responsible for handling HTTP requests and managing the application flow.
src/main/java/com/eX2/X2/entity: Contains the Employee entity class representing an employee.
src/main/java/com/eX2/X2/service: Contains the EmpService class for business logic and CRUD operations related to employees.
src/main/resources/templates: Contains the Thymeleaf templates (HTML files) for rendering views.
src/main/resources/application.properties: Configuration file for Spring Boot application settings.
