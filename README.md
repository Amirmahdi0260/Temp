<div align="center">

# 🚀 XTask

### A Modern Task Management REST API built with .NET 10

A scalable and maintainable Task Management system developed using **ASP.NET Core Web API**, **Onion Architecture**, and **Entity Framework Core**.

![.NET](https://img.shields.io/badge/.NET-10-512BD4?style=for-the-badge\&logo=dotnet)
![ASP.NET Core](https://img.shields.io/badge/ASP.NET_Core-Web_API-5C2D91?style=for-the-badge\&logo=dotnet)
![C#](https://img.shields.io/badge/C%23-14-239120?style=for-the-badge\&logo=c-sharp)
![EF Core](https://img.shields.io/badge/Entity_Framework_Core-10-512BD4?style=for-the-badge)
![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=for-the-badge\&logo=microsoftsqlserver)
![License](https://img.shields.io/badge/License-MIT-success?style=for-the-badge)

</div>

---

# 📖 About

**XTask** is a RESTful Task Management API designed with modern software architecture principles. It provides secure authentication, role-based authorization, project management, and task lifecycle management while keeping the codebase clean, scalable, and easy to maintain.

The project follows **Onion Architecture** and implements the **Repository Pattern** and **Unit of Work Pattern** to separate concerns and simplify future development.

---

# ✨ Features

## 🔐 Authentication & Authorization

* Cookie-Based Authentication
* Secure Login & Logout
* Role-Based Authorization
* Protected API Endpoints

---

## 👥 User Management

* User Registration
* User Authentication
* Role Management

### Administrator Privileges

Administrators can:

* Grant the **Admin** role to another user.
* Revoke the **Admin** role from existing administrators.

Role management is fully handled through the API without requiring manual database changes.

---

## 📁 Project Management

* Create Projects
* Update Projects
* Soft Delete Projects
* Restore Deleted Projects
* Project Status Management

### Automatic Project Completion

When every task belonging to a project reaches the **Completed** status, the project is automatically marked as **Completed**.

This business rule ensures project consistency without manual intervention.

---

## ✅ Task Management

* Create Tasks
* Assign Tasks to Users
* Update Task Status
* Pending
* In Progress
* Completed
* Rejected
* Canceled
* Soft Delete Tasks
* Restore Deleted Tasks

---

# 🏛️ Architecture

The project follows the **Onion Architecture** pattern.

```text
Presentation (Web API)
        │
Application
        │
Domain
        │
Infrastructure
```

## Design Patterns

* Onion Architecture
* Repository Pattern
* Unit of Work
* Dependency Injection
* Service Layer

---

# ⚡ Performance

The project follows Entity Framework Core performance best practices.

* Asynchronous database operations
* Optimized LINQ queries
* AsNoTracking for read-only operations
* Soft Delete strategy
* Efficient Change Tracking
* Reduced unnecessary memory allocations
* Clean repository implementation

---

# 🛠️ Technology Stack

| Category             | Technology                       |
| -------------------- | -------------------------------- |
| Framework            | .NET 10                          |
| API                  | ASP.NET Core Web API             |
| Language             | C#                               |
| ORM                  | Entity Framework Core 10         |
| Database             | SQL Server                       |
| Authentication       | Cookie Authentication            |
| Architecture         | Onion Architecture               |
| Design Patterns      | Repository Pattern, Unit of Work |
| Dependency Injection | Built-in .NET DI                 |

---

# 📂 Project Structure

```text
XTask

├── XTask.Api
├── XTask.Application
├── XTask.Domain
├── XTask.Infrastructure
```

---

# 🚀 Getting Started

## Requirements

* .NET 10 SDK
* SQL Server

## Clone Repository

```bash
git clone https://github.com/your-username/XTask.git
```

## Restore Packages

```bash
dotnet restore
```

## Apply Migrations

```bash
dotnet ef database update
```

## Run

```bash
dotnet run
```

---

# 🎯 What This Project Demonstrates

* ASP.NET Core Web API
* .NET 10
* Onion Architecture
* Repository Pattern
* Unit of Work
* Cookie Authentication
* Role-Based Authorization
* Entity Framework Core
* LINQ
* SOLID Principles
* Clean Code
* High-Performance Data Access

---

# 📌 Future Improvements

* JWT Authentication
* Docker Support
* Unit Testing
* Integration Testing
* Refresh Tokens
* Swagger Authentication
* CI/CD Pipeline

---

# 📄 License

This project is licensed under the MIT License.

---

<div align="center">

⭐ If you found this project useful, don't forget to leave a star!

</div>
