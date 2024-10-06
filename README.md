# todolist-with-fast_api

This is a TodoList API built using FastAPI that includes authentication.

## Features
- User registration and login (authentication)
- CRUD operations for Todos (Create, Read, Update, Delete)
- Admin routes for user and task management

 ## Project Structure
ToDoApp/ │ ├── main.py # Application entry point ├── database.py # Database setup and connection ├── models.py # Database models ├── routers/ # API routes │ ├── todos.py # Routes for managing todos │ ├── users.py # Routes for user management │ ├── auth.py # Authentication routes │ └── admin.py # Admin routes for system management

## Requirements
- Python 3.8+
- FastAPI
- SQLAlchemy
- Uvicorn
- Pydantic
- bcrypt
- JWT

## How to run the Application
1. Clone the repository
   git clone https://github.com/Galya808/todolist-api.git
2. Navigate to the project directory
   cd todolist-api
3. Create a .env file for environment variables
4. Run the application
   uvicorn main:app --reload

# Endpoints
## Authentication
1. ## POST /auth/signup - Register a new user
2. ## POST /auth/login - Login a user
## Todos
1. ## GET /todos/ - Get all todos
2. ## POST /todos/ - Create a new todo
3. ## PUT /todos/{id} - Update a todo by ID
4. ## DELETE /todos/{id} - Delete a todo by ID
## Admin
1. ## GET /admin/ - Get a list of all users
2. ## DELETE /admin/{todo_id} - Delete a todo by ID

# Database

This project uses SQLAlchemy for database management. You can configure the database (SQLite, PostgreSQL, etc.) in the .env file.

