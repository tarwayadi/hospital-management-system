Hospital Management System
This is a beginner-friendly backend application for a Hospital Management System developed using Java and JDBC. The project demonstrates fundamental concepts of database connectivity and object-oriented programming by managing patient, doctor, and appointment data.

Key Features
 1. Patient Management: Add new patients and view existing patient details.
 2. Doctor Management: View a list of available doctors.
 3. Appointment Scheduling: Book new appointments for patients with doctors.
 4. Data Persistence: All data is stored in a MySQL database.

Technologies Used
 1. Java: The core programming language for the application logic.
 2. JDBC (Java Database Connectivity): Used to connect the Java application to the MySQL database.
 3.MySQL: The relational database used to store all patient, doctor, and appointment data.

Prerequisites
 1. To run this project, you need to have the following installed on your system:
 2. Java Development Kit (JDK) 8 or higher
 3. MySQL Server
 4. MySQL JDBC Driver: You will need to download and include this in your project's build path.

Getting Started
Follow these steps to set up and run the project locally.

1. Clone the Repository
Bash
git clone https://github.com/prabhatthakuryt/Hospital-Management-System.git
cd Hospital-Management-System

2. Set Up the Database
    1. Open your MySQL client (e.g., MySQL Workbench or command line).
    2. Create a new database named hospital_management.

          SQL
          CREATE DATABASE hospital_management;
    3. Select the new database and create the required tables.
          SQL
          USE hospital_management;

         CREATE TABLE doctors (
         id INT PRIMARY KEY AUTO_INCREMENT,
         name VARCHAR(255) NOT NULL,
         specialization VARCHAR(255) NOT NULL
        );

        CREATE TABLE patients (
        id INT PRIMARY KEY AUTO_INCREMENT,
        name VARCHAR(255) NOT NULL,
        age INT NOT NULL,
        gender VARCHAR(10) NOT NULL
        );
3. Configure Database Connection
   1. Open the project in your favorite IDE (e.g., IntelliJ IDEA, Eclipse).
   2. Locate the database connection class (e.g., DatabaseConnection.java).
   3.Update the url, username, and password variables to match your MySQL server configuration.

4. Run the Application
   Execute the Main.java or HospitalManagementSystem.java file to run the main application. You will be presented with a command-line interface to interact with the system.

5. Usage
   Once the application is running, you can follow the on-screen menu to perform operations such as:
   Adding a new patient.
   Viewing available doctors.
   Booking a new appointment.







