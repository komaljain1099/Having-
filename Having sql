-- Having VS Where
select gender, avg(age)
from employee_demographics
group by gender
having avg(age) > 20
;

select occupation,avg(salary)
from employee_salary
where occupation like '%manager%'
group by occupation
having avg(salary) > 75000;

-- Q1 Display the gender and the number of employees, but show only those genders that have more than 2 employees.
select gender,
		count(employee_id)
from employee_demographics
group by gender
having count(employee_id) > 5;

-- Q2 Display each department and its average salary, but show only departments whose average salary is greater than 60,000.
Select dept_id,
		avg(salary)
from employee_salary
group by dept_id
having avg(salary) > 60000;

-- Q3 Display each occupation and the highest salary, but show only occupations where the highest salary is greater than 80,000.
select occupation,
		max(salary)
from employee_salary
group by occupation
having 	max(salary) > 80000;

-- Q4 Display each gender and the average age, but show only genders whose average age is greater than 25.
select gender,
	avg(age)
from employee_demographics
group by gender
having avg(age) > 25;

-- Q5 Display each department and the total salary, but show only departments whose total salary is greater than 150,000.
select dept_id,
		sum(salary)
from employee_salary
group by dept_id
having sum(salary) > 150000;

-- Q6 Display each birth year and the number of employees born in that year, but show only years with more than 1 employee.Hint: YEAR(birth_date)
select year(birth_date),
		count(year(birth_date))
from employee_demographics
group by year(birth_date)
having count(year(birth_date)) > 1;

-- Q7 Display each last name and the number of employees, but show only last names that appear more than once.
select last_name,
		count(last_name)
From employee_demographics
group by last_name
having count(last_name) > 1
;

-- Q8 Display each occupation and the minimum salary, but show only occupations whose minimum salary is greater than 50,000.
Select occupation,
		min(salary)
from employee_salary
group by occupation
having min(salary) > 50000;

-- Q9 Display each department and the maximum salary, but show only departments where the maximum salary is at least 90,000.
Select dept_id,
		max(salary)
from employee_salary
group by dept_id
having max(salary) >= 90000;

-- Q10 (Interview Style) Display: Gender, Number of employees, Average age,Show only genders that: have more than 2 employees, and have an average age greater than 25.
select gender,
		count(first_name),
		avg(age)
from employee_demographics
group by gender
having count(first_name) > 2 AND avg(age) > 25;
 
-- Q11 Display each gender and the total number of employees. Show only genders with more than 3 employees.
select gender,
	count(first_name)
from employee_demographics
group by gender
having 	count(first_name) > 3;

-- Q12 Display each department and the total salary. Show only departments with a total salary greater than 200000.
Select dept_id,
		sum(salary)
from employee_salary
group by dept_id
having sum(salary) > 200000;

-- Q13 Display each occupation and the average salary. Show only occupations whose average salary is at least 60000.
select occupation,
		avg(salary)
from employee_salary
group by occupation
having avg(salary) >= 60000;

-- Q14 Display each birth year and the number of employees born in that year. Show only years having more than one employee.
select year(birth_date),
		count(*) as Number_of_employees
from employee_demographics
group by year(birth_date)
having count(*) > 1;

-- Q15 Display each department and the maximum salary. Show only departments where the maximum salary is less than 100000.
SELECT dept_id,
		max(salary)
from employee_salary
group by dept_id
having max(salary) < 100000;

-- Q16 Display each gender and the minimum age. Show only genders where the minimum age is greater than 20.
SELECT gender,
	min(age)
from employee_demographics
group by gender
having min(age)>20;

-- Q17 Display each occupation and the number of employees. Show only occupations with exactly one employee.
select occupation,
		count(*)
from employee_salary
group by occupation
having count(*) = 1;

-- Q18 Display each last name and the number of employees. Show only last names appearing at least three times.
Select last_name,
	count(*)
from employee_demographics
group by last_name
having count(*) >= 3;

-- Q19 Display each department and the average salary. Show only departments where the average salary is between 50000 and 80000.
select dept_id,
		avg(salary)
from employee_salary
group by dept_id
having avg(salary) between 50000 and 80000;

-- Q20 Display each age and the number of employees. Show only ages that have exactly two employees.
Select age,
		count(*)
from employee_demographics
group by age
having count(*) = 2;

-- Q21 Display each gender, average age, and employee count. Show only genders where: average age is greater than 25, employee count is greater than 3
SELECT gender, 
		avg(age),
        count(*)
from employee_demographics
group by gender
having avg(age) > 25 and count(*) >3;

-- Q22 Display each department and total salary. Show only departments where: total salary is greater than 150000, maximum salary is greater than 70000
SELECT dept_id,
		sum(salary),
        max(salary)
from employee_salary
group by dept_id
having sum(salary) > 150000 and max(salary) > 70000;

-- Q23 Display each occupation and:average salary , minimum salary
-- Show only occupations where: average salary is greater than 50000, minimum salary is greater than 30000
Select occupation,
		avg(salary),
		min(salary)
from employee_salary
group by occupation
having avg(salary) > 50000 and min(salary) > 30000;

-- Q24 Display each birth year and average age. Show only birth years where:average age is greater than 25, employee count is greater than 1
Select year(birth_date),
		avg(age),
        count(*)
from employee_demographics
group by year(birth_date)
having avg(age) > 25 and count(*) > 1;

-- Q25 Display each gender and the oldest employee's age. Show only genders where the oldest employee is 45 or older.
Select gender,
		Max(age)
from employee_demographics
group by gender
having max(age) >= 45;

-- Q26 Display each department with:employee count, total salary, average salary. Show only departments where:employee count > 2, average salary > 50000
select dept_id,
		count(*) as employee_count,
		sum(salary),
		avg(salary)
from employee_salary
group by dept_id
having employee_count > 2 and avg(salary) > 50000;




