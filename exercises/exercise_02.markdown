---
layout: default
title: Exercise 2 (Home)
---

# Exercise 2

## Preamble

For this exercise you will be using the "course" database that you used during the first two weeks of our course. The database that contains a version of your course outline, transformed into relational format. I will send you the credentials for a guest account once again, so we make sure you can connect to the database. Make sure you can connect to the database before you leave the classroom. You are not supposed to ask me (or Hanieh) technical questions during the week you are working on your exercise. You can, on the other hand, ask for clarification if needed.

Please comment your code duly and explain what you have done in the code. Having clear comments that show your understanding of coding concepts are more important for me than the code itself. Even if you can't manage to write down in code what you conceive in your head, explain it in comments. Make sure you don't send me a perfectly running code with very little or no comments. This said, make sure you do not send me untested code that you have never run on the SQL server. You must know whether your code runs or not, and in case it does not run you may want to explain where you think the problem lies.

Also be aware that most questions do not have a single best answer, and require you to suggest creative solutions that you find convincing. Make sure you rely on your own logic to do so, because I don't expect to see too many similar responses on those questions. Also keep in mind that some questions may not have a right answer at all (e.g. technically impossible), in which case you are required to explain why. Finally, make it clear which question you are responding to in each section of your code, and also always place the comments related to a code snippet above the code snippet (a universal convention).

Please [submit your solutions]({{ site.baseurl }}/exercises/submission)
 in form of a single script that ideally runs without error on the database. Make sure you compress the script file before submitting it through the online form. The exercise is due on __Thursday, February 26__, but since many of you are taking your midterm exams this week, you can optionally take until __Sunday, March 1__ to complete it.

## Data Dictionary

Table | Content
--- | ---
deliverable | Contains information about the deliverables of the course 
deliverable_type | Lists the types of deliverables 
module | Contains learning modules of the course
reading | Summarizes brief information about the readings of the course 
reading_type | Lists the types of the readings
reference | Contains brief information about the references of the course
reference_type | Lists the types of the references
resource | Contains information about different learning material
session | Contains brief overview of each session
session_deliverable | Builds an n:m relationship between session and deliverable
session_has_resource | Builds an n:m relationship between session and resource

## Setup Guide

- Open MySQLWorkbench
- Go to MySQLWorkbench's Home window and click the plus sign to create a new connection
- In Manage Server Connection window modify the following values: (note that all the fields are case-sensitive)

Field | Value
--- | ---
Connection Name | Class_DB
Hostname | insy437638.c67d2busrsq9.us-west-2.rds.amazonaws.com
Username | guest
Password | insy437638
Default Schema | class

-	Test the connection
-	Press OK to close the edit window and now connect to the connection by clicking on the connection in the home window

## Part 1 - I Can Win

1. List all the references that were not published in Harvard Business Review.
2. List the name and the author(s) of the references that have author information attributed to them.
3. Return the number of book chapters from the list of references.
4. List all the books that are less than a year old.

## Part 2 - Bring It On

5. List all the sessions along with the modules they belong to.
6. List the date of all the sessions along with their readings, the type of the readings, and the title of the reference used for each reading assignment.

## Part 3 - Hurt Me Plenty

7. List all the deliverables that are not due on a single session (either without a due date or due on more than one session). Is it possible to write a query that returns _only_ a list of the distinct delivery types associated with the deliverables that are not due on a single session? Why/how?
9. Which session has the largest number of resources associated with it? Write a query that returns the date of the session with the largest number of resources, the number of resources associated with it, and the number of resource types associated with it. Comment on the accuracy of your query.

## Part 4 - Hardcore 

10. Using conventional SQL write a query that gets as close as possible to [our PDF course outline]({{ site.baseurl }}/public/misc/insy437638.pdf) (obviosuly, only the table of sessions along with its content, and not the whole document with all its texts). Is it possible to reproduce the exact same outline? Why/how?

## Part 5 - Nightmare! (Challenge)

11. Is there any way to use conventional SQL to return a list of distinct sessions, with all the references required for those sessions listed horizontally in front of them (e.g. Session1, Ref1, Ref2, Ref3, ...)? Is there a generalized way to do so (independent of the number of references possible for each session)? Why/how? Are there more than one way to do so? Can you write a query that does so? What are the limitations?

[Submit Solution]({{ site.baseurl }}/exercises/submission)
