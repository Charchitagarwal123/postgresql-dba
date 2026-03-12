# Task 2.1 – Backup Automation System

## Objective
Create and manage database backups to ensure data safety and recovery.

## Commands Used

### Create Backup
pg_dump company_db > company_db_backup.sql

### Description
This command creates a logical backup of the database and stores it in a SQL file.

### Verify Backup File
ls

This command lists files in the directory to confirm that the backup file was created.
