<div align="center">

# 🚀 XBLogProject

### Modern Blog, Project & Task Management System

Built with **ASP.NET Core MVC**, **Web API**, **Entity Framework Core**, and **Onion Architecture**

![.NET](https://img.shields.io/badge/.NET-10-512BD4?style=for-the-badge&logo=dotnet)
![ASP.NET Core](https://img.shields.io/badge/ASP.NET_Core-10-5C2D91?style=for-the-badge&logo=dotnet)
![C#](https://img.shields.io/badge/C%23-14-239120?style=for-the-badge&logo=c-sharp)
![EF Core](https://img.shields.io/badge/Entity_Framework_Core-512BD4?style=for-the-badge)
![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=for-the-badge\&logo=microsoftsqlserver)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

*A clean, scalable, and production-ready application demonstrating modern ASP.NET Core development practices.*

</div>

---

# 📖 Overview

XBLogProject is a full-stack ASP.NET Core application that combines a blogging platform with project and task management capabilities.

The project was developed with a strong focus on **Clean Architecture**, **maintainability**, **performance**, and **security**, following industry-standard software engineering principles.

---

# ✨ Features

## 🔐 Authentication & Authorization

* Cookie-Based Authentication
* Secure Login & Logout
* Role-Based Authorization
* Access Control
* Persistent Authentication Cookies

---

## 👤 User Management

* User Registration
* User Login
* User Profiles
* Role Management

### Dynamic Admin Permission Management

An administrator can:

* Grant the **Admin** role to another user.
* Revoke the **Admin** role from existing administrators.

This functionality is fully managed within the application without requiring direct database modifications.

---

## 📝 Blog Module

* Create Articles
* Edit Articles
* Delete Articles
* Article Details
* Comment System

---

## 📁 Project Management

* Create Projects
* Edit Projects
* Soft Delete
* Restore Deleted Projects
* Project Status Management

### 🤖 Automatic Project Completion

When **all tasks belonging to a project are marked as Completed**, the project is **automatically updated** to the **Completed** status.

This business rule is handled inside the application layer to ensure data consistency.

---

## ✅ Task Management

* Create Tasks
* Assign Tasks to Users
* Pending
* In Progress
* Completed
* Rejected
* Canceled
* Soft Delete
* Restore Deleted Tasks

---

# 🏛️ Software Architecture

The project follows the **Onion Architecture**, separating responsibilities into independent layers.

```text
                 Presentation
          (MVC + Web API)

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

# 🌐 REST API

The solution includes a RESTful Web API that shares the same business logic as the MVC application.

The API is designed for future integration with mobile applications, frontend frameworks, or third-party services.

---

# ⚡ Performance Considerations

The project follows several Entity Framework Core best practices:

* Async database operations
* AsNoTracking() for read-only queries
* Optimized LINQ expressions
* Filtered Include
* Soft Delete implementation
* Efficient Change Tracking
* Reduced unnecessary memory allocations
* Clean separation between read and write operations

---

# 🛠️ Technologies

| Backend              | Database              | Frontend    | Architecture       |
| -------------------- | --------------------- | ----------- | ------------------ |
| ASP.NET Core MVC     | SQL Server            | Bootstrap 5 | Onion Architecture |
| ASP.NET Core Web API | Entity Framework Core | HTML5       | Repository Pattern |
| C#                   | LINQ                  | CSS3        | Unit of Work       |
| Dependency Injection |                       | JavaScript  | Service Layer      |

---

# 📂 Solution Structure

```text
XBLogProject

├── XBLog.Web
│
├── XBLog.API
│
├── XBLog.Application
│
├── XBLog.Domain
│
└── XBLog.Infrastructure
```

---

# 🚀 Getting Started

## Clone Repository

```bash
git clone https://github.com/your-username/XBLogProject.git
```

## Restore Packages

```bash
dotnet restore
```

## Update Database

```bash
dotnet ef database update
```

## Run Application

```bash
dotnet run
```

---

# 📸 Screenshots

> Add screenshots here

* Login
* Dashboard
* Blog
* Projects
* Tasks
* Admin Panel

---

# 🎯 What This Project Demonstrates

* ASP.NET Core MVC
* ASP.NET Core Web API
* Onion Architecture
* Repository Pattern
* Unit of Work
* Entity Framework Core
* Cookie Authentication
* Role-Based Authorization
* SOLID Principles
* Clean Code
* LINQ Optimization
* Performance-Oriented Data Access

---

# 🚧 Future Improvements

* JWT Authentication
* Refresh Token Support
* Docker
* Unit Testing
* Integration Testing
* Email Verification
* File Upload
* Real-Time Notifications (SignalR)

---

# 📄 License

This project is licensed under the MIT License.

---

<div align="center">

### ⭐ If you like this project, don't forget to leave a Star!

</div>
