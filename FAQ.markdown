---
layout: page
title: Frequently Asked Questions
---

## How should I prepare for the first graded exercise?
The first graded exercise (Exercise 2) is mainly about fetching and formatting data using SQL commands. So, obviously you need to know how to `SELECT` data from one or multiple tables, and apply the proper `JOIN` or `UNION` method when needed. Make sure you know how subqueries function since they are necessary for complex requests. Also make sure you know how the aggregate functions work and how you can use SQL clauses like `WHERE`, `HAVING`, `GROUP BY` and `ORDER BY` to filter, sort and group data. 

You will be required to submit your response as a well-commented SQL script that I will subsequently run on my MySQL database. What defines your grade is:

- Whether the code you have submitted uses the correct syntax and runs with no issue
- Whether your code produces the expected results
- Whether you are able to explain what the code actually does in your comments (most important)
- Whether you have come up with your own original reponses to the creative questions (very important)

If you are feeling week or unprepared in any of these areas, you have until the day the exercise is distributed to ask for a tutorial session or to simply ask questions. Also make sure you have read the course material and you have practiced enough. Practice makes perfect.

You can use third-party software to generate code and you can try to solve the tough problems in small groups, but it is very important that you can describe what you have done in your own words (in comments), and provide your own creative solutions where it applies.

## I need more practice!

The Watson book has [a nice companion website](http://richardtwatson.com/dm6e/) with numerous examples and additional exercises.

## Can I use the 5th edition of Watson's book that is available as an ebook in the library?

I can't say I have extensively researched the differences between the two editions, but I have had a look at the 5th edition and at least on the surface it does not seem to have any significant difference with the 6th edition, particularly with regard to what we cover. But unfortunately I can’t guaranty that no part of the chapters has been updated. If you intend to use the 5th edition, at least make sure you have verified the order and the topic of the chapters in each version and their eventual differences. [Here is the TOC of the 6th edition](http://richardtwatson.com/dm6e/Reader/contents.html).

## Can I have a copy of the syllabus in PDF?

Oh, you disappoint me... ;) [Of course you can]({{ site.baseurl }}/public/misc/insy437638.pdf), but it won't be updated during the trimester, so please check this website regularly instead of relying on the PDF.    

## I haven't learned anything up to know, is there any way to learn SQL overnight?

Not really, but [this](https://github.com/tthibo/SQL-Tutorial) may help.

## Why MySQL doesn't let me delete my records?

It is a safety measure, and a non-standard behavior. But you can make it comply by going to MySQLWorkbench | Preferences | SQL Editor and then unchecking "Forbid UPDATEs and DELETEs with no key in WHERE clause or no LIMIT clause."

## Do I need to surround every object name with backticks in MySQL?

No, only if you have used unconventional characters in your naming.

## Single quotes or double quotes?

Whatever works. Typically, double quotes on Heroku and single quotes on Amazon. If you install your own server, you have the choice!

## Is there any good SQL command reference you recommend?

There are many good ones, but almost all of them exclusively cover standard-based SQL. If you want a reference for MySQL's flavor of SQL, read [MySQL's reference manual](https://dev.mysql.com/doc/refman/5.1/en/sql-syntax.html). If you want a quick reference for everyday use, you can find one on [1keydata.com](http://www.1keydata.com/sql/sql.html).

## How can I generate some test data to play with?

Have a look at [generatedata.com](http://www.generatedata.com) as well as [mockaroo.com](http://www.mockaroo.com).

## Where can I get some real data to play with?

- http://donnees.ville.montreal.qc.ca
- http://open.canada.ca
- http://www.donnees.gouv.qc.ca
- http://data.un.org
- https://openlibrary.org/data

## Oops, even the course outline is in a database! Can you give me some SQL commands that help me check the course outline?

I hope by that you mean something beyond `SELECT * FROM table_name;` that you should probably know very well by now.

Apart from that, to get a list of deliverables corresponding to each session:

{% gist retrography/6780da2187556bc09b29 %}

For a list of readings assigned for each session:

{% gist retrography/e6b194919af42af7075a %}

For a list of slides and other resources for each session:

{% gist retrography/db50fb8757f1f6877812 %}
