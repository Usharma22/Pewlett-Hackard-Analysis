# Pewlett-Hackard-Analysis
working with SQL
## Overview of the analysis:
                          The purpose of the analysis was to generate a mentorship list,retirement list,and a title list for the company from the database since the company wants to have a database which it can use to make meaningful decisions.
                          These decisions will help company regarding number of positions open in company, new hirings and also to know the excat number and positions of people who are retiring so that different new programs could be implemented. 


## Results:
### Four major points are: 
     - First we created retirement_titles table which contained the list of employees that were going to retire but were born between 1952 and 1955.
![retirement_table](/Resources/retirement_titles.png)

     - Next We excluded the employees that had left the company and ceated an unique list of table known as unique_titles, that had names of employees with their recent tiltle.    
![unique_titles](/Resources/Unique_titles.png)  

     - Third, creating the number of titles table from the unique titles table to hold information of number of employees with their tiltes who are about to retire.
![retiring_titles](/Resources/Retiring_table.png)

     - Lastly, we create list of employees that are going to retire during 1965 for mentorship program that the company asked for.
![mentorship_eligibilty](/Resources/mentorship_eligibiltyTable.png)

## Summary:
    - Out of 133776 employees born between 1952 and 1955 who were on the list of retirement, some employees (72485 number) were employees that had left the company. So, around 61,000 (61,291 more precise) employees roles will be required to be fulfilled in tsunami.
    -Since the company will have 1549 employees for the mentorship program, they will be enough for the program to mentor the next generation.

    --One of the tables of retiring titles clearly tells us that more staff recruitment might be needed among senior Engineer and Senior Staff as they are in highest number who would be retiring soon.As seen in table below
![retirement_title_table](/Resources/retirement_titles.png) 

    --AS different departments within the company are likely to experience retirement of a good number of employees, it would be helpful to analyze and find out for individual department how many employees would retire and this would help individual departments to come up with a strategy/plan. Like, for example a query for sales department could be created as
     -- to create query from retirment table for sales
        SELECT * FROM dept_info
        WHERE dept_name = 'Sales';




