Difficulty: Easy 

Answer: 
```
SELECT IFNULL((SELECT DISTINCT Salary
              FROM Employee
              ORDER BY Salary DESC
              LIMIT 1 OFFSET 1),NULL) as SecondHighestSalary
```
Tip:

<code>IFNULL(expression, alt_value)</code>

SELECT col AS output_col