# FastAPI Blog API

A backend blog application built with **FastAPI**, showcasing clean REST API design, secure authentication, data validation, and modular architecture. This project demonstrates key backend development concepts using Python and FastAPI.

---

## 🔧 Functionalities

### ✅ CRUD Operations
- Create, read, update, and delete blog posts and users via RESTful API endpoints.

### 👤 User Management
- User registration with **password encryption**
- User retrieval with sensitive fields hidden (e.g., password)

### 🔐 Authentication
- Secure login using **JWT-based authentication**
- Hashed password storage with **bcrypt** via Passlib
- Token-based access control for protected endpoints

### 🔗 Relationships
- **Users ↔ Blogs** relationship using SQLAlchemy ORM
- Each blog post is linked to its author (User)

### 🧮 Data Validation & Serialization
- **Pydantic** schemas for request/response validation
- Ensures type safety and input sanitization

### 📃 API Documentation
- **Interactive Swagger UI**
- **ReDoc** interface for auto-generated OpenAPI docs

### 🧩 Modular Architecture
- Separation of concerns using:
  - `routers/` (route definitions)
  - `schemas/` (Pydantic models)
  - `models/` (SQLAlchemy models)
  - `repository/` (DB logic)

### ⚠️ Error Handling
- Returns meaningful HTTP status codes
- Centralized exception handling for robustness

### 🔍 Query Parameters
- Support for:
  - Filtering
  - Sorting
  - Pagination

### 🐞 Debugging & Testing
- Works well with **VS Code debugging**
- API testing with **Swagger UI** and **Postman**

---

## 🛠 Tech Stack

| Area                  | Tool/Library       |
|-----------------------|--------------------|
| Programming Language  | Python 3.6+         |
| Web Framework         | FastAPI             |
| ORM / Database        | SQLAlchemy + SQLite |
| Data Validation       | Pydantic            |
| Authentication        | JWT (JSON Web Tokens) |
| Password Hashing      | Passlib (bcrypt)    |
| API Docs              | Swagger UI & ReDoc  |
| Server                | Uvicorn (ASGI)      |
| Debugging             | VS Code             |
| Testing               | Postman, Swagger UI |
| Deployment (optional) | Deta Cloud          |

---

## 🚀 FastAPI Benefits Highlighted

- **High performance**: FastAPI is built on Starlette and Pydantic, making it super fast.
- **Automatic docs**: Swagger and ReDoc documentation with zero config.
- **Type-safe development**: Reduces bugs by enforcing types and validation.
- **Modular structure**: Easily scalable due to clean architecture and DI system.
- **Asynchronous support**: Use of async features enables high concurrency.

---

## 📌 How to Use in Your Project

- Follow modular folder structure for scalability.
- Use Pydantic for all input/output data to ensure validation and security.
- Secure sensitive endpoints using JWT authentication.
- Organize business logic in `repository/` layer to separate it from route definitions.
- Use query parameters to support filtering and pagination.
- Test APIs using Swagger UI or Postman for efficient debugging.
- Consider deploying to free platforms like **Deta**, **Render**, or **Railway**.

---

## 📂 Folder Structure

