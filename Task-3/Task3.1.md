# Task 3.1 – PostgreSQL Monitoring

## Objective
Observe real-time database behavior using PostgreSQL system views.

## Monitoring Queries

### Check Active Connections
SELECT * FROM pg_stat_activity;

### Identify Long Running Queries
SELECT pid, usename, now() - query_start AS duration, state, query
FROM pg_stat_activity
WHERE state != 'idle'
ORDER BY duration DESC;

### Monitor Locks
SELECT * FROM pg_locks;

### Check Database Size
SELECT datname, pg_size_pretty(pg_database_size(datname))
FROM pg_database;

### Check Table Size
SELECT relname, pg_size_pretty(pg_total_relation_size(relid))
FROM pg_stat_user_tables;

## Explanation
These system views help monitor database activity, running queries, locks, and storage usage.
