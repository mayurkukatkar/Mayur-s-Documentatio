# Introduction to Framework
*(These are called fully finished products of programming like Maggi noodles or Baba noodles)*  

---

### ✅ Definition 1
A **Framework** is a special software that is built on the top of one or more technologies having the ability to generate the common logic of the application dynamically and makes the programmers write only application-specific logic.

### ✅ Definition 2  
A **Framework** is a special software that provides abstraction on one or more technologies to simplify the application development process.

---

### 🔹 What is Abstraction?
- Abstraction means **hiding the unnecessary details and highlighting the necessary details**.
- Every framework internally uses one or more technologies to generate the **common logic of the application**, but it does not let the programmer know about it – this abstraction makes development easier.

---

### 🔹 Key Points
- Frameworks are **built on top of technologies**  
- Technologies are **built on top of languages**

---

### 🔧 Example Architecture

![Framework Architecture](/img/img1.jpg)

---

### 💡 Note
- **Spring Boot = Spring++** (an enhanced version of the Spring Framework)
- Frameworks simplify development by providing **ready-to-use architecture** and **pre-built modules**.

# Plain JDBC Technology vs Spring JDBC (Framework Based Development)

---

## 🚗 Plain JDBC Technology Application

### ✅ Steps in Plain JDBC
1. Activate JDBC driver software by loading the JDBC driver class  
2. Establish a connection with the Database software from Java App  
   *(road between Java app and DB software)*
3. Create JDBC **Statement** object  
   *(Vehicle that carries SQL queries and query results)*
4. Use Statement object to send and execute SQL queries in DB software  
5. Gather SQL query results and process them  
6. Handle exceptions  
7. Close JDBC objects (including JDBC connection)

---

### 🔧 Common vs Application Logic
| Type of Logic | Meaning |
|---------------|----------|
| **Common Logic** | Repeated code used in every application (ex: loading driver, getting connection, closing resources) |
| **Application-specific Logic** | Business logic written for the application's requirements |

---

### ⚠ Boilerplate Code Problem
- The code that **repeats multiple times** in a project with **no or minor changes** is called **boilerplate code**.
- All **technology-based application development (like JDBC, Servlets)** suffer from this problem.
- Programmer has to write both:
  - ✅ Common logics  
  - ✅ Application-specific logics  
  → This **increases burden** on the programmer.

---

## ✅ Spring JDBC Application (Framework Based)

### ✅ Steps in Spring JDBC
1. Create **JdbcTemplate** class object  
   → Takes care of **common logic** internally
2. Use `JdbcTemplate` object to send and execute SQL queries in DB software  
3. Gather SQL query results and process them *(application-specific logic only)*

---

### 💡 Notes About Frameworks
- **Spring/Spring Boot** are collections of **30+ modules**
- The **Spring JDBC Module** provides **abstraction** over plain JDBC and **simplifies application development**
- While working with frameworks:
  - ✅ Developers focus only on **application-specific logic**
  - ✅ Framework automatically handles **common logic**
  - ✅ No boilerplate code problem
  - ✅ Less burden on programmer
  - ✅ Cleaner and faster development

---

### ✅ Final Conclusion
| Feature | Plain JDBC | Spring JDBC |
|----------|------------|-------------|
| Boilerplate Code | ❌ Yes | ✅ No |
| Manual JDBC Code | ✅ Yes | ❌ No |
| Focus on Business Logic | ❌ No | ✅ Yes |
| Programmer Burden | High | Low |
| Abstraction Level | Low | High |

---
