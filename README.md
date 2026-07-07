<div align="center">

# 🚀 XTask

### Modern Task Management REST API built with .NET 10

A scalable and maintainable Task Management System developed using **ASP.NET Core Web API**, **Onion Architecture**, and **Entity Framework Core**.

![.NET](https://img.shields.io/badge/.NET-10-512BD4?style=for-the-badge\&logo=dotnet)
![ASP.NET Core](https://img.shields.io/badge/ASP.NET_Core-Web_API-5C2D91?style=for-the-badge\&logo=dotnet)
![C#](https://img.shields.io/badge/C%23-14-239120?style=for-the-badge\&logo=c-sharp)
![Entity Framework Core](https://img.shields.io/badge/Entity_Framework_Core-10-512BD4?style=for-the-badge)
![Microsoft SQL Server](https://img.shields.io/badge/Microsoft_SQL_Server-CC2927?style=for-the-badge\&logo=microsoftsqlserver)
![License](https://img.shields.io/badge/License-MIT-success?style=for-the-badge)

</div>

---

# 📖 Overview

**XTask** is a modern Task Management REST API designed to simplify project organization and task tracking while following clean software architecture principles.

The project is built with **ASP.NET Core Web API** on **.NET 10**, following the **Onion Architecture** pattern to achieve scalability, maintainability, and separation of concerns.

It demonstrates modern backend development practices including **Cookie-Based Authentication**, **Role-Based Authorization**, **Repository Pattern**, **Unit of Work**, and optimized **Entity Framework Core** data access.

---

# ✨ Features

## 🔐 Authentication & Authorization

* Cookie-Based Authentication
* Secure User Login & Logout
* Role-Based Authorization
* Protected API Endpoints
* Persistent Authentication Cookies

---

## 👥 User Management

* User Registration
* User Authentication
* User Management
* Dynamic Role Management

### Administrator Permissions

Users with the **Admin** role can:

* Grant the **Admin** role to other users.
* Revoke the **Admin** role from existing administrators.

Role management is completely handled through the API without requiring direct database modifications.

---

## 📁 Project Management

* Create Projects
* Update Projects
* Soft Delete Projects
* Restore Deleted Projects
* Project Status Management

### 🤖 Automatic Project Completion

When every task belonging to a project reaches the **Completed** status, the project is automatically marked as **Completed**.

This business rule guarantees project consistency without requiring manual updates.

---

## ✅ Task Management

* Create Tasks
* Assign Tasks to Users
* Pending Status
* In Progress Status
* Completed Status
* Rejected Status
* Canceled Status
* Soft Delete Tasks
* Restore Deleted Tasks

---

## 🌐 RESTful API

The application exposes a RESTful API that can easily be integrated with:

* Web Applications
* Mobile Applications
* SPA Frameworks
* Third-party Services

---

# 🏛️ Architecture

XTask follows the **Onion Architecture** pattern to achieve clean separation between business logic and infrastructure.

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
* Unit of Work Pattern
* Dependency Injection
* Service Layer Pattern

---

# ⚡ Performance Optimizations

The project follows Entity Framework Core best practices for better performance and lower memory usage.

* Asynchronous database operations
* Optimized LINQ queries
* `AsNoTracking()` for read-only operations
* Filtered Include queries
* Soft Delete implementation
* Efficient Change Tracking
* Reduced unnecessary memory allocations
* Clean Repository implementation

---

# 🛠️ Technology Stack

| Category             | Technology                         |
| -------------------- | ---------------------------------- |
| Framework            | .NET 10                            |
| API                  | ASP.NET Core Web API               |
| Language             | C# 14                              |
| ORM                  | Entity Framework Core 10           |
| Database             | Microsoft SQL Server               |
| Authentication       | Cookie-Based Authentication        |
| Architecture         | Onion Architecture                 |
| Design Patterns      | Repository Pattern, Unit of Work   |
| Dependency Injection | Built-in .NET Dependency Injection |

---

# 📂 Solution Structure

```text
XTask

├── XTask.Api
│
├── XTask.Application
│
├── XTask.Domain
│
└── XTask.Infrastructure
```

---

# 🚀 Getting Started

## Prerequisites

* .NET 10 SDK
* Microsoft SQL Server
* Visual Studio 2026 (Recommended)

---

## Clone Repository

```bash
git clone https://github.com/your-username/XTask.git
```

---

## Restore Packages

```bash
dotnet restore
```

---

## Configure Database

Update the **Connection String** inside:

```text
appsettings.json
```

Example:

```json
"ConnectionStrings": {
  "DefaultConnection": "Server=YOUR_SERVER;Database=XTaskDb;Trusted_Connection=True;TrustServerCertificate=True;"
}
```

---

## Apply Migrations

```bash
dotnet ef database update
```

---

## Run the Application

```bash
dotnet run
```

The API will be available through the configured local URL and can be tested using **Swagger UI**.

---

# 📷 API Documentation

Swagger is enabled for testing and exploring API endpoints during development.

After running the application, navigate to:

```text
https://localhost:{PORT}/swagger
```

---

# 🎯 What This Project Demonstrates

* ASP.NET Core Web API
* .NET 10
* Onion Architecture
* Repository Pattern
* Unit of Work
* Cookie-Based Authentication
* Role-Based Authorization
* Entity Framework Core
* Microsoft SQL Server
* LINQ
* SOLID Principles
* Clean Code
* RESTful API Design
* High-Performance Data Access

---

# 🚀 Future Improvements

* JWT Authentication
* Refresh Token Support
* Docker Support
* Unit Testing
* Integration Testing
* CI/CD Pipeline
* Email Notifications
* Real-time Notifications using SignalR

---

# 🤝 Contributing

Contributions, suggestions, and improvements are welcome.

Feel free to fork the repository, open issues, or submit pull requests.

---

# 📄 License

This project is licensed under the **MIT License**.

---

<div align="center">

### ⭐ If you found this project useful, please consider giving it a star.

**Thank you for visiting XTask!**

</div>
