# Task4 Aggregate Functon - SUM,COUNT,AVG.
CREATE TABLE employe (
   emp_id INT PRIMARY KEY,
   department VARCHAR(50),
   age INT,
   salary INT);  
INSERT INTO employe(emp_id,department,age,salary) VALUES 
('1','IT','23','35000'),
('2','HR','27','45000'),
('3','IT','28','30000'),
('4','IT','25','45000'),
('5','HR','24','35000');

SELECT department , SUM(salary) FROM employe
GROUP BY department ;

SELECT department , salary , COUNT(*) FROM employe
GROUP BY department ;

SELECT department , AVG(salary) FROM employe
GROUP BY department ;
