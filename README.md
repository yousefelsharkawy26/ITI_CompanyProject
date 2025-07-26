# 🏢 ITI Company Project

## 📘 Overview
This is a simple .NET-based company management system built as part of an ITI educational project.  
The system manages three core entities:
- **Departments**  
- **Employees**  
- **Projects**

It's designed to demonstrate entity relationships and basic CRUD operations without authentication.

---

## 🧱 Technology Stack
- **Language**: C#
- **Framework**: ASP.NET Core MVC (.NET 6+)
- **ORM**: Entity Framework Core
- **Database**: SQL Server
- **IDE**: Visual Studio 2022 (recommended)

---

## 🧩 Core Features

- **Departments**
  - Each department contains multiple employees.

- **Employees**
  - Each employee belongs to one department.
  - An employee can work on one or more projects.

- **Projects**
  - Projects can have multiple employees assigned.

> The relationships implemented are:
- One-to-many: Department → Employees  
- Many-to-many: Employees ↔ Projects (via a join table)

---

## 🚀 Getting Started

### Prerequisites
- [.NET SDK 6.0 or later](https://dotnet.microsoft.com/en-us/download)
- [SQL Server](https://www.microsoft.com/en-us/sql-server/)
- Visual Studio (or any preferred IDE)

### Steps to Run Locally

```bash
# 1. Clone the repository
git clone https://github.com/yousefelsharkawy26/ITI_CompanyProject.git
cd ITI_CompanyProject

# 2. Open the solution in Visual Studio

# 3. Update the database connection string in appsettings.json

# 4. Apply EF Core Migrations (if not already done)
Tools > NuGet Package Manager > Package Manager Console
> Update-Database

# 5. Run the project (Ctrl + F5)
