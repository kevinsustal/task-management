# Task Management API

The Task Management API is a RESTful web service designed to help users manage their tasks efficiently. This API allows users to create, retrieve, update, and delete tasks, making it a versatile tool for personal task management, project planning, and more.

## Table of Contents

- [Getting Started](#getting-started)
    - [Prerequisites](#prerequisites)
    - [Installation](#installation)
- [Usage](#usage)
    - [API Endpoints](#api-endpoints)
    - [Sample Requests](#sample-requests)
- [Data Model](#data-model)


## Getting Started

### Prerequisites

Before you begin, ensure you have met the following requirements:

- Java 8+ installed
- Spring Boot framework (version x.x.x)
- Your favorite IDE or code editor
- A database (e.g., H2, MySQL, PostgreSQL)

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/kevinsustal/task-management.git
    ```
   ```bash
   cd task-management-api
   ```
   ```bash
   ./mvnw spring-boot:run

The API will be accessible at http://localhost:8080/api/tasks.

### Usage:
- API Endpoints
- GET /api/tasks: Retrieve a list of all tasks.
- GET /api/tasks/{id}: Retrieve a task by its ID.
- POST /api/tasks: Create a new task.
- PUT /api/tasks/{id}: Update an existing task by ID.
- DELETE /api/tasks/{id}: Delete a task by its ID.

  
### Data Model
  The Task entity in the database has the following attributes:

- id (Long): The unique identifier for the task.
- title (String): The title or name of the task.
- description (String): Additional details or notes about the task.
- dueDate (LocalDate): The due date for completing the task.
- completed (boolean): Indicates whether the task is completed (true) or pending (false).