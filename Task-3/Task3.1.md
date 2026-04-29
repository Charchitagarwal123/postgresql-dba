# Task 3.1 – PostgreSQL Monitoring

## Objective
Observe real-time database behavior using PostgreSQL system views.

## Monitoring Queries

### Check Active Connections
SELECT * FROM pg_stat_activity;

### OPEN TERMINAL
open Ubuntu terminal

### INSTALL REQUIRED PACKAGES
sudo apt update
sudo apt upgrade
sudo apt install python3-pip -y
pip3 install flask psycopg2-binary

### CREATE PROJECT FOLDER
mkdir flask_dashboard
cd flask_dashboard

### CREATE FILES
touch app.py
mkdir templates
touch index.html

### WRITE BACKEND CODE
Step 1: Open file
nano app.py


## Explanation

