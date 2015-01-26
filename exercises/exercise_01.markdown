---
layout: default
title: Class Exercise 1
---

## Part 1

Let's first make sure we all have the same table specifications to start with. Run the following lines to drop your "people" table and recreate it.

{% highlight sql %}

DROP TABLE IF EXISTS people;

CREATE TABLE people (id int(11) NOT NULL UNIQUE AUTO_INCREMENT,
first_name varchar(45) NOT NULL,
last_name varchar(45) NOT NULL,
birth_date date DEFAULT NULL,
PRIMARY KEY (id));

{% endhighlight %}

Now check your email and save the `.csv` file you have received. This is the list of the students in the class. Open the file in notepad, textedit, or any other text editor you usually use. Have a look at the columns and figure out what additional columns you will need in your "people" table to import the data. Then try to determine the data types and the constraints that fit them the best.

1. Use `ALTER TABLE` to modify the table

2. Insert some information about me in the table using `INSERT INTO` in order to make sure the specifications are correct

    Field | Value
    --- | ---
    First Name | Mahmood
    Last Name | Zargar
    Birth Date | Jan 15, 1982
    McGill ID | 260403725
    Level| Graduate
    Degree | Doctor of Philosophy
    Program | PhD Management
    Major | Information Systems
    Class | G Level Year 4
    Email | mahmood.shafeiezargar@mcgill.ca

3. Delete the intruder who has crept into the class list from the table

4. Import the class list using MySQLWorkbench's graphic interface:

   ![Import CSV Recordset]({{ site.baseurl }}/public/images/import.png)

5. Write a query that shows the students in their 3rd year

## Solution to Part 1

{% gist retrography/f7b2e148dce14ba00794 %}

## Part 2

1. How many people are there in the class?
2. How many registered or web-registered students are there in the class?
3. Write a query that returns the number of students in their 2nd year
4. Write a query that returns the average seniority of students who are "Web Registered"
5. Write a query that returns the average seniority of students who are "Registered"
6. Write a query that returns the average seniority of each of the two groups above. Are the "Web Registered" students more senior?
7. Write a query that sorts the students by their seniority
8. Write a query that fetches the row related to the person with the highest level of seniority 
9. Write a query that fetches a list of distinct majors we have in the class
10. Write a query that fetches a list of distinct majors and the number of people in them
11. Write a query that fetches a list of distinct majors with more than two students, as well as the cumulative McGill experience of the individuals in those majors
