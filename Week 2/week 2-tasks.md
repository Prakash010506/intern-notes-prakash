# Week 2 – Tasks

I have started working on the Week 2 practical tasks related to Authentication and Authorization.

1. *No Authentication* – First demo
2. *Basic Authentication* – Second demo
3. *Social / Open Authentication* – Third demo

I have started with the first step, *No Authentication*, and will proceed with the remaining tasks step by step.

# No Authentication:

## Objective

The first practical task is to create a simple Employee Management REST API without authentication and test it using Postman.

## Technology Stack

- Java
- Spring Boot
- Maven
- MySQL
- Postman
- IntelliJ IDEA

## 1. Create the Spring Boot Application

I created a Spring Boot application using Java and Maven.

The application is used to create and retrieve employee information through REST APIs.

## 2. Create Employee Entity

I created an Employee class to represent employee data.

The employee contains:

- ID
- Name
- Email
- Department

The ID is automatically generated and is used as the primary key.

## 3. Connect MySQL Database

I created an employee_db database in MySQL.

The Spring Boot application is configured to connect to this database.

The database is used to store the employee information.

## 4. Create Repository

I created an EmployeeRepository using JpaRepository.

The Repository is responsible for communicating with the database and performing database operations.

## 5. Create Service

I created an EmployeeService.

The Service acts as a middle layer between the Controller and Repository and handles the application logic.

## 6. Create Controller

I created an EmployeeController to handle the REST API requests.

The base API is:/employees

## 7. POST – Create Employee

I used the following API in Postman:

POST http://localhost:8080/employees

POST is used to create new data. Therefore, it represents the *Create* operation in CRUD.

I sent employee details in JSON format:

{
  "name": "Prakash",
  "email": "prakash@gmail.com",
  "department": "IT"
}

### Result

The request returned *200 OK*, and the employee was successfully created and stored in the MySQL database.

## 8. GET – Retrieve Employees

I then used:

GET http://localhost:8080/employees

GET is used to retrieve existing data. Therefore, it represents the *Read* operation in CRUD.

### Result

The request returned *200 OK*, and the employee data stored in the database was successfully displayed in Postman.

## 9. No Authentication

For this first demo, I did not configure any authentication.

I tested the APIs without providing:

- Username
- Password
- Token

Therefore, the API can be accessed without authentication credentials.

## Request Flow

Postman
↓
Controller
↓
Service
↓
Repository
↓
MySQL Database
↓
Response to Postman

## Result

I successfully started and tested the No Authentication REST API. I understood how a request moves through the Controller, Service, and Repository layers and how the application communicates with MySQL.
