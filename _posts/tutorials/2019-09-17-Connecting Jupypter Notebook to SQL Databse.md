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

### Background

Recently, I was working with a large csv file with multiple tables that required a lot of data wrangling. My first impulse was to import it into Excel and initiate the clean up there. Excel would have worked fine, but it would have taken longer to change/replace/delete columns and values. I opted to use my newly acquired skills in Python and SQL and SQLite, mostly because I wanted to practice those skills. So that's what I did, and this is a tutorial based on that using a simple database file.

### Step 1 - Converting .CSV into a SQL Database file

The first step is to convert your .CSV files into an SQL friendly database file that ends in .DB.

I found multiple ways to do this. All of them involve creating SQL tables with defined fields, data types.

- Use a web application that converts file formats such as [Convertcsv.com](http://www.convertcsv.com/csv-to-sql.htm). This website is pretty straight forward, as they take you through the process step-by-step to generate a .DB file.

- If you're interested in having an actual database GUI where SQL files are properly displayed and visualized in tables and schemas I would highly recommend using [SQLite](https://sqlitebrowser.org/). This is a a light weight, open source database for small applications and projects. It's easy to download and set up. Go to the [download page](https://sqlitebrowser.org/dl/) and get the version that corresponds to your OS. After it's downloaded, open it and create a dummy table by clicking ```New Database``` and giving your .DB a name. Afterward you can import your CSV file into it. For visual assistance with this step, check out this [Youtube video](https://www.youtube.com/watch?v=TOqI-KiTBKU).


- A third option - which I employed - is to use this excellent application via command line converter: [GitHub](https://github.com/simonw/csvs-to-sqlite). It is made by Simon Willison, and I highly recommend his other data related repositories. To use it, you need to have python3 installed on your computer, then open up your command line and use the codes in the bottom portion of the GitHub. Then to convert your .CSV using the codes provided at the top of the README.


### Step 2 - Open Jupyter Notebook

If you don't know about Jupyter for Python, what are you even doing with your life?

*Just kidding*

If you don't have Jupyter Notebook, the easiest way would be to install [Anaconda](https://www.anaconda.com/distribution/). Again download the appropriate version: if you're Mac, Windows, Linux. After that's done, simply launch Jupyter Notebook. For an easy walkthrough of this process please watch this video: [Jupyter Notebook Installation](https://www.youtube.com/watch?v=sYH0LECSKSA).

### Step 3 - Making the Connection to your .DB

Finally! We're going to connect to your .DB file and query from there.

In this tutorial I used a .CSV that includes only two columns: the name of a city and its population. I will walk you through each of the steps needed to querying your .DB with SQL. Instead of listing it here, open up the [Jupyter Notebook file](https://github.com/mrjacklu/tutorials/blob/master/SQL%20Querying%20in%20Jupyter/SQL%20Querying%20in%20SQLite.ipynb).

You can find all the files to this tutorial on my [GitHub](https://github.com/mrjacklu/tutorials/tree/master/SQL%20Querying%20in%20Jupyter).

### Voila! You have learned how to change your .CSV into usable .DB file and then get a specific SQL query from it. And finally, downloading the file back into .CSV format in case in you want to make a visualization out of it.
