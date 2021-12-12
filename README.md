# Pewlett_Hackard_Analysis

## Overview of Project
A manager has given three assignments: to determine the number of retiring employees per title, identify the number of employees who are eligible to participate in a mentorship program and lastly, to help prepare the manager for the upcoming "silver tsunami". For the analysis, I have used the data tools PostgreSQL, pgAdmin python and Visual Studio Code.

## Deliverable 1: The Number of Retiring Employees by Title
Using PostgreSQL, I created and executed a query to make a retirement titles table for employeers who are born between Jauanry 1, 1952 and Deember 31 1955. The retirement table syntax and table can be seen below. Following the table creation I exported the table as CVS which can be retrived in the data file, listed as retirement_titles.csv

![Retirement_titles_table.png](https://user-images.githubusercontent.com/48603147/145732284-f42c55d7-f057-4b84-bf7b-1c4efbcb5a2a.png)

The next step in deliverable 1 was to create a unique title table that contains the employee number, first and last name and most recent title. The code and table can be seen in the image below. Table has been exported as a CVS in the data file and is listed as unique_titles.csv

![Unique_titles_table.png](https://user-images.githubusercontent.com/48603147/145732245-9bcd65f6-b25b-4c73-864b-9e1c09d286f1.png)

The final step in deliverable 1 was to write a query to create a retiring tiles table that contains the number of titles filled by employees who are retiring. The query and table can be seen in the following image and the CVS can be found in the data file listed as Retiring_titles_table.csv

![Retiring_titles_table.png](https://user-images.githubusercontent.com/48603147/145732205-23aaf015-fc09-4d6a-a235-efc87e8d408e.png)

## Deliverable 2: Employees eligible for the mentorship program
In this deliverable I created a table that holds the employees who are eligible for a mentorship program. The employees eligible are employees who were born between Jaunary 1st, 1965 and December 31st, 1965. As seen in the query below, I retreived the employee number, first name and last name and birthdate columns from the employees table, retrieved the from_date and to_date from the department employee table, joined the employees and title table on the primary keys and filterered the to_date columne and birth_date column to retrieve all emplyees whose birthdates within the given constraints. Mentorship eligibility table was exported as a csv into the data folder.
![mentorship_table.png](https://user-images.githubusercontent.com/48603147/145733249-fb2c111c-7e9d-4f47-905d-ac7ff871e061.png)

## Deliverable 3: Overview of analysis, results and summary
# Overview of Analysis 
The purpose of this analysis was to identify employeers who might be retiring from the company, Pewlett Hackard, and to provide insight on which departments are losing employers. In an effort to help ease the burden of lost employees we identified employeers who are eligible to participate in a mentorship program. 
# Results
From the second deliverable, the count of employeers by who could retire at any given time by department is as followes. 
* 32,425 Staff Employees
* 29,415 Senior Engineers
* 14,221 Engineers
* 8,047 Senior Staff
* 4,502 Techinque Leaders
* 1,761 Assistant Engineers
![Retiring_titles_table.png](https://user-images.githubusercontent.com/48603147/145732205-23aaf015-fc09-4d6a-a235-efc87e8d408e.png)
**As we can see, the number of potential reitirees is very high with 90,398 employees expected to retire at any given point. The percentage of retireing employees is 23% of the total company as seen in the pie chart below and therefore the mentorship program is strongly recommended. 
![retiring_table.png](
# Summary 
How many roles will need to be filled?
* 90,398 roles will be need to be filled out as there are 90,398 employees entering potential retirement
Are the enough qualifed retierment-ready employees in the departments to mentor the next generaton of Pewlett Hackard employees?
* There are not enough employees who are qualified to participate in the mentorship program as there are only 1,940 employees who are eligible as found from the mentor_elogibility table created in the 2nd deliverable.
