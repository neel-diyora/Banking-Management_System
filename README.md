# 💳 Banking Management System

A secure and robust **Java-based Banking Management System** that allows users to register, log in, and manage bank accounts and transactions. This project uses **Java**, **MySQL**, and **JDBC**, applying **Object-Oriented Programming (OOP)** principles to build a modular, maintainable, and scalable system.

---

## 📌 Features

- ✅ User registration and secure login using email and password  
- ✅ Create and manage individual bank accounts  
- ✅ View balance and perform transactions  
- ✅ Security PIN verification for sensitive operations  
- ✅ Unique constraints on email to prevent duplicate entries  
- ✅ Proper exception handling and input validation  
- ✅ Separation of concerns via modular OOP design  

---

## 🧰 Tech Stack

| Technology | Description                        |
|------------|------------------------------------|
| Java       | Core language for backend logic    |
| JDBC       | To interact with MySQL database    |
| MySQL      | Backend relational database        |
| OOP        | For class-based design and abstraction |

---

## 🗃️ Database Schema

### `accounts` Table

| Field          | Type           | Constraints         |
|----------------|----------------|---------------------|
| account_number | bigint         | Primary Key         |
| full_name      | varchar(255)   | Not Null            |
| email          | varchar(255)   | Unique, Not Null    |
| balance        | decimal(10,2)  | Not Null            |
| security_pin   | char(4)        | Not Null            |

### `user` Table

| Field     | Type           | Constraints         |
|-----------|----------------|---------------------|
| full_name | varchar(255)   | Not Null            |
| email     | varchar(255)   | Primary Key         |
| password  | varchar(255)   | Not Null            |

---

## 🏗️ Project Structure

```
BankingManagementSystem/
│
├── BankingApp.java         # Entry point (Main class)
├── AccountManager.java     # Logic for account operations
├── Accounts.java           # Account model with methods
├── User.java               # User model and login logic
├── .gitignore
└── Banking Management System.iml
```

---

## ⚙️ How to Run

1. Ensure you have **Java** and **MySQL** installed on your system.
2. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/BankingManagementSystem.git
   cd BankingManagementSystem
   ```
3. Create the required database and tables using the schema described above.
4. Update your database credentials in the Java files.
5. Compile and run the project:
   ```bash
   javac *.java
   java BankingApp
   ```

---

## 🔐 Security Notes

- Passwords and security PINs are not encrypted; for production systems, implement hashing and encryption (e.g., **BCrypt**).
- Avoid exposing database credentials in source files. Use **environment variables** or **config files**.

---

## 🚀 Future Improvements

- Add encryption for passwords and security pins  
- Introduce transaction history tracking  
- Build a Swing-based or web-based GUI  
- Add role-based access control (e.g., Admin/Customer)  
- Implement REST APIs for a full-stack application  

---

## 🙌 Acknowledgements

This project was developed as a **learning exercise** to understand full-cycle software development using **Java**, **JDBC**, and **SQL**, incorporating **clean code principles** and **OOP concepts**.
