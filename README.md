# Auto TimeTable Generator

## Overview
Auto TimeTable Generator is a Windows Forms Application developed in C# .NET that automatically schedules and generates time tables for schools, colleges, or universities. It manages various constraints like subjects, teachers, time slots, and classes to produce conflict-free timetables efficiently.

## Features
- Manages class, program, and semester configurations.
- Handles teacher and lecture subject allocations.
- Sets time slots for lectures.
- Uses MSSQL server for robust database management.
- User-friendly Windows Forms graphical interface.
- Automatically generates time tables avoiding overlaps and conflicts.
- Generates descriptive reports and time table representations.

## Technologies Used
- **Language**: C#
- **Framework**: .NET Framework
- **UI Framework**: Windows Forms (WinForms)
- **Database**: Microsoft SQL Server (MSSQL)

## Repository Structure
- **/AutoTimeTableGenerator**: Contains the C# Windows Forms application source code (`.sln` and `.csproj` files).
- **/Database**: Contains SQL scripts (`Database Script with Data.sql`) and database files (`AutoTimeTableDb.mdf`, `AutoTimeTableDb_log.LDF`) to set up the default MSSQL database.
- **/img Auto Time Table**: Contains UI images and screenshots of the application.
- **Documentation**: Includes a presentation (`reasearch presentation.pptx`) and a Word document (`table generator.docx`) regarding the project details and PDF research papers.

## Setup Instructions
1. Clone the repository.
2. Open the solution file `AutoTimeTableGenerator/AutoTimeTableGenerator.sln` in Microsoft Visual Studio.
3. Attach the database or run the script in `/Database` to your local MS SQL Server instance.
4. Update the connection string located in `AutoTimeTableGenerator/TimeTableGenerator/DatabaseLayer.cs` according to your local MS SQL Server instance configurations.
   ```csharp
   conn = new SqlConnection(@"Data Source=PC;Initial Catalog=AutoTimeTableDb;Integrated Security=True");
   ```
5. Build and run the project `TimeTableGenerator` in Visual Studio.

## License
This project is open-source. Feel free to use and modify it for your specific requirements.
