# https-github.com-YOUR_USERNAME-library-management-system
library management systems
# 📚 Library Management System

A comprehensive desktop application for managing library operations built with **JavaFX**, **MySQL**, and **Maven**.

![Java](https://img.shields.io/badge/Java-21-orange)
![JavaFX](https://img.shields.io/badge/JavaFX-21-blue)
![MySQL](https://img.shields.io/badge/MySQL-8.0-lightgrey)
![Maven](https://img.shields.io/badge/Maven-3.9-red)

## ✨ Features

### 👥 Member Management
- Add new library members
- View all members in a table
- Update member details
- Delete member records
- Search members by ID or name

### 📖 Book Management
- Add new books to catalog
- Update book information
- Track book quantity
- Search books by title, author, or ISBN

### 📝 Issue & Return
- Issue books to members
- Return books with automatic fine calculation
- Track due dates
- View issued books history

### 📊 Reports & Analytics
- View available books
- Check overdue books
- Member borrowing history
- Most borrowed books

## 🛠️ Technologies Used

| Technology | Version | Purpose |
|------------|---------|---------|
| Java | 21 | Core programming |
| JavaFX | 21 | GUI framework |
| MySQL | 8.0 | Database |
| Maven | 3.9+ | Build automation |
| JDBC | 8.0 | Database connectivity |

## 📋 Prerequisites

Before running this project, make sure you have:

- ✅ **Java JDK 21** or higher
- ✅ **Maven 3.9** or higher
- ✅ **MySQL 8.0** or higher
- ✅ **IntelliJ IDEA** (recommended) or Eclipse

## 🚀 Installation & Setup

### 1. Clone the Repository

```bash
git clone [https://github.com/YOUR_USERNAME/library-management-system.git](https://github.com/YOUR_USERNAME/library-management-system.git)
cd library-management-system
```

### 2. Set Up Database

1. Open MySQL command line or MySQL Workbench
2. Create the database:

```sql
CREATE DATABASE LibraryManagement;
USE LibraryManagement;
```

3. Run the SQL script to create tables (see `database/schema.sql`)

### 3. Configure Database Connection

Open `src/main/java/com/library/database/DatabaseConnection.java` and update:

```java
private static final String URL = "jdbc:mysql://localhost:3306/LibraryManagement";
