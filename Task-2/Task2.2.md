# Task 2.2 – Restore Verification & PITR (Intro)

## Objective
Verify database recovery by restoring a backup and checking the stored data.

## Commands Used

### Create Restore Database
createdb company_db_restore

### Restore Backup
psql company_db_restore < company_db_backup.sql

### Verify Restored Data
SELECT * FROM app_schema.employees;

### Explanation
The backup file was restored into a new database to confirm that the data can be successfully recovered.
