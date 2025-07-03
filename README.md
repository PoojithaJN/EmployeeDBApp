# EmployeeDBApp

A simple **Java Console Application** using **JDBC** to perform CRUD (Create, Read, Update, Delete) operations on an **Employees** table in a **MySQL database**.

## Objective

To build a menu-driven employee management system that allows:
- Adding new employees  
- Viewing all employee records  
- Updating employee email  
- Deleting employees by ID  

## Tools & Technologies Used

- **Java (JDK 24)**
- **JDBC (Java Database Connectivity)**
- **MySQL Database**
- **Eclipse IDE**
- **MySQL Connector/J (JDBC Driver)**

## Key Concepts Used

- **JDBC API** for database connectivity
- **DriverManager** to establish a database connection
- **Connection, Statement, PreparedStatement** for executing SQL queries
- **ResultSet** for handling SQL query results
- **Try-with-resources** for automatic resource management
- **Console input** using `Scanner`
- **Menu-driven program** using `while` loop and `switch-case`
- **Exception handling** with `try-catch`

## 🚦 How to Run

1. **Create the Database:**
   - Open MySQL Workbench or CLI.
   - Run this SQL:
     ```sql
     CREATE DATABASE testdb;
     USE testdb;

     CREATE TABLE employees (
         id INT PRIMARY KEY AUTO_INCREMENT,
         name VARCHAR(100),
         email VARCHAR(100),
         salary DOUBLE
     );
     ```
2. **Open Eclipse IDE.**
3. **Create a New Java Project** ( `Task7`).
4. **Add a Class named `EmployeeDBApp`** and write the Java code.
5. **Download MySQL JDBC Driver**  
   - https://dev.mysql.com/downloads/connector/j/  
   - Add the `.jar` file to your project via **Build Path > Add External JARs**.
6. **Update MySQL credentials** in the code:
   ```java
   static final String DB_URL = "jdbc:mysql://localhost:3306/testdb";
   static final String DB_USER = "root";
   static final String DB_PASS = "your_password";
7. **Run the Program:**
   - In Eclipse, right-click on `EmployeeDBApp.java`.
   - Select **Run As > Java Application**.
