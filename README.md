🧾 Student Registration Form (Java Swing + MySQL + JDBC)
📖 Project Overview

This project is a GUI-based Student Registration System built using Java Swing for the user interface and MySQL as the backend database.
It allows users to:

Enter student details (name, age, email, course)

Validate and store them in a MySQL database via JDBC

Retrieve and view all registered students

This project demonstrates core Java, JDBC, GUI design, and database connectivity concepts — ideal for student portfolios.

🧠 Features

✅ Simple and user-friendly Swing GUI
✅ Input validation for correct data entry
✅ MySQL integration through JDBC
✅ “View Students” feature to display stored records
✅ Error handling and success popups

⚙️ Technologies Used
Component	Technology
Language	Java (JDK 8+)
GUI Framework	Java Swing
Database	MySQL
Connector	MySQL Connector/J (JDBC Driver)
🗄️ Database Setup

Open MySQL Workbench and run the following commands:

CREATE DATABASE studentdb;
USE studentdb;

CREATE TABLE students (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    age INT,
    email VARCHAR(100),
    course VARCHAR(50)
);

💻 Java Code Configuration

In your StudentRegistration.java, update the database credentials:

con = DriverManager.getConnection(
    "jdbc:mysql://localhost:3306/studentdb",
    "root",
    "your_password_here"
);


Replace "your_password_here" with your MySQL root password.

🔧 Setup Instructions

Install Java JDK (v8 or above)

Install MySQL Server & Workbench

Download JDBC Driver
👉 https://dev.mysql.com/downloads/connector/j/

Add the JAR to your project

VS Code → Terminal:

javac -cp .;"C:\path\to\mysql-connector-j-9.0.0.jar" StudentRegistration.java
java -cp .;"C:\path\to\mysql-connector-j-9.0.0.jar" StudentRegistration

🧩 Sample GUI

📸 (Add your screenshots here once you run the project)

Example layout:

+-----------------------------------+
|   Student Registration Form       |
|-----------------------------------|
| Name:    [_______________]        |
| Age:     [_______]                |
| Email:   [_______________]        |
| Course:  [_______________]        |
| [Submit]   [View Students]        |
+-----------------------------------+

✅ Example Output
✅ Student registered successfully!
📋 Registered Students:
ID: RA2411003011459, Name: AARYA C, Age: 19, Email: aarya4776@gmail.com, Course: B.Tech 

🏁 Project Status

✅ Completed and Working
🔹 Compatible with Windows, macOS, and Linux
🔹 Can be extended to include search and delete features
