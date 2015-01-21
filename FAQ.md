---
layout: page
title: Frequently Asked Questions
---

## Can I use the 5th edition of Watson's book that is available as an ebook in the library?

I can't say I have extensively researched the differences between the two editions, but have I had a look at the 5th edition and at least on the surface it does not seem to have any significant difference with the 6th edition, particularly with regard to what we cover. But unfortunately I can’t guaranty that no part of the chapters has been updated. If you intend to use the 5th edition, at least make sure you have verified the order and the topic of the chapters in each version and their eventual differences. [Here is the TOC of the 6th edition](http://richardtwatson.com/dm6e/Reader/contents.html).

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

There are many good ones, but almost all of them exclusively cover standard-based SQL. If you want a reference for MySQL's flavor of SQL, read [MySQL's reference manual](https://dev.mysql.com/doc/refman/5.1/en/sql-syntax.html). If you want a quick reference for everyday use, you can find one [here](http://www.1keydata.com/sql/sql.html).


<!--- queries for database access, also how to create fake data --->
