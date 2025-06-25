# 🎓 Student Management System – Spring Boot + MongoDB

A backend REST API project built using **Spring Boot** and **MongoDB** for managing student records. This system enables educational institutions or admins to perform Create, Read, Update, Delete (CRUD), and Search operations for students using roll number or ID.

---

## 🔧 Tech Stack

- **Java 8+**
- **Spring Boot 2.7.18**
- **MongoDB**
- **Spring Web**
- **Spring Data MongoDB**
- **Maven**

---

## 🚀 Features

- 📥 Add student data
- 📃 View all student records
- 🔍 Search by roll number or ID
- ✏️ Update student using roll number (partial update supported)
- ❌ Delete student by ID

---

## 📂 Project Structure

Student-Management-System/
├── controller/ → REST API endpoints
├── service/ → Business logic layer
├── repository/ → MongoDB repository interface
├── student_details/ → Model class (student schema)
├── application.properties → MongoDB & app config
└── StudentManagementSystemApplication.java → Main class

---


---

## 📮 API Endpoints

| Method | Endpoint                  | Description                        |
|--------|---------------------------|------------------------------------|
| POST   | `/student`                | Add new student                    |
| GET    | `/student`                | Get all students                   |
| GET    | `/student/findByRoll/{r}` | Get student by roll number         |
| GET    | `/student/findById/{id}`  | Get student by MongoDB ObjectId    |
| PUT    | `/student/updateByRoll/{r}`| Update student fields by roll      |
| DELETE | `/student/deleteById/{id}`| Delete student by ObjectId         |

---

## 🧪 Sample Student JSON

```json
{
  "name": "Ravi Kumar",
  "age": 20,
  "dept": "Computer Science",
  "email": "ravi.kumar@example.com",
  "phone": "9876543210",
  "address": "Durgapur, West Bengal",
  "roll": "CS2025007"
}

---

🛠 Future Enhancements
✅ Add input validation and custom error messages

🔐 Integrate Spring Security and JWT for authentication

🌐 Connect a React or Angular frontend

📑 Add Swagger for live API documentation
