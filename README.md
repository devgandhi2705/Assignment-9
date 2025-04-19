# PIJ-Assignment-9 (MySQL-JDBC)

## Overview
This project is a Java console-based application to manage student data using JDBC and MySQL.

## Functionalities
- Add Student - Create new student records
- Display All Students - View a list of all registered students
- Search Student by PRN - Find specific student using PRN identifier
- Search Student by Name - Locate students by their name
- Update Student - Modify existing student information
- Delete Student - Remove student records from the database

## Setup
1. Install MySQL and create the `studentdb` database with the following table:

```sql
CREATE DATABASE IF NOT EXISTS studentdb;
USE studentdb;
CREATE TABLE IF NOT EXISTS students (
    prn VARCHAR(20) PRIMARY KEY,
    name VARCHAR(100),
    dept VARCHAR(100)
);
```

2. Update your MySQL username and password in `DBConnection.java`.

3. Compile and run `Main.java` from the `src/` folder.
