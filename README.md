**Fiber Todo App with MongoDB**
This project is a simple TODO application built using Go, the Fiber framework, and MongoDB. It demonstrates how to create a RESTful API with CRUD operations for managing TODO items.

Code Overview
1. Fiber Framework: Provides a lightweight and fast HTTP server for handling API requests.
2. MongoDB: Used as the database to store TODO items.
3. Environment Variables: The application reads configuration like MONGO_URI and PORT from a .env file using the godotenv package.
4. Data Model:
    * Each TODO item has:
       a. ID (ObjectID): MongoDB's unique identifier.
       b. Completed (bool): Status of the TODO.
       c. Body (string): Description of the task.

      
Endpoints
GET /api/todos: Retrieves all TODO items from the database.
POST /api/todos: Adds a new TODO item.
PATCH /api/todos/:id: Marks a TODO item as completed using its ID.
DELETE /api/todos/:id: Deletes a TODO item by its ID.


The application handles request parsing, validation, and error handling, ensuring smooth interaction with the database
