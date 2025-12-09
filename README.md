# 📚 MySQL Basics – Beginner Friendly Learning Repository  

This repository contains my learning notes, SQL examples and explanations from my **MySQL Basics** practice. It includes core database concepts, SQL commands, constraints, filtering, and aggregate functions used in data analytics and application development.  

---

## 📌 Overview  

MySQL is one of the most widely used relational database systems for storing and managing structured data. Through this learning journey, I practiced how to create databases, insert data, modify records, add constraints, and generate insights using SQL queries.

This repository demonstrates:
- foundational SQL knowledge  
- hands-on MySQL usage  
- database understanding  
- beginner-friendly examples  

---

## 📘 Topics Covered  

### 🔹 1. Introduction to Data & Databases  
- What is Data  
- What is a Database  
- RDBMS  
- SQL definition  
- What is MySQL  

### 🔹 2. Database Operations  
- Create Database  
- List Databases  
- Use Database  
- Delete Database  

### 🔹 3. CRUD Operations  
- INSERT  
- SELECT  
- UPDATE  
- DELETE  

---

## 📊 MySQL Data Types  

| Category | Example |
|---|---|
| integer | INT |
| decimal | DECIMAL(10,2) |
| boolean | BOOLEAN |
| char | CHAR(10) |
| varchar | VARCHAR(100) |
| text | TEXT |
| date | DATE |
| time | TIME |
| datetime | DATETIME |
| binary | BLOB |

---

## 🔐 MySQL Constraints  

- NOT NULL  
- UNIQUE  
- PRIMARY KEY  
- FOREIGN KEY  
- CHECK  
- DEFAULT  
- INDEX  

Used to ensure:
- data validity  
- accuracy  
- integrity  

---

## 🔎 Filtering Clauses  

- WHERE  
- ORDER BY  
- LIMIT  
- LIKE  
- BETWEEN  
- DISTINCT  

---

## 🧮 Aggregate Functions  

- COUNT()  
- SUM()  
- AVG()  
- MIN()  
- MAX()  
- GROUP_CONCAT()  

---

## 🎓 Sample Student Table (With All Constraints)

```sql
CREATE DATABASE studentdb;
USE studentdb;

CREATE TABLE students (
    student_id INT PRIMARY KEY AUTO_INCREMENT,
    student_name VARCHAR(100) NOT NULL,
    email VARCHAR(150) UNIQUE,
    city VARCHAR(50) DEFAULT 'Not Assigned',
    age INT CHECK (age >= 5)
);

CREATE TABLE courses (
    course_id INT PRIMARY KEY AUTO_INCREMENT,
    student_id INT NOT NULL,
    course_name VARCHAR(100) NOT NULL,
    start_date DATE NOT NULL,
    fee DECIMAL(10,2) DEFAULT 0,
    CONSTRAINT fk_student
        FOREIGN KEY(student_id)
        REFERENCES students(student_id)
);
```
## 🎯 Skills Gained  

- SQL Basics  
- Data Querying  
- Table Designing  
- Data Types  
- Constraints  
- Using WHERE & LIKE  
- Aggregate Functions  
- Understanding business insights  

---

## 💡 Why Learn SQL?  

SQL is a must-have skill for:

- Data Analytics  
- Data Science  
- Business Analytics  
- Backend Development  
- Database Administration  

SQL helps retrieve data, clean data, and generate data-based insights.

---

## 🔧 Tools Used  

- MySQL Workbench  
- MySQL Server  

---

## 👨‍💻 Author  

**Manas Ranjan Patra**  
Data Analytics Enthusiast | Learning SQL, Python & Analytics 

---

## ⭐ Support  

If you like this repo, please give it a ⭐ on GitHub 😊  

---

## 🤝 Connect  

Happy to connect with other learners & professionals working on analytics and SQL!  
