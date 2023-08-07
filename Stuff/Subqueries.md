```SQL
SELECT firstName, lastName
FROM customers
WHERE customerId IN
    (SELECT customerId
    FROM orders
    WHERE total > 300);
```
Allows for a query to run and pass the data into another query