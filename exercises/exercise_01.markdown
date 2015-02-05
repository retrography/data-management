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

3. Import the class list using MySQLWorkbench's graphic interface:

    ![Import CSV Recordset]({{ site.baseurl }}/public/images/import.png)

4. Delete the intruder who has crept into the class list from the table

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
7. Write a query that returns the students sorted by their by their seniority (the more senior ones first)
8. Write a query that returns the information regarding the most senior person
9. Write a query that returns a list of distinct majors we have in the class
10. Write a query that returns a list of distinct majors and the number of people in each of them
11. Write a query that returns a list of distinct majors with at least two students, as well as the cumulative McGill experience of the individuals in each major

## Solution to Part 2
{% gist retrography/6b419f21ee5b674f13db %}

## Part 3

Before starting Part 3 of the exercise, make sure that you have used the solution from Part 1 to recreate the table and import the data.

1. Add column "team" to the table "people" as a foreign key, along with a lookup table for the foreign key that contains only a team id and a team label. Create some teams and assign students to them in a way you like.
2. Write a query that returns the list of students along with the name of the teams they belong to. What happens to the students that are not in any team?
3. Transform all columns in table "people" containing categorical values into foreign keys and add corresponding lookup tables for each. This includes the following columns: reg_status, level, degree, program, major.
4. Write a query that returns the list of students with all the lookup values fetched from the lookup tables using joins. What do you think about the new design of the class database?

## Part 4

1. Make a "course" table with a many-to-many relationship to "people"
2. Write a `JOIN` query that returns people and the courses they are taking as one list
3. Make a new field in "people" that contains information regarding people sitting next to each othe in the class  
4. Write a 'JOIN' query that returns people sitting next to each other in one list
