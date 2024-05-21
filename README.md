# Library Management System

## Overview

This project is a Library Management System built using ASP.NET Core 6. It allows users to manage book categories and books within those categories. The system supports CRUD (Create, Read, Update, Delete) operations for both categories and books. The repository includes both frontend and backend components.

## Features

- Add, view, update, and delete book categories.
- Add, view, update, and delete books within categories.
- User-friendly interface to manage the library efficiently.

## Technologies Used

- ASP.NET Core 6
- Entity Framework Core
- Razor Pages or Blazor (specify if applicable)
- SQL Server (or any other database you are using)
- HTML, CSS, JavaScript (for frontend)

## Prerequisites

- [.NET 6 SDK](https://dotnet.microsoft.com/download/dotnet/6.0)
- SQL Server (or your preferred database)
- IDE (Visual Studio, Visual Studio Code, or any other preferred IDE)

## Setup Instructions

### Backend Setup

1. **Clone the Repository**
   ```bash
   git clone [https://github.com/yourusername/LibraryManagementSystem.git](https://github.com/alphaket14/asp-dotnet-booklib.git)
   cd library-master
   ```

2. **Configure Database**
   - Open `appsettings.json` in the project directory.
   - Update the connection string to point to your SQL Server instance.

   ```json
   "ConnectionStrings": {
     "DefaultConnection": "Server=your_server;Database=LibraryDB;User Id=your_user;Password=your_password;"
   }
   ```

3. **Apply Migrations and Create Database**
   Open the terminal in the project directory and run the following commands:

   ```bash
   dotnet ef migrations add InitialCreate
   dotnet ef database update
   ```

4. **Run the Application**
   ```bash
   dotnet run
   ```

   The backend will be available at `https://localhost:5001` or `http://localhost:5000`.

### Frontend Setup

- If the frontend is a separate project, navigate to the frontend directory and follow similar steps to set it up.
- Ensure that the frontend is configured to communicate with the backend API endpoints.

## Usage

### Adding a Category

1. Navigate to the Categories section.
2. Click on "Add New Category".
3. Enter the category name and save.

### Adding a Book

1. Navigate to the Books section.
2. Click on "Add New Book".
3. Select the category from the dropdown list.
4. Enter the book name and other details, then save.

### Viewing, Updating, and Deleting

- To view, update, or delete categories or books, use the respective options provided in the UI.

## Contributing

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Commit your changes (`git commit -am 'Add some feature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Open a Pull Request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For any inquiries or feedback, please contact [somaksomanchi1krishna@gmail.com].

---

Thank you for using the Library Management System. We hope it serves your needs well!
