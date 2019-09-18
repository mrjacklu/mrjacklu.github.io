---
title: "SQL Querying in Jupyter Notebook"
date: 2019-09-17
tags: []
category: tutorials
header:
  image: ""
excerpt: "This is a tutorial on querying SQL via Jupyter Notebook."
mathjax: "true"
---

# A Jupyter Notebook / SQL Tutorial!

Recently, I was working with a large csv file with multiple tables that required a lot of data wrangling. My first impulse was to import it into Excel and initiate the clean up there. Excel would have worked fine, but it would have taken longer to change/replace/delete columns and values. I opted to use my newly acquired skills in Python and SQL and SQLite. in order to practice those skills. So that's what I did.

# Converting .CSV into a SQL Database file

The first step is to convert your .CSV files into an SQL friendly database file that ends in .DB.

I found multiple ways to do this. All of them involve creating SQL tables with defined fields, data types.

- Use a web application that converts file formats such as [Convertcsv.com](http://www.convertcsv.com/csv-to-sql.htm). This website is pretty straight forward, as they take you through the process step-by-step to generate a .DB file.

- If you're interested in having an actual database GUI where SQL files are properly displayed and visualized in tables and schemas I would highly recommend using [SQLite](https://sqlitebrowser.org/). This is a a light weight, open source database for small applications and projects. It's easy to download and set up. Go to the [download page](https://sqlitebrowser.org/dl/) and get the version that corresponds to your OS. After it's downloaded, you need to create a dummy table. Just create a new file, name it. Then you can import your CSV file into it. For visual assistance with this, check out this [Youtube video](https://www.youtube.com/watch?v=TOqI-KiTBKU).





#
