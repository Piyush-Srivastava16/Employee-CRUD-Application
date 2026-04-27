# 👨‍💼 Employee CRUD Application

A simple Spring Boot web application for managing employee records using CRUD operations (Create, Read, Update, Delete) with a clean MVC architecture and Thymeleaf-based UI.

This project demonstrates how to build a full-stack backend-driven web application using Spring Boot, Spring Data JPA, and Thymeleaf.

---

## 🚀 Features

- 📋 View all employees in a web interface  
- ➕ Add new employee  
- ✏️ Update existing employee details  
- ❌ Delete employee  
- 🗄️ Persistent data storage using JPA/Hibernate  
- 🌐 Server-side rendered UI using Thymeleaf  
- 🧩 Clean MVC architecture (Controller–Service–Repository)  

---

## 🛠️ Tech Stack

- Backend: Java, Spring Boot  
- Frontend: Thymeleaf, HTML  
- Database: MySQL (or any JPA-compatible DB)  
- ORM: Spring Data JPA / Hibernate  
- Architecture: MVC (Model–View–Controller)  
- Build Tool: Maven  

---

## 📁 Project Structure

com.example.employeeCrud
│
├── controller
│   └── EmployeeController.java
│
├── service
│   └── EmployeeService.java
│
├── repository
│   └── EmployeeRepository.java
│
├── model
│   └── Employee.java
│
└── EmployeeCrudApplication.java

src/main/resources
│
├── static
│   └── (CSS / JS / images if any)
│
├── templates
│   ├── index.html
│   ├── new_employee.html
│   └── update_employee.html
│
└── application.properties

---

## 🧩 Application Flow

- Controller handles HTTP requests (/, /saveEmployee, /deleteEmployee/{id})  
- Service layer processes business logic  
- Repository interacts with database  
- Thymeleaf renders views (index.html, new_employee.html, update_employee.html)  

---

## ⚙️ How to Run the Project

### 1. Clone the repository
git clone https://github.com/your-username/Employee-CRUD-Application.git

### 2. Navigate to project directory
cd Employee-CRUD-Application

### 3. Configure database in application.properties
spring.datasource.url=jdbc:mysql://localhost:3306/employee_db
spring.datasource.username=root
spring.datasource.password=your_password

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true

### 4. Run the application
mvn spring-boot:run

### 5. Open in browser
http://localhost:8080/

---

## 📡 Endpoints Overview

| URL | Method | Description |
|-----|--------|-------------|
| / | GET | View all employees |
| /showNewEmployeeForm | GET | Show add employee form |
| /saveEmployee | POST | Save employee |
| /showFormForUpdate/{id} | GET | Show update form |
| /deleteEmployee/{id} | GET | Delete employee |

---

## 🧱 Entity Structure

| Field | Type | Constraint |
|------|------|-----------|
| id | Long | Primary Key, Auto Increment |
| firstName | String | Not Null |
| lastName | String | Not Null |
| email | String | Unique, Not Null |

---

## 📌 Key Concepts Used

- Spring Boot Auto Configuration  
- Spring MVC Architecture  
- Dependency Injection (@Autowired)  
- Spring Data JPA Repository  
- Thymeleaf Template Engine  
- CRUD Operations  

---

## 📈 Future Improvements

- 🔐 Add Spring Security (Login System)  
- 📊 Pagination & Sorting  
- 🎨 UI improvements with Bootstrap/Tailwind  
- 🔍 Search functionality  
- 🌐 Convert to REST API + React frontend  

---

## 👨‍💻 Author

Piyush Srivastava  
GitHub: https://github.com/Piyush-Srivastava16  

---
