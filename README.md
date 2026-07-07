🚀 TaskFlow - Task Management System API

<p align="center"> A modern Task Management RESTful API built with <b>ASP.NET Core Web API</b> following the <b>Onion Architecture</b> principles. </p>

<p align="center">








</p>

📖 Overview

TaskFlow is a portfolio project developed with ASP.NET Core Web API using Onion Architecture.

The system is designed to help organizations manage projects and tasks efficiently.

Administrators can create projects, assign tasks to registered users, monitor progress, and track project completion. Users can authenticate, view assigned tasks, and update task statuses.

When all tasks belonging to a project are completed, the system automatically marks the project as completed.

This project demonstrates practical experience in ASP.NET Core Web API, Onion Architecture, Entity Framework Core, Repository Pattern, Unit of Work Pattern, Cookie Authentication, and RESTful API design.

✨ Features
🔐 Cookie-Based Authentication
👤 User Registration & Login
🛡️ Role-Based Authorization
📁 Project Management
📋 Task Management
👥 Task Assignment
♻️ Soft Delete & Restore
✅ Automatic Project Completion
🏗️ Onion Architecture
💾 SQL Server Database
⚡ Entity Framework Core
📄 Swagger Documentation
🔄 Unit Of Work Pattern
🧩 Repository Pattern
🏛️ Architecture

The project follows the Onion Architecture pattern to achieve maintainability, scalability, and separation of concerns.

Project Layers
API
Controllers
Middleware
Authentication Configuration
Swagger
Application
Services
DTOs
Contracts
Business Rules
Domain
Entities
Enums
Interfaces
Core Models
Infrastructure
Entity Framework Core
SQL Server
Repositories
Unit Of Work
Data Access Layer
📊 Business Workflow
Admin
 │
 ├── Create Project
 │
 ├── Assign Tasks
 │
 └── Manage Users

User
 │
 ├── Login
 │
 ├── View Assigned Tasks
 │
 └── Complete Tasks

System
 │
 └── Automatically Completes Project
     When All Tasks Are Completed
🗄️ Entity Relationships
User
 │
 └───────< TaskItem >─────── Project
Relationship Summary
One User → Many Tasks
One Project → Many Tasks
Each Task → One User
Each Task → One Project
No Direct Relationship Between User And Project
📸 API Documentation

Swagger/OpenAPI is integrated for testing and exploring all endpoints.

Main Endpoints
Authentication
POST /api/auth/register
POST /api/auth/login
POST /api/auth/logout
Projects
GET    /api/projects
GET    /api/projects/{id}
POST   /api/projects
PUT    /api/projects/{id}
DELETE /api/projects/{id}
PATCH  /api/projects/{id}/restore
Tasks
GET    /api/tasks
GET    /api/tasks/{id}
POST   /api/tasks
PUT    /api/tasks/{id}
DELETE /api/tasks/{id}
PATCH  /api/tasks/{id}/restore
PATCH  /api/tasks/{id}/complete
🛠️ Technologies
ASP.NET Core Web API
C#
Entity Framework Core
Microsoft SQL Server
Cookie Authentication
Swagger / OpenAPI
Onion Architecture
Repository Pattern
Unit Of Work Pattern
LINQ
Dependency Injection
📂 Project Structure
TaskFlow
│
├── TaskFlow.API
├── TaskFlow.Infrastructure
├── TaskFlow.Application
└── TaskFlow.Domain
🚀 Getting Started
Clone Repository
git clone https://github.com/your-username/TaskFlow.git
Navigate To Project
cd TaskFlow
Configure Database

Update your SQL Server connection string inside:

appsettings.json
Apply Migrations
dotnet ef database update
Run Application
dotnet run
💡 Skills Demonstrated
ASP.NET Core Web API
Onion Architecture
Repository Pattern
Unit Of Work Pattern
Entity Framework Core
SQL Server
Cookie Authentication
Role-Based Authorization
RESTful API Design
Dependency Injection
Clean Code Principles
📌 Future Improvements
JWT Authentication
Refresh Tokens
Pagination
Search & Filtering
AutoMapper
CQRS Pattern
Unit Testing
Integration Testing
Docker Support
Serilog Logging
📄 License

This project is available under the MIT License.
