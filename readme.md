# Employee Management System (Spring Framework)

## 📌 Overview

This is a simple **Employee Management System** built using the **Spring Framework (Core + Dependency Injection)**.
It demonstrates how to use **Component Scanning**, **Autowired Dependency Injection**, and **Layered Architecture**.

---

## 🏗️ Project Structure

```
com.employee
│
├── model
│   └── Employee.java
│
├── repository
│   └── EmployeeRepository.java
│
├── service
│   └── EmployeeService.java
│
├── main
│   └── MainApp.java
│
└── beans.xml
```

---

## ⚙️ Technologies Used

* Java
* Spring Framework (Core)
* XML Configuration
* Maven (optional)

---

## 🔍 Features

* Add Employee
* View All Employees
* Uses **Spring Dependency Injection**
* Follows **Layered Architecture (Repository → Service → Main)**

---

## 📂 Explanation of Components

### 🧩 EmployeeRepository

* Stores employee data in a list
* Provides methods to:

  * Add employee
  * Retrieve all employees

---

### 🧩 EmployeeService

* Handles business logic
* Uses `@Autowired` to inject repository
* Methods:

  * `createEmployee()` → Adds employee
  * `displayEmployees()` → Prints employee details

---

### 🧩 beans.xml

* Configures Spring container
* Enables component scanning:

```
<context:component-scan base-package="com.employee"/>
```

---

### 🧩 MainApp

* Entry point of application
* Loads Spring container
* Calls service methods

---

## ▶️ How to Run

1. Clone the repository

```
git clone https://github.com/your-username/your-repo-name.git
```

2. Open project in IDE (Eclipse/IntelliJ)

3. Run:

```
MainApp.java
```

---

## ✅ Sample Output

```
101 Arun IT
102 Priya HR
```

---

## 💡 Key Concepts Covered

* Spring IoC Container
* Dependency Injection (@Autowired)
* Component Annotation (@Component)
* XML-based configuration

---

## 📌 Author

* Your Name

---

## ⭐ Notes

This is a beginner-friendly project to understand **Spring Core concepts**.
