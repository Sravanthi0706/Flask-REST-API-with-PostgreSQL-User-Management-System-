Flask REST API – User Management Backend

Professional Summary
This project is a RESTful backend API built using Python Flask and PostgreSQL. It implements complete CRUD operations, user registration, input validation, and pagination. The project follows a Controller–Model–Config architecture and demonstrates real-world backend development practices suitable for scalable and production-ready applications.

Key Skills Demonstrated
- Python Backend Development
- REST API Design
- Flask Framework
- PostgreSQL Database Integration
- SQL (CRUD Operations, Pagination)
- Controller–Model–Config Architecture
- Input Validation and Error Handling
- Modular and Maintainable Code Design

System Architecture
Client (Postman / Frontend)
→ Flask Controller Layer (Routes)
→ Business Logic Layer (Models)
→ PostgreSQL Database

Project Structure
FastAPI_Python/
├── app.py                     # Application entry point
├── controller/
│   └── home.py                # REST API endpoints
├── models/
│   ├── my_model.py            # Database CRUD operations
│   ├── user_register.py       # User registration workflow
│   ├── validator.py           # Input validation logic
│   └── random_keygen.py       # Unique user key generation
├── configs/
│   └── config.py              # PostgreSQL configuration
└── README.md

Core Features
- RESTful API implementation using Flask
- User registration with structured validation
- PostgreSQL integration using psycopg2
- Create, Read, Update, and Delete (CRUD) operations
- Pagination support for large datasets
- Modular and extensible codebase
- Structured JSON API responses

API Endpoints
POST  /user/v1/register                 Register a new user
GET   /freek/home                       Fetch all users
POST  /freek/update                     Update user information
POST  /freek/delete                     Delete a user
GET   /freek/limit/<limit>/page/<page>  Paginated user listing

Validation and Data Integrity
- Email format validation
- Phone number validation
- Username and password validation
- Centralized validation utilities
- Defensive error handling with meaningful responses

Technology Stack
Language: Python 3
Framework: Flask
Database: PostgreSQL
Database Driver: psycopg2
API Style: REST
Architecture: Controller–Model–Config
Data Format: JSON

How to Run the Project
1. Clone the repository
2. Create and activate a virtual environment
3. Install dependencies (Flask, psycopg2)
4. Configure PostgreSQL credentials in configs/config.py
5. Run the application using python app.py

Security and Best Practices
- Parameterized SQL queries
- Input validation to reduce injection risks
- Unique identifiers for user records
- Clean separation of concerns

