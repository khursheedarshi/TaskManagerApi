# TaskManagerApi
Task Manager API
This is a basic web-based task-tracking application built using C# .NET Core for the backend and ReactJS for the frontend. The application allows users to add tasks, set due dates, and mark tasks as completed
## Setup Instructions

### Backend (C# .NET Core)

1. Open the `TaskManagerApi` directory in the terminal.

2. Install necessary NuGet packages:
   ```bash
   dotnet add package Npgsql.EntityFrameworkCore.PostgreSQL -v 3.1.4
   dotnet add package Microsoft.EntityFrameworkCore.PostgreSQL -v 12.0
   dotnet add package Microsoft.EntityFrameworkCore.Design -v 3.1
   dotnet add package Microsoft.EntityFrameworkCore.Tools -v 3.1

   Configure the database connection in appsettings.json:
   {
    "ConnectionStrings": {
        "DefaultConnection": "Host=localhost;Port=5432;Database=TaskManagerDb;Username=<username>;Password=<password>"
    },
    "Logging": {
        // ...
    },
    // ...
}
