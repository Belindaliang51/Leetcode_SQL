Diffculty: Medium

HINT: subquery 
```
SELECT 
FROM
JOIN
ON
WHERE()IN(
  SELECT FROM
  GROUP BY
)
```

Answer: 
```
SELECT Department.Name AS Department,
        Employee.Name AS Employee,
        Salary
FROM Employee
JOIN Department
  ON Employee.DepartmentId = Department.Id
WHERE(Employee.DepartmentID, Salary)IN(
    SELECT DepartmentId, Max(Salary)
    FROM Employee
    GROUP BY DepartmentId
)
```
