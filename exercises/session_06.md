---
layout: default
title: Class Exercise 1
---
{% highlight sql linenos %}
SELECT
{% endhighlight %}

```
DROP TABLE IF EXISTS people;

CREATE TABLE people
(
    `id` int(11) NOT NULL AUTO_INCREMENT,
    `first_name` varchar(45) NOT NULL,
    `last_name` varchar(45) NOT NULL,
    `birth_date` date DEFAULT NULL,
    PRIMARY KEY (`id`),
    UNIQUE KEY `id_UNIQUE` (`id`)
);
```
