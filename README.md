# Pewlett-Hackard-Analysis
## Resources:
- SQL
- pgAdmin4
- QuickDBD

## Overview of the Analysis: 
With this weeks module, I was asked to delve into the porgramming language of SQL. While more niche, and therefore less broad in scope than Python, SQL is especially pertinent when dealing with relational databases. Relational databases are one such quality of this weeks module because we are dealing with a wide range of tables that share columns of data. I first used QuickDBD to give a data visualization of 6 tables of data (Departments, Employees, Salaries, Managers, Dept_Emp, Titles). From here, I established each of these tables in PgAdmin4 using the Query Editor and then importing the provided csv files for each. Upon completion of this, I then was able to start formulating more complex tables between the shared data of the tables, such as Employee Count by Department Number, number of employees retiring, etc. The aforementioned steps bring me to the Module Challenge. Here we are being asked to determine the number of retiring employees per title, as well as identify employees who are eligible to participate in a mentorship program. I will do this through the use of already existing tables as well as creating new tables to ascertain these requests by Bobby's manager. 

## Results:
<img width="517" alt="Results 1" src="https://user-images.githubusercontent.com/95828604/152886408-5773621e-c877-4033-ad6c-c8d819d902f9.png">
- The count of most recent titles amongst employees who are about to retire is as follows:
  - 29,414 Senior Engineers
  - 28,254 Senior Staff
  - 14,222 Engineers
  - 12,243 Staff
  - 4,502 Technique Leaders
  - 1,761 Assistant Engineers
  - 2 Managers

<img width="673" alt="Results 2" src="https://user-images.githubusercontent.com/95828604/152887019-a40cdc44-cc45-4857-be03-a28fe8b1eb31.png">
- The total number employees who are eligible to participate in a mentorship program is 56,859.

<img width="666" alt="Results 4" src="https://user-images.githubusercontent.com/95828604/152889162-fa4b0aec-782c-4cdd-bc9c-236a5774ccf7.png">
- The total number of retirement titles (the complete list of job titles both present and past for those who are retiring) is 133,776.

<img width="478" alt="Results 3" src="https://user-images.githubusercontent.com/95828604/152888807-4a1a6104-66a9-40a5-91e5-e6246f629f94.png">
- The total number of unique titles (those who are retiring) is 90,398. This means that there were 43,378 less cells after correcting for duplicates, and filtering for date of birth/date hired.

## Summary:
- How many roles will need to be filled as the "silver tsunami" begins to make an impact?
As my fourth result shows, there will be 90,398 people retiring soon in the "silver tsunami". Therefore, in the end, there will need to be 90,398 roles fulfilled by the end of the "silver tsunami". I created a more in depth breakdown with the following query, which allows me to see the count of the 90,398 amongst the various departments.
<img width="614" alt="Summary 1" src="https://user-images.githubusercontent.com/95828604/152892825-dc8afaed-d2ff-4b0a-8da4-93ce09b07860.png">

- Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?
No there are not enough qualified and retirement ready employees to replace the current mentors, should they need to. 
<img width="654" alt="Summary 2" src="https://user-images.githubusercontent.com/95828604/152893405-d78982fd-f66c-4c02-8e90-005d0c056be1.png">
