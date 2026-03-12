# Task 1.2 – Schema & Object Lifecycle Manager

## Objective
Control database object sprawl and organize objects using schemas.

## Commands Used

### Create Schema
CREATE SCHEMA app_schema AUTHORIZATION admin_role;

### Move Table to New Schema
ALTER TABLE public.employees SET SCHEMA app_schema;

### Create Index
CREATE INDEX idx_employees_salary
ON app_schema.employees(salary);

### Create View
CREATE VIEW high_salary_employees AS
SELECT emp_id, name, salary
FROM app_schema.employees
WHERE salary > 50000;

## Verification Commands

List Schemas
\dn

List Tables
\dt

List Indexes
\di

List Views
\dv
