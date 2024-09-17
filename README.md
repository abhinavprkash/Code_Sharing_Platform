
# Code Sharing Platform

A web-based application that allows users to share and view code snippets. Users can post code snippets, browse existing ones, and retrieve them via a secure mechanism. The platform includes secret snippets and a feed for recent code uploads.

## Features

- **POST Updates**: Allows users to upload code snippets.
- **View Code**: Users can browse and view previously uploaded code snippets.
- **Snippets Feed**: Displays a feed of recent code uploads.
- **Super Secret Snippets**: Manages secure and private snippets that are accessible only through special permissions.
- **Database Integration**: Utilizes an embedded database (H2) to store and manage code snippets.

## Tech Stack

- **Java**: Primary language for back-end development.
- **Spring Boot**: Used for setting up the web server and handling the API requests.
- **Gradle**: For building and managing dependencies.
- **H2 Database**: Lightweight, embedded database for storing code snippets.
- **HTML/CSS**: For frontend views and interaction.
- **Framer Motion**: Integrated for animations and UI effects.

## Prerequisites

- **Java Development Kit (JDK)** (version 11 or higher)
- **Gradle** (comes with the project setup)
- **An IDE** (e.g., IntelliJ IDEA, Eclipse) to run the project
- **Git** (optional, for version control)

## Installation Guide

### 1. Clone the Repository

```bash
git clone <repository-url>
cd Code_Sharing_Platform
```

### 2. Build the Project

This project uses **Gradle** as its build tool. You can build the project using the following command:

For UNIX-based systems:
```bash
./gradlew build
```

For Windows:
```bash
gradlew.bat build
```

### 3. Run the Application

Once the project is built, you can run it locally.

For UNIX-based systems:
```bash
./gradlew bootRun
```

For Windows:
```bash
gradlew.bat bootRun
```

### 4. Access the Application

Once the application is running, you can access it at:

```
http://localhost:8080/
```

Use your browser to navigate to this address, where you'll be able to interact with the platform (view and post snippets, browse the feed, etc.).

### 5. Database Configuration

The project uses an embedded **H2 database** (`snippets.mv.db`). You can access the H2 console via:

```
http://localhost:8080/h2-console
```

- **JDBC URL**: `jdbc:h2:~/snippets`
- **Username**: `sa`
- **Password**: *(Leave empty)*

This allows you to manage the data directly in the embedded database.

## Folder Structure

- **POST updates**: Contains code for posting new snippets.
- **Show the code_**: Handles the display logic for showing snippets.
- **Snippets feed**: Code for managing and displaying the feed of recent snippets.
- **Super secret snippets**: Manages snippets with special permissions.
- **Work with the database**: Includes database interaction logic (CRUD operations on snippets).
- **task**: Contains tasks for handling specific user operations.

## Contributing

1. Fork the repository.
2. Create a new feature branch (`git checkout -b feature/feature-name`).
3. Commit your changes (`git commit -m 'Add feature'`).
4. Push to the branch (`git push origin feature/feature-name`).
5. Create a new Pull Request.

## License

This project is licensed under the MIT License.
