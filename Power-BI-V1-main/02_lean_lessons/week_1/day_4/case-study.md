<!-- # Case Study -->

## Introduction

<br>

Today we are going to work on a case study where we will see examples of how to apply what we have learned so far. It is important that you always have the business sense of the data that you have, and you will be able to be more exigent with information that you could get. The dataset we will be using is the **Liquor Sales** and you can get it from the resources folder **[Power BI resources](https://github.com/ironhack-edu/power-bi-resources)**.

<br>

## Challenge 1 - Modify data attributes

<br>

As we just loaded our dataset, we must validate all data that we have and start creating the fields that will help us to get our analysis to the next level. These are the missions:

- _INVOICE_, _STORE_, _ZIPCODE_, _CATEGORY_, _VENDOR NUM_, _ITEM NUM_ - Convert to STRING

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/case_study/to_string.png)

<br>

_([External link to the image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/case_study/to_string.png))_

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/case_study/to_string2.png)

<br>

_([External link to the image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/case_study/to_string2.png))_

<br>

- Ensure every other company is ok about data type
- Delete Address and Store Name Columns

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/case_study/delete.png)

<br>

_([External link to the image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/case_study/delete.png))_

<br>

- Create a column to calculate avg cost per bottle

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/case_study/avg_bottle.png)

<br>

_([External link to the image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/case_study/avg_bottle.png))_

<br>

## Challenge 2 - Using PowerQuery

<br>

On the power query we can get access to many options and formulas that will help us to develop our dashboard and manipulate our data in a "developer" mode:

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/case_study/power_query.png)

<br>

_([External link to the image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/case_study/power_query.png))_

<br>

- Create a copy of the original table

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/case_study/duplicate.png)

<br>

_([External link to the image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/case_study/duplicate.png))_

<br>

- Create a parameter with the following specifications:
  _ Type: Número decimal
  _ Values list:
  _ Default Value
  _ Actual value

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/case_study/param_1.png)

<br>

_([External link to the image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/case_study/param_1.png))_

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/case_study/param_2.png)

<br>

_([External link to the image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/case_study/param_2.png))_

<br>

- Right-click on the field to filter (for this case you must use Sale(Dollars)) and select filter by text, equal it to your parameter. It should filter your copy, when it happens just click on close and apply.
- Add a table to see how is the distribution of bottles that sold parameter bottles by Category Name and Count of bottles_sold and Sum of bottles_sold.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/case_study/filter.png)

<br>

_([External link to the image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/case_study/filter.png))_

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/case_study/filter2.png)

<br>

_([External link to the image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/case_study/filter2.png))_

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/case_study/filter3.png)

<br>

_([External link to the image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/case_study/filter3.png))_

<br>

## Challenge 3 - First Visuals

<br>

Using the dataset that hast the parameter applied, do the following:

- Add a line chart to see per Item Description the sales that each one has

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/case_study/line.png)

<br>

_([External link to the image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/case_study/line.png))_

<br>

- Add table to see how is the distribution of bottles that sold parameter bottles by Category Name and Count of bottles_sold and Sum of bottles_sold.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/case_study/table.png)

<br>

_([External link to the image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/case_study/table.png))_

<br>

- Create a bar char using your duplicated dataset. From this, use the bottles_sold and avg_per_bottle to see if you sell more bottles, the average is higher or lower

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/case_study/bar.png)

<br>

_([External link to the image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/case_study/bar.png))_

<br>

**HINT**: Be sure to show labels but modify them to have no format and only one decimal.
