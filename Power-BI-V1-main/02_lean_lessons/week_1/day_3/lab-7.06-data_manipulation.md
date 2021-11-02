<!-- # Lab | Data Manipulation -->

## Introduction

As a data analyst, you will have to work with a big amount of data and different data types. Extracting meaningful insights from your data can be done by using all data sources available and learning how this could be achieved in a correct way using a BI Tool. In this lab, you will use Power BI to load multiple datasets into it, validate that data was correctly loaded, and perform simple manipulations using the PowerBI interface.

Download the **Financial and Population dataset from Resources Folder**. Once you download the files, save them in a folder of your preference.

### Prerequisites

- At this point, you should have installed Power BI on your laptop

If you have any doubts about the prerequisites, please clarify with your instructor or teaching assistants.

<br>

## Challenge 1 - Create Calculated Fields

<br>

In this challenge, we will practice creating calculated columns and modifying data types. These guidances are helpful to train your problem-solving thinking and to learn how to work around problems.
To solve this problem, you need to keep the following points in mind:

- We need to create these fields which will make us easier to perform the next challenge
- Be careful with data types, check all possible incorrect ones, and change them to avoid wrong calculations (ex. Currency in Text type)

Therefore, you will not be able to achieve challenge 2 without these fields. Below is an overview of the steps:

- Calculate the concatenated field that contains the Country and Year for both datasets:
  - the calculated field that returns the following
    - Example:
      ```
      Mexico - 2021
      ```
- Create the field of the population in terms of millions
  - your calculation should be like _field_ operation. Save it as a new column.
- Get the month of the date in a column called Month Number
  - Identify the DateTime field in the Financial Sample dataset
  - Extract the month of this field and save it into a new column
- Similar to the previous one, you need to calculate the Year of the Date field
  - Extract the year of the original field and save it into a new column

<br>

## Challenge 2 - First Data Analysis

<br>

In the previous challenge, you have created the primary keys to join both tables. Now is time to start with our data analysis so we have to create the relation between the two datasets using de field ID to just create:

- The relationship must be many to one from Financial Sample to Population.
  - The key from Financial Sample must be unique
  - The key from Population could have duplicates
- The cross filter must be in both directions
  - The relationship must be configured like this:
    - Cardinality: Many to one
    - Direction: Both sides

Once you set the relationship, you must create these visualizations using PowerBI and, after that, you'll be able to explain your raw datasets into beautiful graphics that give us a better context of the whole bunch of information:

- Pie Chart: You need to create a Pie chart that shows us the Profits per Segment (Financial Dataset). Show only the top 5 segments and the labels for each slice (Label Amount – the percentage of total)

  - Filter the top 5 segments by SUM of profit
  - Modify the detail labels of the chart to show something like this:
    - Total data value, percentage of importance

- Bar Chart: Create a Horizontal bar chart where you can see per Country Field (Financial Dataset), how is distributed the population of males and females. Modify the legend name of the bar chart and show the total percentage of all your data.
- Table: Create a table where you’re able to visualize per Location in Population, the SUM of Units Sold, and the MEAN of Discounts. Be sure to be ordered by Units sold descendent

- Slicer: Create a slicer that makes you filter by specific Country in the financials dataset. Be sure that this one filters each graph that you just did.
