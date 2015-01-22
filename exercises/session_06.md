---
layout: default
title: Class Exercise 1
---

Let's first make sure we all have the same table specifications to start with. Run the following lines to drop your "people" table and recreate it.

{% highlight sql linenos %}
DROP TABLE IF EXISTS people;

CREATE TABLE people (`id` int(11) NOT NULL AUTO_INCREMENT,
`first_name` varchar(45) NOT NULL,
`last_name` varchar(45) NOT NULL,
`birth_date` date DEFAULT NULL,
PRIMARY KEY (`id`),
UNIQUE KEY `id_UNIQUE` (`id`));
{% endhighlight %}

Now check your email and save the `.csv` file you have received. This is the list of the students in the class. Open the file in notepad, textedit, or any other text editor you usually use. Have a look at the columns and figure out what additional columns you will need in your "people" table to import the data. Then try to determine the data types and the constraints that fit them the best.

- Use `ALTER TABLE` to modify the table
- Insert some information about me in the table using `INSERT INTO` in order to make sure the specifications are correct

> First Name: Mahmood
> Last Name: Zargar
> Birth Date: Jan 15, 1982
> McGill ID: 260403725
> Level: Graduate
> Degree: Doctor of Philosophy
> Program: PhD Management
> Major: Information Systems
> Class: G Level Year 4
> Email: mahmood.shafeiezargar@mcgill.ca

- Delete the intruder who has crept into the class list from the table
- Import the class list using MySQLWorkbench's graphic interface:

![Import CSV Recordset]({{ site.baseurl }}/public/images/import.png)

- Write a query that shows the students in their 3rd year
- How many people are there in the class?
- How many students are there in the class?
- Write a query that shows the number of students in their 2nd year
- Write a query that shows the average class of students who are "Web Registered"
- Write a query that shows the average class of students who are "Registered"
- Write a query that compares the two above. Are the "Web Registered" students  more senior?
- Write a query that sorts the students by their class
- Write a query that fetches the largest number of years spent in McGill
- Write a query that fetches a list of distinct majors we have in the class
- Write a query that fetches a list of distinct majors and the number of people in them
- Write a query that fetches a list of distinct majors with more than two students, as well as the cumulative McGill experience of the individuals in those major
