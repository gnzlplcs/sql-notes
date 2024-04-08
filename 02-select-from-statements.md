# SELECT and FROM statements

```sql
--SELECT all columns
SELECT * FROM EmployeeDemographics;

--only selects two columns
SELECT FirstName, LastName
FROM EmployeeDemographics;
--retrieves only two columns, all rows

--TOP
SELECT TOP 5 *
FROM EployeeDemogaphics;
--returns only the first 5 rows

--DISTINCT
SELECT DISTINCT(Gender)
FROM EmployeeDemographics;
--returns only unique values ('Male' and 'Female')

--COUNT
SELECT COUNT(LastName)
FROM EmployeeDemographics;
--returns an unnamed column with the number of
--ocurrencies (No column name - 9)

--AS allows to rename a column or table using an alias
SELECT COUNT(LastName) AS LastNameCount
FROM EmployeeDemographics;
--returns an named column with the number of ocurrencies
--(LastNameCount - 9)

--MAX
SELECT MAX(Salary)
FROM EmployeeSalary;
--returns max value 65000

--MIN
SELECT MIN(Salary)
FROM EmployeeSalary;
--returns min value 36000

--AVG
SELECT AVG(Salary)
FROM EmployeeSalary;
--returns the average of the selected column: 48555

--SELECT from main
SELECT *
FROM SQLTutorial.dbo.EmployeeSalary
```