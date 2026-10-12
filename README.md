Video: https://drive.google.com/REPLACE_WITH_YOUR_LINK

# Task 1 — Simple Database CRUD Operations

Console application (C# / Npgsql) connected to PostgreSQL that performs Create, Read, Update and Delete on a `Student` table.

## Requirements
- .NET 8 SDK (or newer)
- PostgreSQL running locally
- Npgsql package

## Setup
1. Create an empty database in PostgreSQL (e.g. `studentdb`).
2. Edit the connection settings in `Program.cs` (`Username`, `Password`, `Database`).
3. Install the dependency and run:
   ```
   dotnet add package Npgsql
   dotnet run
   ```
4. The `Student` table is created automatically by the application on startup.

## Features
- Add / View / Update / Delete students by `Id`
- All queries are parameterized (`@name`, `@age`, `@gpa`, `@id`) — no string concatenation of user input
- Each command prints the SQL it runs, to show what happens in the background
