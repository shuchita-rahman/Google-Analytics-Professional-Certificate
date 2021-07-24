
# Learning Objectives
* Discuss the use of data in the decision-making process.
* Compare and contrast data-driven decision making with data-inspired decision making.
* Explain the difference between quantitative and qualitative data including reference to their use and specific examples.
* Discuss the importance and benefits of dashboards and reports to the data analyst with reference to Tableau and spreadsheets.
* Differentiate between data and metrics, giving specific examples.
* Demonstrate an understanding of what is involved in using a mathematical approach to analyze a problem.


# 1. Understand the Power of Data
We know data is a collection of facts. Data Analysis reveals patterns and insight into that facts. Then business takes those insights to make a decision.  **Decision-making** processes from data are two types:
1. **Data-driven** decision making.
2. **Data-inspired** decision making.

In this reading, we will learn about data-driven decision making. 

## 1.1 Data Trials and Triumphs
The goal of all data analysts is to use data to draw accurate conclusions and make good recommendations. That all starts with having complete, correct, and relevant data. 

But keep in mind, it is possible to have solid data and still make the wrong choices. It is up to data analysts to interpret the data accurately. 

When data is interpreted incorrectly, it can lead to huge losses. Consider the examples below.

#### **Mars Orbiter Loss**

In 1999, NASA lost the $125 million Mars Climate Orbiter, even though it had good data. The spacecraft burned to pieces because of poor collaboration and communication. The Orbiter’s navigation team was using the SI or metric system (newtons) for their force calculations, but the engineers who built the spacecraft used the English Engineering Units system (pounds) for force calculations. 

No one realized a problem even existed until the Orbiter burst into flames in the Martian atmosphere. Later, a NASA review board investigating the root cause of the problem figured out that the issue was isolated to the software that controlled the thrusters. One program calculated the thrusters’ force in pounds; another program looking at the data assumed it was in newtons. The software controllers were making data-driven decisions to adjust the thrust based on 100% accurate data, but these decisions were wrong because of inaccurate assumptions when interpreting it. A conversion of the data from one system of measurement to the other could have prevented the loss.

#### Coke launch failure
In 1985, New Coke was launched, replacing the classic Coke formula. The company had done taste tests with 200,000 people and found that test subjects preferred the taste of New Coke over Pepsi, which had become a tough competitor. Based on this data alone, classic Coke was taken off the market and replaced with New Coke. This was seen as the solution to take back the market share that had been lost to Pepsi. 

But as it turns out, New Coke was a massive flop and  the company ended up losing tens of millions of dollars. How could this have happened with data that seemed correct? It is because the data wasn’t complete, which made it inaccurate. The data didn't consider how customers would feel about New Coke replacing classic Coke. The company’s decision to retire classic Coke was a data-driven decision based on incomplete data.

## 1.2 Type of Data
The main intention of data visualization is to find out a summary of the data. Our data summer will be different depending on the data type. Suppose a store has customer information database where they these information about their customers *Name, Age, Sex, Address, Weekly_Visit,Salary, Children, Review*, etc.  Here we easily can see that data all is not numeric. Here **Age** is a numerical value but **Sex**, **Address** is not numerical value. If we want to know the **average age** of the customer we can easily find out by adding the Age column then dividing it with number of customers.We can’t do the same thing for **Sex**, or **Address**. So for different types of data we need to come up with different approach. 
There are **two types** of data/variables:

![](variableType.png)  

### Quantitative Data:   
>**Data which deal with number or which have objective and specific measures is called quantitative data.**

This can often be 
  *  The what?
  * How many?
  * How often?
  
Ex: Age, Height, Salary.
   
   
* **Discrete Data:** Just like the name Discrete data are distinct or individual value. We can count Discrete data but we can’t measure it. Discrete data are integer value. For instance,
**How many children do you have?**
The answer can be 0, 1, 3,or, 5. But you can’t have 2.5 children. **It has to be distinct value.** 
In store database, **Weekly Visit** are Discrete Quantitative data.

* **Continuous Data:** Continuous data are those numerical data which can be measured but can not be counted. This type of data can be divided or reduced.Example : Height, Weight. 
In store database **Age**, **Salary** are Continuous Quantitative Data.

### Qualitative/ Categorical Data:
>**Data which have subjective or explanatory measures of qualities and characteristics are called Qualitative/ Categorical Data.**

Ex: Gender, Hair color, Language, etc.
    
* **Nominal Data:** When data is labeled or assigned is called nominal data. Nominal doesn’t have ordered, if we change the sequence it doesn’t change the data meaning. Ex: Suppose tell us the list of natural hair colors? Blonde, Black, Red, etc. 
In store database, **Sex** is Nominal Qualitative Data.

* **Ordinal Data:** Ordinal data are those which represent a distinct value but also maintain an order. Ex: T-shirt size Small, Medium, Large.   
In store database, **Service_Review**(Poor, Average, Satisfied) is a Ordinal Qualitative Data.

# 1.3 Quantitative and Qualitative Data in Action

A local ice cream shop has started using their online reviews to engage with their customers. The owner notices that their rating has been going down. He sees that lately his shop has been receiving more negative reviews. He wants to know why,
He come up with this approach.

**Step-1:** He started to ask questions that lead to quantitative Data.
* How many negative reviews are there? 
  **Ans : 50**
* What's the average rating?
  **Ans: 3.5**
* How many of these reviews use the same keywords? **Ans: 20**

>**Outcome:** The owner understand customers aren't happy.

**Step-2:** From the outcome of the step-1 he decided to ask more question which lead to qualitative data.
* Why are customers unsatisfied? **Ans: Frustrated**
 > **Outcome:** 20 reviews use the word *frustrated*.

**Step-3:** From the outcome of the step-2 owner decided to gather more qualitative data.
* why this word is being repeated?
* How can we improve their experience?

> **Outcome:** He finds out that customers are frustrated because the shop is running out of popular flavors before the end of the day.

Solution: **The ice cream shop change their  weekly order to make sure it has enough of what the customers want.**

# [ 1.4 Qualitative and Quantitative data in Business](https://www.coursera.org/learn/ask-questions-make-decisions/supplement/q79uq/qualitative-and-quantitative-data-in-business)

![](Qualitative_Quatitative.png)
Source : [https://www.coursera.org/learn/ask-questions-make-decisions/supplement/q79uq/qualitative-and-quantitative-data-in-business](https://www.coursera.org/learn/ask-questions-make-decisions/supplement/q79uq/qualitative-and-quantitative-data-in-business)

# 1.5 Learning Log: Ask SMART questions about real-life data sources

#### Overview
In a previous [self-reflection](https://github.com/shuchita-rahman/Google-Analytics-Professional-Certificate/blob/main/Ask%20Questions%20to%20Make%20Data-Driven%20Decisions/Week%20-%201/README.md#solutions), you prepared for a “data conversation” with someone in your life by creating SMART questions to help you understand more about the data they usually interact. Now, you’ll complete an entry in your learning log to reflect on that conversation and how you might approach this data for a real project.

#### Review Note
Before you begin your new entry, take a moment to locate and read the [Learning Log](https://github.com/shuchita-rahman/Google-Analytics-Professional-Certificate/blob/main/Ask%20Questions%20to%20Make%20Data-Driven%20Decisions/Week%20-%201/README.md#solutions) you took during your data conversation. Based on the answers to your well-prepared SMART questions, you should have a better context for your target audience now. Review those answers and start thinking about the following:

* Stakeholder’s business goals. Here, the person you had a conversation with. 
* Identifying the data needed to answer the **SMART** questions
* Exploring what data the stakeholder already has.

Determining the data that you don’t have, but need in order to answer the questions

#### [Solution]()
# 2. Follow the Evidence
## 2.1 Sharing the Data
You have the analysis of your data. Now you want to share it with the Stakeholders. Depending on the Stakeholders you will display the analysis so that, they can easily understand it. Here are two ways to show your analysis. 
1. **Report:**  A report is a static collection of data given to stakeholders periodically.
2. **Dashboard:** A dashboard is monitors live, incoming data.

### Report

| Pros                       | Cons                   |
|----------------------------|------------------------|
| High level historical Data | Continual maintenance |
| Easy to design |Less visually appealing |
|Pre-cleaned and sorted data  | Static |

Example: Here is a covid-19 dataset. You can see their are lot of data and we don't know where to look. To share the death report we can use pivot table.

![](covid.png)

### Dashboard
| Pros                       | Cons                   |
|----------------------------|------------------------|
| Dynamic, automatic and interactive | Labor-intensive design |
| More stakeholders access |Can be confusing |
|Low maintenance  | Potentially uncleaned data. |

## 2.2 Data versus Metrics
Data is useful after turning it into a piece of information. To turn the data into information we use metrics.  

> **Metric:** Single, quantifiable data that can be used for measurement. 

Data starts as a collection of raw facts, until we organize them into individual metrics that represent a single type of data. Metric can be formula you use.
For instance, a teacher wants to understand how his students are performing in a particular subject. He gathers all students grades and made a frequency table from that

| Mark             | Number of Students (total 80) |
|------------------|-------------------------------|
| mark  <  50 | 20                            |
|  50 > mark <  80 | 50                           |
| 80 > mark  <  100 | 10                            |

From the table teacher can find out that most of the students performance is average point.
These frequency table is used as a metric to understand the students performance.

# 2.3 [Designing Compelling Dashboards](https://www.coursera.org/learn/ask-questions-make-decisions/supplement/Jvsne/designing-compelling-dashboards)
# 3. Connecting the Data Dots
## 3.1 Mathematical Thinking
You already learn different processes of thinking. Now you will know how **mathematical thinking** bring new information to the table. For mathematical thinking, you don't have to become a mathematician suddenly.  It means looking at a problem and breaking it logically down step-by-step to find a new solution.
For instance, You are a homeroom teacher of a class. You have all the marks of 80 students in English and Maths. You want to know which subject you should teach your students more.  
So for this, you think mathematically. You made a frequency table and categorized student performance.
>  Divide the number of categories/values into intervals, then count the number of results in each interval

| Marks          | English | Math |
|----------------|---------|------|
| mark =< 50     | 10      | 30   |
| 50 > mark < 80 | 40      | 40   |
| mark => 80     | 30      | 10   |

From this table you can come up with the solution to teach your students math more to increase their performance.

## 3.2 [Small Data and Big Data.](https://www.coursera.org/learn/ask-questions-make-decisions/supplement/VAdzR/big-and-small-data)

 


