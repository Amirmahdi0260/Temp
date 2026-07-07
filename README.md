<div align="center">

# 🚀 XTask

### Modern Task & Project Management System

A modern **Task Management System** built with **.NET 10**, **ASP.NET Core MVC**, **ASP.NET Core Web API**, and **Onion Architecture**.

Designed with a strong focus on **Clean Architecture**, **Scalability**, **Performance**, and **Maintainability**.

![.NET](https://img.shields.io/badge/.NET-10-512BD4?style=for-the-badge\&logo=dotnet)
![ASP.NET Core](https://img.shields.io/badge/ASP.NET_Core-10-5C2D91?style=for-the-badge\&logo=dotnet)
![C#](https://img.shields.io/badge/C%23-14-239120?style=for-the-badge\&logo=c-sharp)
![Entity Framework Core](https://img.shields.io/badge/Entity_Framework_Core-10-512BD4?style=for-the-badge)
![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=for-the-badge\&logo=microsoftsqlserver)
![License](https://img.shields.io/badge/License-MIT-success?style=for-the-badge)

</div>

---

# 📖 Overview

**XTask** is a modern task and project management application that enables teams to organize projects, assign tasks, track progress, and manage user permissions securely.

The application is built using **Onion Architecture** and follows clean software engineering principles such as **Repository Pattern**, **Unit of Work**, and **Dependency Injection**, ensuring a scalable and maintainable codebase.

---

# ✨ Features

## 🔐 Authentication & Authorization

* Cookie-Based Authentication
* Secure Login & Logout
* Role-Based Authorization
* Persistent Authentication Cookies
* Protected Routes

---

## 👥 User Management

* User Registration
* User Login
* User Profile Management
* Dynamic Role Assignment

### Administrator Permissions

Users with the **Admin** role can:

* Grant the **Admin** role to other users.
* Revoke the **Admin** role from existing administrators.

This permission is fully managed inside the application without requiring direct database changes.

---

## 📁 Project Management

* Create Projects
* Edit Projects
* Delete Projects (Soft Delete)
* Restore Deleted Projects
* Project Status Management

### 🤖 Automatic Project Completion

When every task belonging to a project is marked as **Completed**, the project status is automatically updated to **Completed**.

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
* Soft Delete
* Restore Deleted Tasks

---

## 🌐 Web API

The solution includes a RESTful Web API that shares the same business logic as the MVC application, making future integration with mobile applications or SPA frameworks straightforward.

---

# 🏛️ Architecture

The project follows the **Onion Architecture** to ensure clear separation of concerns.

```text
Presentation (MVC + Web API)
            │
      Application
            │
         Domain
            │
    Infrastructure
```

### Design Patterns

* Onion Architecture
* Repository Pattern
* Unit of Work
* Dependency Injection
* Service Layer

---

# ⚡ Performance

The project applies several Entity Framework Core best practices:

* Asynchronous database operations
* `AsNoTracking()` for read-only queries
* Optimized LINQ queries
* Soft Delete implementation
* Efficient Entity Framework Core Change Tracking
* Filtered Include queries
* Reduced unnecessary memory allocations

---

# 🛠️ Technologies

| Category       | Technologies                           |
| -------------- | -------------------------------------- |
| Framework      | .NET 10                                |
| Backend        | ASP.NET Core MVC, ASP.NET Core Web API |
| Language       | C# 14                                  |
| ORM            | Entity Framework Core 10               |
| Database       | SQL Server                             |
| Authentication | Cookie Authentication                  |
| Architecture   | Onion Architecture                     |
| Patterns       | Repository Pattern, Unit of Work       |
| Frontend       | Bootstrap 5, HTML5, CSS3, JavaScript   |

---

# 📂 Solution Structure

```text
XTask
│
├── XTask.Web
├── XTask.Api
├── XTask.Application
├── XTask.Domain
└── XTask.Infrastructure
```

---

# 🚀 Getting Started

## Prerequisites

* .NET 10 SDK
* SQL Server
* Visual Studio 2026 or Visual Studio Code

## Clone the repository

```bash
git clone https://github.com/your-username/XTask.git
```

## Restore packages

```bash
dotnet restore
```

## Apply database migrations

```bash
dotnet ef database update
```

## Run the project

```bash
dotnet run
```

---

# 📸 Screenshots

> Add screenshots of the following pages:

* Login
* Dashboard
* Project List
* Task List
* Task Details
* Admin Panel

---

# 🎯 What This Project Demonstrates

* ASP.NET Core MVC
* ASP.NET Core Web API
* .NET 10
* Onion Architecture
* Repository Pattern
* Unit of Work
* Cookie-Based Authentication
* Role-Based Authorization
* Entity Framework Core
* LINQ
* SOLID Principles
* Clean Code
* High-Performance Data Access

---

# 🚀 Future Improvements

* Email Verification
* JWT Authentication
* Refresh Tokens
* Docker Support
* SignalR Notifications
* Unit Testing
* Integration Testing

---

# 📄 License

This project is licensed under the MIT License.

---

<div align="center">

### ⭐ If you found this project useful, consider giving it a star!

</div>
