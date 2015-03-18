---
layout: default
title: Exercise 3 (Home)
---

# Exercise 3

## Preamble

For this exercise you will be working on a database that you know pretty well: The class database. You know pretty well the database, and of course you know that it has its own share of flaws and insufficiencies. In fact the designer of the database had to make it under time pressure and he actually just put something together. Now it is your turn to bring your magic touch to the database.

Here is an overview of the database:

![Import CSV Recordset]({{ site.baseurl }}/public/images/model.png)

You can also get the complete script to regenerate the database (data dump) from [here](https://gist.github.com/retrography/cd808312e131df2d5f3f). 

One again I repeat: Don't leave the questions unanswred. Code the parts that you can solve, and at least explain your approach if you can't solve.

## Questions

### Part 1

This database has a number of obvious design flaws, many of them among the flaws we have explicitly discussed in the class. 

1. Find these flaws, explain why they can be considered flaws and propose ways to fix them. Rely on what has been covered in the class (Normalization, DML, naming conventions, data taypes, etc...), not only your personal intuition. 
2. Design an improved version of the database and create it. You can use the visual interface or code manually. Whatever your choice is, please send me both your code and a visual representation of the results (reverse engineer).
3. Transform and import the data from the old database. This is not supposed to be a manual procedure. Do it using scripts, and send me the script.*

### Part 2

The database is also incomplete and does not include all the fields needed to manage a class. Your next mission is to complete the database.

1. How can we track absenteeism, student performance (exercises, grades, etc...) and group performance in the database? Suggest a database design for this purpose. The new design must necessarily include a student table, a group table and a presence table, along with the proper links.
2. Create this new design using code or visual tools and send me both the script and the model diagram.
3. Populate the new database with the data from the old database, the sudent information that you have already received and the group information that are public.*

* Question 3 of both parts only requires basic response that demonstrates your proficiency in transforming data. A complete data transformation solution will bring you extra points.

[Submit Solution]({{ site.baseurl }}/exercises/submission)
