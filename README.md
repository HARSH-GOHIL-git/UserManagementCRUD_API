# User Management API

## Overview
This is a User Management API built using **ASP.NET Core** and **C#**. The API provides a set of endpoints for managing users, including creating, reading, updating, and deleting users. The API also includes custom middleware for logging, error handling, and authentication.

---

## Features
* **CRUD Operations:** Create, read, update, and delete users.
* **Logging Middleware:** Logs all incoming requests and outgoing responses.
* **Error Handling Middleware:** Catches unhandled exceptions and returns consistent, standardized error responses.
* **Authentication Middleware:** Validates tokens from incoming requests, allowing access only to users with a valid token.

---

## API Endpoints

### Users
| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `GET` | `/users` | Returns a list of all users |
| `GET` | `/users/{id}` | Returns a single user by ID |
| `POST` | `/users` | Creates a new user |
| `PUT` | `/users/{id}` | Updates a single user by ID |
| `DELETE` | `/users/{id}` | Deletes a single user by ID |

---

## Usage

1. Clone the repository to your local machine:
2. Open the project in Visual Studio.
3. Build and run the project.
4. Use a tool like Postman to send requests to the API endpoints.

Authentication
To authenticate with the API, you must include a valid token in the Authorization header of your HTTP request. The token should be formatted as follows:

Logging
The API logs all incoming requests and outgoing responses using the custom logging middleware. You can view these logs directly in the console output while the application is running.

Error Handling
The application relies on global error-handling middleware. It safely catches unhandled exceptions and returns clean, consistent JSON error responses rather than exposing stack traces to the client.

Certificate
This project was completed as part of the Coursera - ASP.NET Core API Development course.
https://www.coursera.org/learn/back-end-development-with-dotnet

Acknowledgments
I would like to thank Coursera and the instructors of the ASP.NET Core API Development course for providing the opportunity to learn and complete this project.
