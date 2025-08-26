*# 💾 SQL Queries Showcase

This repository contains a collection of **SQL queries** demonstrating my expertise in **data retrieval, manipulation, and database management**.

---

## 📌 **Table of Contents**
- [Introduction](#introduction)
- [Database Schema](#database-schema)
- [Sample Queries](#sample-queries)
  - [1. Basic Queries](#1-basic-queries)
  - [2. Joins & Relationships](#2-joins--relationships)
  - [3. Aggregations & Grouping](#3-aggregations--grouping)
  - [4. Subqueries & Advanced SQL](#4-subqueries--advanced-sql)
- [How to Run](#how-to-run)
- [Screenshots](#screenshots)
- [License](#license)

---

## **Introduction**

This project highlights **mySQL** queries written to solve real-world database problems, covering:

- CRUD operations (Create, Read, Update, Delete)
- Joins (INNER, LEFT, RIGHT, FULL)
- Aggregate Functions (COUNT, SUM, AVG, MAX, MIN)
- Nested Queries & CTEs (Common Table Expressions)
- Database Design & Optimization

---

## **Database Schema**
Below is a sample schema used in these queries:

```sql
CREATE TABLE Customers (
    CustomerID INT PRIMARY KEY,
    Name VARCHAR(100),
    Email VARCHAR(100),
    Country VARCHAR(50)
);

CREATE TABLE Orders (
    OrderID INT PRIMARY KEY,
    CustomerID INT,
    OrderDate DATE,
    Amount DECIMAL(10,2),
    FOREIGN KEY (CustomerID) REFERENCES Customers(CustomerID)
);
*


## **Screenshots**

### **1. INNER JOIN**
> *Query to join table bidder and auction innerly on a condition.*
<p align="center">
  <img src="screenshot/sql1.png" alt="Customers from Nigeria" width="80%" style="border-radius:10px;box-shadow:0px 0px 10px #ccc;">
</p>

---

### **2. LEFT JOIN**
> *Query left joining `bidder` and `auction` tables ON a condition*
<p align="center">
  <img src="screenshot/sql2.png" alt="Customers and Orders" width="80%" style="border-radius:10px;box-shadow:0px 0px 10px #ccc;">
</p>

---

### **3.Filtering base on a condition**
> *Query using `WHERE` and 'AND' to filter out a data*
<p align="center">
  <img src="screenshot/sql54.png" alt="Total Amount Spent" width="80%" style="border-radius:10px;box-shadow:0px 0px 10px #ccc;">
</p>

---

### **4. GROUP BY **
> *Subquery to 'GROUP BY' a value .*
<p align="center">
  <img src="screenshot\sql5.png" alt="High Spending Customers" width="80%" style="border-radius:10px;box-shadow:0px 0px 10px #ccc;">
</p>

---
