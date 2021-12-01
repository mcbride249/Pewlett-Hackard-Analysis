# Pewlett-Hackard-Analysis

## Project Overview
Pewlett -Hackard, a large company with several thousand employees with a length history is looking to offer retirment packages for those with certain criteria and is looking to find out which positions will need to be filled in the near fitire as a result of the upcoming retirements.

**Goals:**
1. Who is eligible for retirement.
2. Generate a list of all employees eligible for the retirement package.
3. A list of employees containing their unique employee number, their last name, first name, gender, and salary.
4. A list of managers for each department, including the department number, name, and the manager's employee number, last name, first name, and the starting and ending              employment dates.
5. An updated current_emp list that includes everything it currently has, but also the employee's departments.


**##Summary**

1. 41,380 employees are eligible for retirment.


2. A list of retiring employees can be found in the csv file: retirement_info 

    GitHub link to CSV file: https://github.com/mcbride249/Pewlett-Hackard-Analysis/blob/main/Data/retirement_info.csv

    ![Image - retirment_info](https://user-images.githubusercontent.com/92111396/144246089-e048dfb8-ad3f-45e5-9942-ac8575bc0b06.PNG)

    https://github.com/mcbride249/Pewlett-Hackard-Analysis/blob/main/Resources/Image%20-%20retirment_info.PNG


3. A list of retiring employees can be found in the csv file: emp_info.

   GitHub link to CSV file: https://github.com/mcbride249/Pewlett-Hackard-Analysis/blob/main/Data/emp_info.csv

   ![Image - emp_info](https://user-images.githubusercontent.com/92111396/144245853-eac99cac-d4f4-40de-ad09-28aa8911b50e.PNG)

   https://github.com/mcbride249/Pewlett-Hackard-Analysis/blob/main/Resources/Image%20-%20emp_info.PNG
  


4. A list of retiring employees can be found in the csv file: manager_info.

   GitHub link to CSV file: https://github.com/mcbride249/Pewlett-Hackard-Analysis/blob/main/Data/manager_info.csv

   ![Image - manager_info](https://user-images.githubusercontent.com/92111396/144245876-c2e8c83d-d535-43b6-a042-c4c364efcede.PNG)

   https://github.com/mcbride249/Pewlett-Hackard-Analysis/blob/main/Resources/Image%20-%20manager_info.PNG
  


5.  A list of retiring employees can be found in the csv file: dept_info.

   GitHub link to CSV file: https://github.com/mcbride249/Pewlett-Hackard-Analysis/blob/main/Data/dept_info.csv

   ![Image - dept_info](https://user-images.githubusercontent.com/92111396/144245767-e349d807-e38a-4c5e-ac57-4bef2ad212b3.PNG)

   https://github.com/mcbride249/Pewlett-Hackard-Analysis/blob/main/Resources/Image%20-%20dept_info.PNG



**##Resources**
-Data Source: current_emp.csv, departments.csv, dept_emp.csv, dept_info.csv, dept_manager.csv, emp_count.csv, emp_info.csv, employees.csv, manager_info.csv, mentorship_eligibility.csv, retirement_info.csv, retirement_titles.csv, retiring_titles.csv, salaries.csv, sales_development_info.csv, titles.csv, unique_titles.csv, Employees_Challenge_starter_code.csv
-Software: Python 3.7.10, Visual Studio Code, 1.38.1, pgAdmin 4v6




**##Module 7 - Written Analysis** 


**##Overview##**

The purpose of this analysis was to determine the number of retiring employees by title in addition to generating a list of the employees who are eligible for the mentorship programme at the company of Pewlett-Hackard. This was done through pgAdmin and SQL, using and expanding upon the database that was previously created in the online lesson. In this analysis we created several new tables including “Retirement Titles”, “Unique Titles” “Retiring Titles”, and the “Mentorship Eligibility” tables. These tables were created by combining specific data from previous tables using the JOIN function and then filtering and ordering the data using the COUNT, WHERE, ORDER, and GROUPBY functions. Finally, each table was exported as CSV file under their respective titles to be reviewed by Bobby’s supervisor.


**##Results##**

•	30% of Hewlett-Packard’s workforce will be retiring which is a total of 90,398 employees.

•	The title that will be retiring the most, and by extension the position that will require the largest hiring of staff to replace will be the position of senior engineer with     29,414 retirements. The Retiring Titles table shows the count of each position that is retiring.

![Image - retiring_titles](https://user-images.githubusercontent.com/92111396/144248703-6d91ce14-4760-4013-9479-9021f39cc0de.PNG)
https://github.com/mcbride249/Pewlett-Hackard-Analysis/blob/main/Resources/Image%20-%20retiring_titles.PNG

•	57,668 senior positions will need to be replaced in addition to a total of 15,983 engineer and assisting engineer positions.

•	1,549 employees are eligible for the mentorship programme. 748 of these employees hold an engineer position at some level; this demonstrates a shortfall in the number of         engineers in the mentorship programme who are eligible to replace retiring employees.

![Image - mentorship_eligibility](https://user-images.githubusercontent.com/92111396/144249028-e893e532-5376-43e9-9e73-5c253cecd106.PNG)
https://github.com/mcbride249/Pewlett-Hackard-Analysis/blob/main/Resources/Image%20-%20mentorship_eligibility.PNG



**##Sumamry##**

A total of 90,398 positions will need to be filled as the “silver tsunami” begins to make an impact, which is 30% of Pewlett-Hackard’s entire workforce. 57,668 of these retiring positions have been identified as senior positions, which accounts for just over 19% of Pewlett-Hackard’s senior personnel. This implies that the company will also see a significant loss of their experienced employees at the leadership level. 
Currently, the mentorship programme has identified only 1,549 personnel as eligible for the mentorship program which is grossly insufficient to replace the expected number of retirees that the company is facing. An expansion of this program to include employees who were born after the year 1965 may help in expanding the pool of potential mentorship candidates and allow the company to promote internally.  This could easily be done by altering the code on the query to include a wider range of birth dates; an example of this can be seen here: (WHERE (birth_date BETWEEN '1965-01-01' AND '1985-12-31').
It may be best however to find a different metric other than age to determine who is eligible for the mentorship program. The experience level of an employee is not necessarily tied to the year that they were born, and another metric such as “performance” should be included in the analysis. This would allow Pewlett-Hackard to identify those employees who are performing well and allow them the opportunity to be mentored for senior positions. However, that would require more data than what is available to us now and as such we are unable to provide any insight based on this criteria.   

