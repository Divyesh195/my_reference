# SQL

## 1. Command to search a pattern

### Select all customers that starts with the letter "a"
```
SELECT * FROM Customers
WHERE CustomerName LIKE 'a%';
```

### Select all customers from city which has "on" in the name
```
SELECT * FROM Customers
WHERE city LIKE '%on%';;
```