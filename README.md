# 📚 Students & Courses API

## 📌 Project Description

This project is a backend API built using **Node.js**, **Express**, and **Sequelize** with **MySQL** database.
It demonstrates the use of models, relationships, and full CRUD operations.

The system manages:

* Students
* Courses
* Enrollments (Many-to-Many relationship)

---

## 🛠️ Technologies Used

* Node.js
* Express.js
* Sequelize ORM
* MySQL
* Sequelize CLI

---

## 🗄️ Database Configuration

The project uses MySQL with the following configuration:

* **Database Name:** waseem_web2
* **Username:** root
* **Password:** waseemxd12
* **Dialect:** mysql

Make sure your MySQL server is running before starting the project.

---

## ⚙️ Setup Instructions

### 1. Install dependencies

```bash
npm install
```

### 2. Create database

```bash
npx sequelize db:create
```

### 3. Run migrations

```bash
npx sequelize db:migrate
```

### 4. Start the server

```bash
npm start
```

Server will run on:

```
http://localhost:5000
```

---

## 🔗 API Endpoints

### 👨‍🎓 Students

* **GET /students** → Get all students
* **GET /students/:id** → Get student by ID
* **POST /students** → Create new student
* **PUT /students/:id** → Update student
* **DELETE /students/:id** → Delete student

---

### 📘 Courses

* **GET /courses** → Get all courses
* **GET /courses/:id** → Get course by ID
* **POST /courses** → Create new course
* **PUT /courses/:id** → Update course
* **DELETE /courses/:id** → Delete course

---

### 🔗 Enrollments

* **GET /enrollments** → Get all enrollments
* **POST /enrollments** → Enroll a student in a course
* **DELETE /enrollments/:id** → Remove enrollment

---

## 🧩 Relationships

* A **Student** can enroll in many **Courses**
* A **Course** can have many **Students**
* This is implemented using a **Many-to-Many relationship** through the Enrollment table

---

## 📬 Sample Request (POST Student)

```json
{
  "name": "Waseem",
  "email": "waseem@example.com"
}
```

---

## 📬 Sample Request (POST Enrollment)

```json
{
  "studentId": 1,
  "courseId": 2
}
```

---

## 🚀 How to Test

You can test the API using:

* Postman
* Thunder Client
* Browser (for GET requests)

---

## 📁 Project Structure

```
project/
│── config/
│── controllers/
│── migrations/
│── models/
│── routes/
│── app.js
│── package.json
```

---

## ✅ Features

* Full CRUD operations
* MySQL database integration
* Sequelize ORM with migrations
* Organized MVC structure
* Many-to-Many relationships

---

## 👨‍💻 Author

Waseem Mohammed
