
# Learning Objectives

* Describe spreadsheets, query languages, and data visualization tools, giving specific examples.
* Demonstrate an understanding of the uses, basic features, and functions of a spreadsheet.
* Explain the basic concepts involved in the use of SQL including specific examples of queries.
* Identify the basic concepts involved in data visualization, giving specific examples.

# Introduction 
We already know about the data life cycle, and process data need to go through to find an answer. Now in this week, we will learn about the tools a data analyst use in those process. We will learn about spreadsheets, SQL in action. It's okay if you don't know the basics of these tools. We will learn the ins and out of these tools this week.

# 1.Mastering Spreadsheets Basics

## 1.1 Phases of the data life cColumns and rows and cells, oh my!
**Adding data to spreadsheet:**

---------------------------------------------------------

![PNG](Data.PNG)
---------------------------------------------------------



**Sort Data**

> Choose the column -> Data -> Ascending/Descending

---------------------------------------------------------

![](Data.PNG)
---------------------------------------------------------

![](sort.png)
---------------------------------------------------------

![](age_Sort.png)
---------------------------------------------------------


**Formula**

>A formula is a set of instructions that performs a specific calculation using the data in a spreadsheets.

---------------------------------------------------------


![](averageFormula.png)

---------------------------------------------------------

![](ave.png)

---------------------------------------------------------

![](ans.png)

---------------------------------------------------------


# 1.2 More spreadsheet resources

In the spirit of lifelong learning, it is good to have resources to turn to when you want to know more about using spreadsheets. Two of the most well known and used spreadsheet platforms are Google Sheets and Microsoft Excel. Both provide free online training resources that you can access anytime you need them. Bookmark these links if you want to access them later.

[Google Sheets Training and Help](https://support.google.com/a/users/answer/9282959?visit_id=637361702049227170-1815413770&rd=1)

Learn even more ways to move, store, and analyze your data with the Google Sheets Training and Help page, located in the Google Workspace Learning Center.This hub offers an expanded list of tips, from beginner to advanced, along with cheat sheets, templates, guides, and tutorials. 

[Google Sheets Cheat Sheet
](https://support.google.com/a/users/answer/9300022)

Want to learn more about Google Sheets? This online help article features a short list of the most important functions you will use, including rows, columns, cells, and functions. 

[Microsoft Excel for Windows Training](https://support.microsoft.com/en-us/office/excel-for-windows-training-9bc05390-e94c-46af-a5b3-d7c22f6990bb)

Get to know Excel spreadsheets a little better by visiting this free online training center. Offering everything from a quick-start guide and introduction to tutorials and templates, you will find everything you need to know, all in one place.

# 2. Structured Query Language(SQL)
## 2.1 SQL in action
SQL can do all of the things that spreadsheet can do. For larger scale SQL is better than spreadsheets. SQL needs a database that will understand its language. Let's talk. There are a number of databases out there that use SQL.
Example 
* Oracle
* MySQL
* PostgreSQL
* Microsoft SQL Server
* MongoDB

To communicate with database SQL use **Query**. Query structure is universal. So no matter which database you use your query would be similar.

![](queryStucture.png)
Source : [https://www.coursera.org/learn/foundations-data/lecture/dPBUG/sql-in-action](https://www.coursera.org/learn/foundations-data/lecture/dPBUG/sql-in-action)

## 2.2 More about SQL 
**Basic syntax for SQL**
Every programming language, including SQL, has to follow a unique set of guidelines known as syntax. As soon as you enter your search criteria using the correct syntax, the query should start working to pull the information you have requested from the target database.

**What is a query?**

A query is basically a request for data or information from a database. For example, ''Tell me how many comedy movies were made in 1985” or ''How many people live in Puerto Rico?'' When we query databases, we use SQL to communicate our question or request. Both the user and the database can always exchange information as long as you “speak” the same language.

**The foundation of every SQL query is the same:** 

*  **SELECT** to choose the columns you want to return.
*  **FROM** to choose the tables where the columns you want are located.
*  **WHERE** to filter for certain information.

![](SQL_Basic.png)

**Tip 1:** You can write your SQL queries all in lowercase and don’t have to worry about proper spacing between words. With that said, however, using capitalization and spacing can help you read the information more easily. Keep your queries neat, and they will be easier to review or troubleshoot if you need to check them later on.


In the SQL syntax shown above, the SELECT clause identifies the column you want to pull data from by name, field1, and the FROM clause identifies the table in which the column is located by name, table. Finally, the WHERE clause narrows your query so that the database returns only the data with an exact value match or the data that matches a certain condition that you want. 

For example, if you are looking for a specific customer with the last name Chavez, the WHERE clause would be: WHERE field1 = 'Chavez';

However, if you are looking for all customers with a last name that begins with the letters “Ch”, the WHERE clause would be: WHERE field1 LIKE 'Ch%';

You can see that the LIKE clause is very powerful because it allows you to tell the database to look for a certain pattern! The percent sign (%) is used as a wildcard to match one or more characters. In our example, both Chavez and Chen would be returned. Note that in some databases the asterisk (*) is used as the wildcard instead of the percent sign (%).

**Can you use  SELECT * ?**
In the example, if you replace SELECT field1 with SELECT *  you would be selecting all the columns in the table. From a syntax point of view, it is a correct SQL statement, but you should use it sparingly and with caution because depending on how many columns a table has, you could be selecting a tremendous amount of data.

Finally, you will notice that we have shown the SQL statement with a semicolon at the end. The semicolon is a statement terminator and is part of the American National Standards Institute (ANSI) SQL-92 standard which is a recommended common syntax for adoption by all SQL databases. However, not all SQL databases have adopted or enforce the semicolon, so it’s possible you may come across some SQL statements that aren’t terminated with a semicolon. If a statement works without a semicolon, it’s fine.

**Tip 2:** Some tables aren’t designed with descriptive enough naming conventions. In our previous example, field1 was the column for a customer’s last name, but you wouldn’t know it by the name. A better name would have been something like last_name. In these cases, you can place comments alongside your SQL statements to help you remember what the name represents. Comments are text placed between certain characters, /* and */, or after two dashes (--) as shown below. 

![](d.png)!


Tip 3: You can also make it easier on yourself by assigning a new name or alias to the column or table names to make them easier to work with (and avoid the need for comments). This is done with a SQL AS clause. In the example below, you are changing field1 to last_name and table to customers for the duration of the query only. It doesn’t change the names in the actual table used in the database.



![](table.png)

Image of a screen shot with alias examples: field1 AS last_name and table AS customers. Each alias has a comment with --.

![](a.png)

**Putting SQL to work**
Imagine you are a data analyst for a small business and your manager asks you for some employee data. You decide to write a query with SQL to get what you need from the database. 

You want to pull all the columns: empID, firstName, lastName, jobCode, and salary. Because you know the database isn’t that big, instead of entering each column name in the SELECT clause, you use SELECT *.  This will select all the columns from the Employee table in the FROM clause.

SELECT* FROM Employee
Now, you can get more specific about the data you want from the Employee table. If you want all the data about employees working in the SFI job code, you can use a WHERE clause to filter out the data based on this additional requirement. 

Here, you use:

![](quer.png)


![](table_uery.png)

# 3. Data Visualization
## 3.1 Planning a data visualization

Earlier, you learned that data visualization is the graphical representation of information. As a data analyst, you will want to create visualizations that make your data easy to understand and interesting to look at. Because of the importance of data visualization, most data analytics tools (such as spreadsheets and databases) have a built-in visualization component while others (such as Tableau) specialize in visualization as their primary value-add. In this reading, you will explore the steps involved in the data visualization process and a few of the most common data visualization tools available. 

### **Steps to plan a data visualization**:

Imagine you’re a data analyst for a clothing distributor. The company helps small clothing stores manage their inventory, and sales are booming. One day, you learn that your company is getting ready to make a major update to its website. To guide decisions for the website update, you’re asked to analyze data from the existing website and sales records. Let’s go through the steps you might follow.

##### **Step 1:** Explore the data for patterns
First, you ask your manager or the data owner for access to the current sales records and website analytics reports. This includes information about how customers behave on the company’s existing website, basic information about who visited, who bought from the company, and how much they bought.

While reviewing the data you notice a pattern among those who visit the company’s website most frequently: geography and larger amounts spent on purchases. With further analysis, this information might explain why sales are so strong right now in the northeast—and help your company find ways to make them even stronger through the new website.

##### Step 2: Plan your visuals

Next it is time to refine the data and present the results of your analysis. Right now, you have a lot of data spread across several different tables, which isn’t an ideal way to share your results with management and the marketing team. You will want to create a data visualization that explains your findings quickly and effectively to your target audience. Since you know your audience is sales oriented, you already know that the data visualization you use should:

* Show sales numbers over time
* Connect sales to location
* Show the relationship between sales and website use
* Show which customers fuel growth

##### Step 3: Create your visuals
Now that you have decided what kind of information and insights you want to display, it is time to start creating the actual visualizations. Keep in mind that creating the right visualization for a presentation or to share with stakeholders is a process. It involves trying different visualization formats and making adjustments until you get what you are looking for. In this case, a mix of different visuals will best communicate your findings and turn your analysis into the most compelling story for stakeholders. So, you can use the built-in chart capabilities in your spreadsheets to organize the data and create your visuals.

### Build your data visualization toolkit
There are many different tools you can use for data visualization. 

**Spreadsheets** (Microsoft Excel or Google Sheets)

 Spreadsheets are great for creating simple visualizations like bar graphs and pie charts, and even provide some advanced visualizations like maps, and waterfall and funnel diagrams.
But sometimes you need a more powerful tool to truly bring your data to life. Tableau and RStudio are two examples of widely used platforms that can help you plan, create, and present effective and compelling data visualizations.

**Visualization software (Tableau)**

 Tableau offers built-in visual best practices, which makes analyzing and sharing data fast, easy, and useful. Tableau works well with a wide variety of data and includes an interactive dashboard that lets you and your stakeholders click to explore the data interactively. 

**Programming language (R with RStudio)** 

Most people who work with R end up also using RStudio, an integrated developer environment (IDE), for their data visualization needs. As with Tableau, you can create dashboard-style data visualizations using RStudio.

**Key takeaway**

The best data analysts use lots of different tools and methods to visualize and share their data. As you continue learning more about data visualization throughout this course, be sure to stay curious, research different options, and continuously test new programs and platforms to help you make the most of your data. 



