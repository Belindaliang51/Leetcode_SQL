Difficulty: Easy 

Answer: 
```
SELECT p.FirstName, p.LastName, a.City, a.State 
FROM Person AS p
LEFT JOIN Address AS a 
ON p.PersonId = a.PersonId
```
Tip:
JOIN vs LEFT JOIN 
default JOIN is INNER JOIN, whereas LEFT JOIN is one of the OUTER JOIN(s)
