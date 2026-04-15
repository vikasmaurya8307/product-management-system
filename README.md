# 📦 Product Management System (PMS)
### Python-MySQL Integration | Data Persistence | Structured Analytics with Pandas

<p align="left">
<img src="https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white" />
<img src="https://img.shields.io/badge/Database-MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" />
<img src="https://img.shields.io/badge/Library-Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" />
<img src="https://img.shields.io/badge/Interface-CLI-black?style=for-the-badge&logo=gnumetashadertoy" />
</p>

---

## 📌 Project Overview
The **Product Management System** is a robust CLI-based application designed to bridge the gap between high-level Python logic and relational database storage. This project focuses on efficient **CRUD (Create, Read, Update, Delete)** operations, utilizing the `Pandas` library to transform raw SQL data into professionally structured tabular formats for better readability and data handling.

## 🚀 Core Features

* **Relational Data Persistence:** Seamlessly integrates with MySQL to ensure permanent storage of product records.
* **Dynamic Data Entry:** Interactive command-line modules for real-time product insertion with validation.
* **Advanced Search Capabilities:** High-speed querying to fetch specific records by unique identifiers (Product IDs).
* **Structured Data Output:** Leverages the power of **Pandas DataFrames** to display database results in a clean, organized, and tabular format.
* **Stable Connection Management:** Implemented centralized database configuration for easy environment switching and secure connectivity.

---

## 🛠️ Technical Stack
* **Language:** Python 3.x
* **Database:** MySQL Server
* **Libraries:** `mysql-connector-python` (Database Driver), `pandas` (Data Manipulation)
* **Design Pattern:** Modular Programming (Separation of Concerns)

---

## 📂 Project Architecture
```text
📦 product-management-system
 ┣ 📜 database.py          # Configuration & Connection Engine
 ┣ 📜 insertdata_input.py  # Data Intake: Handles user input & SQL INSERT logic
 ┣ 📜 searching.py         # Query Engine: Logic for fetching and filtering data
 ┗ 📜 README.md            # System Documentation

⚙️ System Setup & Deployment
1. Database Initialization
Run the following SQL commands in your MySQL environment to set up the relational schema:
CREATE DATABASE indian_bank;
USE indian_bank;

CREATE TABLE products (
    products_id INT PRIMARY KEY,
    products_name VARCHAR(50),
    products_price INT
);
2. Dependency Installation
Install the required Python drivers and libraries via pip:

Bash
pip install mysql-connector-python pandas
3. Execution Workflow
Establish Connection: Run python database.py to verify the DB handshake.

Ingest Data: Run python insertdata_input.py to populate the system.

Retrieve Information: Run python searching.py to view the comprehensive inventory or search for specific items.

📊 Sample Output Representation
====================== All Products =======================
   products_id products_name products_price
0          101        Laptop          50000
===========================================================

Enter product_id to search: 101
Searching...
Result Found:
   products_id products_name products_price
0          101        Laptop          50000
👨‍💻 Developed By
Vikas Maurya Backend Developer & Data Enthusiast
