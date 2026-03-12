# Task 1.1 – Database & Role Management

## Objective
Implement role based access control in PostgreSQL.

## Commands Used

### Create Database
CREATE DATABASE company_db;

### Connect to Database
\c company_db

### Create Roles
CREATE ROLE admin_role;
CREATE ROLE read_only;
CREATE ROLE read_write;

### Verify Roles
\du

### Create Table
CREATE TABLE employees(
emp_id SERIAL PRIMARY KEY,
name TEXT,
salary INT
);

### Insert Data
INSERT INTO employees(name,salary) VALUES
('Rahul',60000),
('Neha',55000),
('Amit',45000);
