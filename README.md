# 💊 Python Pharmacy Management System

The **Pharmacy Management System** is a software application designed to streamline and automate daily pharmacy operations. It helps pharmacists efficiently manage medicines, stock, customers, and reports through an intuitive interface.

---

## 🌟 Overview

This project combines a **Tkinter-based graphical user interface** with a **MySQL database** to provide a complete solution for managing pharmacy workflows. It ensures accuracy, efficiency, and ease of use in handling medical inventory and related operations.

---

## 🖥️ User Interface (Tkinter)

* Built using **Python Tkinter**
* Simple and user-friendly design
* Provides access to:

  * Login system
  * Dashboard
  * Stock management
  * Report generation

---

## 🗄️ Database (MySQL)

* Uses **MySQL** as the backend database
* Stores:

  * Medicine details
  * Customer records
  * Hospital data
  * Stock information

---

## 🔑 Core Features

### 🔐 Login System

* Secure authentication for users
* New user registration supported
* Role-based access control

---

### 📊 Dashboard

* Overview of pharmacy operations
* Displays:

  * Stock status
  * Order history
  * Pending tasks

---

### 💊 Medicine Management

* Add new medicines
* Update existing records
* Delete outdated entries
* Store:

  * Name
  * Quantity
  * Price
  * Expiry date

---

### 📦 Stock Monitoring

* Track medicine availability
* Identify low stock levels
* Monitor expiry dates
* Improve inventory control

---

### 📄 PDF Report Generator

* Generate stock reports in PDF format
* Easy sharing with hospitals or management

---

### 📋 Stock Statement

* Displays:

  * Available medicines
  * Shelf numbers
  * Expiry dates
* Helps in quick inventory checks

---

## 🔒 Security

* User authentication system
* Controlled access to sensitive operations
* Ensures data safety and integrity

---

## ⚠️ Challenges

* Keeping medicine data updated
* Managing large inventory efficiently
* Handling expiry tracking accurately
* Ensuring system scalability

---

## 🛠️ MySQL Database Setup

Run the following SQL commands to create the database and tables:

```sql
-- Create Database
CREATE DATABASE mydata;

-- Use Database
USE mydata;

-- Table: pharma (medicine details)
CREATE TABLE pharma (
    medicine_id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    quantity INT,
    price DECIMAL(10,2),
    expiry_date DATE
);

-- Table: pharmacy (user details)
CREATE TABLE pharmacy (
    user_id INT AUTO_INCREMENT PRIMARY KEY,
    username VARCHAR(50),
    password VARCHAR(100),
    role VARCHAR(50)
);

-- Table: toaddress (customer/hospital address)
CREATE TABLE toaddress (
    address_id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    address TEXT,
    phone VARCHAR(15)
);
```

---

## 📦 How to Run

1. Install Python and MySQL
2. Set up the database using the SQL script above
3. Connect Python to MySQL using a connector (e.g., `mysql-connector-python`)
4. Run the Tkinter application

---

## 🎯 Purpose

This project is built to:

* Simplify pharmacy operations
* Improve inventory management
* Reduce manual errors
* Provide a learning experience in full-stack development

---

## 📌 Note

This project is intended for **educational purposes** and demonstrates how a pharmacy system can be developed using Python and MySQL.
