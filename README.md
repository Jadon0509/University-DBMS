# 🎓 University Database Management System

A web-based University Database Management System developed using Flask, MySQL, HTML, and CSS. This project provides an interface for managing university-related data including departments, courses, instructors, students, classrooms, sections, advisors, prerequisites, and time slots.

## 📌 Project Overview

The University Database Management System is designed to simplify the storage and management of academic information within a university environment. The system uses a relational database structure and provides a user-friendly web interface for inserting and managing records.

## 🚀 Features

### Classroom Management
- Add classroom information
- Prevent duplicate classroom entries

### Department Management
- Add department details
- Store building and budget information

### Course Management
- Add courses linked to departments
- Department existence validation

### Instructor Management
- Add instructor records
- Store salary and department information

### Section Management
- Manage course sections
- Classroom validation before insertion

### Teaches Management
- Assign instructors to course sections

### Student Management
- Add and manage student information

### Takes Management
- Register students for courses
- Validate student records before enrollment

### Advisor Management
- Assign faculty advisors to students

### Time Slot Management
- Manage class schedules and timings

### Prerequisite Management
- Define course prerequisites
- Validate prerequisite courses

---

## 🛠 Technologies Used

### Frontend
- HTML5
- CSS3
- JavaScript

### Backend
- Python
- Flask Framework

### Database
- MySQL

---

## 📂 Project Structure

```text
University-Database-System/
│
├── app.py
├── templates/
│   └── index.html
│
├── static/
│   └── assets
│
├── database/
│   └── university.sql
│
├── requirements.txt
├── README.md
└── .gitignore
```

---

## ⚙️ Installation Guide

### 1. Clone Repository

```bash
git clone https://github.com/your-username/University-Database-System.git
cd University-Database-System
```

### 2. Install Dependencies

```bash
pip install flask
pip install mysql-connector-python
```

or

```bash
pip install -r requirements.txt
```

### 3. Create Database

```sql
CREATE DATABASE university1;
```

Import your SQL schema into MySQL.

### 4. Configure Database Connection

Update the credentials in `app.py`:

```python
db = mysql.connector.connect(
    host="localhost",
    user="root",
    password="your_password",
    database="university1"
)
```

### 5. Run Application

```bash
python app.py
```

### 6. Open Browser

```text
http://127.0.0.1:5000
```

---

## 🗄 Database Tables

The system includes the following tables:

- classroom
- department
- course
- instructor
- section
- teaches
- student
- takes
- advisor
- time_slot
- prereq

---

## 🔗 Database Relationships

The database follows a relational model where:

- Departments contain Courses
- Instructors belong to Departments
- Students belong to Departments
- Courses can have Prerequisites
- Instructors teach Sections
- Students enroll through Takes
- Students are assigned Advisors

---

## 🎯 Learning Objectives

This project demonstrates:

- Database Design
- Relational Schema Implementation
- Foreign Key Constraints
- CRUD Operations
- Flask Web Development
- MySQL Integration
- Form Handling
- Backend Validation

---

## 📸 User Interface

The application provides a single-page interface for:

- Adding classroom records
- Managing departments
- Managing courses
- Managing instructors
- Managing students
- Assigning advisors
- Managing schedules
- Managing prerequisites

---

## 🔒 Validation Implemented

- Duplicate classroom prevention
- Department existence validation
- Student existence validation
- Prerequisite validation
- Foreign key integrity checks

---

## 👨‍💻 Author

**Harshit Singh Jadon**

University Database Management System Project

---

## 📄 License

This project is developed for educational and academic purposes.
