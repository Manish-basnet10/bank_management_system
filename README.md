
# Bank Management System

## 📌 Project Description
A Java-based Bank Management System that allows customers to create accounts, deposit, withdraw money, and check balances. Admin can manage accounts. The system uses **JDBC with MySQL** for data storage and retrieval.

---

## ✅ Problem Statement
Manual banking operations are slow and error-prone. This system automates account management and transactions securely.

---

## 🎯 Target Users
- **Customers**: Perform banking operations like deposits, withdrawals, and balance checks.
- **Admins**: Manage accounts and monitor transactions.

---

## 🔑 Features
- Create new account
- Deposit and withdraw money
- Check balance
- Transaction history
- Admin account management

---

## 🛠 Technologies Used
- **Java**
- **MySQL** (Database)
- **JDBC** (Database Connectivity)
- **OOP Principles**: Inheritance, Polymorphism, Abstraction, Encapsulation

---

## 📂 Project Structure
BankManagementSystem/
│
├── src/ (Java source files)
├── database/ (SQL script)
├── screenshots/ (Project images)


✅ Step 3: Class Diagram (UML)

Here’s the basic UML diagram.

+-----------------+         +-------------------+
|     Account     |         |     Transaction   |
+-----------------+         +-------------------+
| - accountNo     |         | - transactionId  |
| - name          |         | - date           |
| - balance       |         | - amount         |
| - type          |         | - type           |
+-----------------+         +-------------------+
| + deposit()     |         | + record()       |
| + withdraw()    |         +-------------------+
| + checkBalance()|
+-----------------+

          ^
          |
+-----------------+
|    Savings      |
+-----------------+
| + interestRate  |
| + applyInterest()|
+-----------------+

+-----------------+
|      Bank       |
+-----------------+
| - accountList   |
+-----------------+
| + createAccount()|
| + deleteAccount()|
| + viewAccounts() |
+-----------------+

---

##  OOP Concepts Used
- **Encapsulation**: Private fields with getters/setters.
- **Inheritance**: SavingsAccount and CurrentAccount inherit from Account.
- **Polymorphism**: Overridden methods for withdrawals.
- **Abstraction**: Abstract Account class.
