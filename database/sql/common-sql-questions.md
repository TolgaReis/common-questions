# Common SQL Questions

## How to reset AUTO_INCREMENT in MySQL

How can I *reset* the **AUTO_INCREMENT** of a field?

You can reset the counter with:

```sql
ALTER TABLE tablename AUTO_INCREMENT = 1
```

​	For InnoDB(Storage engine for the database management system **MySQL** and **MariaDB**) you cannot set the **AUTO_INCREMENT** value lower or equal to the current index.