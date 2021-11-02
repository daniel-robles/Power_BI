# Lesson 7.7 - Data Manipulation 2

<br><br>

### Lesson Duration: 4 hours

<br>

- **Purpose**: In this lesson, students will get more familiar with data manipulation with Power BI, learn how to conduct data transformations, create calculated fields and parameters. This topic also can be considered as a precursor to learning DAX (Data Analysis eXpressions), one of the most powerful features of Power BI.

<br>

## Pre-requisites

To successfully take this class, the students would need:

- Completed all previous lessons
- Installed Power BI Desktop
- Access to all datasets used in class and lab (students have access to this [repository](https://github.com/ironhack-edu/power-bi-resources) - liked to their Student Portal)

---

## Learning Objectives

After this lesson, students will be able to:

- Use more advanced approaches for data manipulation using Power BI
- Create calculated fields
- On an introductory level, work with mathematical functions (an introductory lesson for DAX functions)

<br><br>

### Session 1

> 🕰️ 40 min

#### Key Concepts

- More manipulation (simple data transformations) using Power BI
  - Using built-in functions for numerical data
  - Using built-in functions for text data
- Creating calculated fields (simple mathematical functions, operators, etc.)

<details>
<summary> Click for Session Detail: Power BI DAX Math Functions </summary>

<br>

## Power BI DAX Math Functions

> :exclamation: Note to the instructor: We will cover DAX in greater detail later, but for now, you can tell students they should think about them as a kind of calculated column.

You can use the "dax_math" file to check the math functions created, which are shown below.

The mathematical functions in Data Analysis Expressions (DAX) are very similar to the Excel mathematical and trigonometric functions. There is a lot of math function but we only review a few that are the most commonly used.

> :exclamation: Note to the instructor: For this activity, we will use the "employees.csv" file. Students will have this file available in the **[Power BI resources](https://github.com/ironhack-edu/power-bi-resources)** repository too. As you can see, there are only 15 records in this table.

To demonstrate the Power BI DAX Math functions, we are going to use the below-shown data:

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_1.jpg)

<br>

- Create a Matrix
- Add EmpID as a row.
- Add FirstName, LastName and S.ales columns as values.
- To demonstrate these DAX Math functions in Power BI, we have to use the calculated column.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_3.jpg)

<br>

In order to create a column, please click on the New Column option under the Power BI Home tab, or Modeling tab.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_2.jpg)

<br>

The following series of examples show you the use of DAX Math Functions in Power BI.

<br>

### Power BI DAX CEILING function

- The DAX Ceiling function in Power BI returns the closest value, which is greater than or equal to a given value.
- The syntax of this Power BI CEILING function is **`CEILING(Number, significance)`**.

As you can see from the below screenshot, we renamed the default column name to be CEIL. The below statement finds the closest integer value greater than or equal to Sales: `CEIL = CEILING(Employees[Sales], 1)`.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_4.jpg)

<br>

### Power BI DAX FLOOR function

- The Power BI DAX FLOOR function returns the closest value, which is less than or equal to a given value.
- The syntax of this Power BI DAX Floor function is **`FLOOR(expression, significance)`**.
- This Power BI DAX math function finds the closest value which is less than or equal to Sales: `FLOOR = FLOOR(Employees[Sales],1)`.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_5.jpg)

<br>

### Power BI DAX ROUND function

- The Power BI DAX ROUND function is to round the given values to the closest value.
- The syntax of this Power BI DAX Round function is **`ROUND(expression, significance)`**.
- It rounds the Sales values to the nearest integer: `ROUND = ROUND(Employees[Sales], 0)`.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_6.jpg)

<br>

### Power BI DAX CURRENCY function

- The DAX CURRENCY function in Power BI converts the value into the currency data type.
- The syntax of this Power BI DAX CURRENCY function is: **`CURRENCY(expression)`**.
- It converts the Sales values to Currency data type: `Money = CURRENCY(Employees[Sales])`.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_7.jpg)

<br>

### Power BI DAX INT function

- The DAX INT function in Power BI converts the given value into an integer data type.
- The syntax of this Power BI DAX INT function is: **`INT(expression)`**.
- Power BI DAX INT function converts the Sales values to Integer data type: `INT = INT(Employees[Sales])`.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_8.jpg)

<br>

### Power BI DAX SQRT function

- The DAX SQRT function in power BI returns the square root of a given number.
- The syntax of the Power BI DAX SQRT function is as shown below: **`SQRT(expression)`**.
- It returns the square root of a Sales column values: `SQRT = SQRT(Employees[Sales])`.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_9.jpg)

<br>

### Power BI DAX SIGN function

- The Power BI DAX SIGN function returns the sign of a given number. This function returns 1 for positive values, -1 for negative values, and 0 for zeros.
- The syntax of this Power BI DAX SIGN function is: **`SIGN(expression)`**.
- It returns the sign of the Service Grade column values: `SIGN = SIGN(Employees[SQRT])`.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_10.jpg)

<br>

### Power BI DAX POWER function

- The Power BI DAX POWER function finds the Power of a given number. This function accepts a second argument to specify the power value.
- The syntax of this Power BI DAX POWER function is **`POWER(expression, raise_number)`**.

For example Power(4, 3) = 4³.
The below statement returns the factorial of a yearly income divided by 1000: `POWER = POWER(Employees[Sales], 2)`.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_11.jpg)

<br>

### Power BI DAX RAND function

- The Power BI DAX RAND function returns the random positive number between 0 and 1.
- The syntax of the Power BI DAX RAND function is: **`RAND()`**.

Let's now create a new column to generate random values:`RAND = RAND()`.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_12.jpg)

<br>

### Power BI DAX RANDBETWEEN function

- The DAX RANDBETWEEN function in Power BI returns the random number between the user-specified start and end values.
- The syntax of the Power BI DAX RANDBETWEEN function is: **`RANDBETWEEN(start, end)`**.

Let's create a new column to generate random values between 10 and 50:`RANDBET = RANDBETWEEN(10, 50)`.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_13.jpg)

<br>

### Power BI DAX TRUNC function

- The Power BI DAX TRUNC function truncates the given number to an integer by removing the decimals.
- The syntax of the Power BI DAX TRUNC function is: **`TRUNC(number, num_of_digits)`**.

This Power BI DAX math function truncates the Sales column values: `TRUNC = TRUNC(Employees[Sales], 1)`.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_14.jpg)

<br>

### Power BI DAX ROUNDDOWN function

- The Power BI DAX ROUNDDOWN function rounds down the given number towards a zero.
- The syntax of the Power BI DAX ROUNDDOWN function is: **`ROUNDDOWN(number, num_of_digits)`**.

It rounds down the Sales column values to 2 digits: `ROUNDDOWN = ROUNDDOWN(Employees[Sales], -2)`.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_15.jpg)

</details>

#### :pencil2: Check for Understanding - Class activity

> 🕰️ 10 min (+ 10 min Review)

<details>
  <summary> Click for Instructions: Activity 1 </summary>

<br>

Do the research and share with the class:

- What is DAX in Power BI?
- How is it useful?

</details>

<details>
  <summary>Click for Solution: Activity 1 solutions</summary>

Data Analysis Expressions (DAX) is a library of functions and operators that can be combined to build formulas and expressions in Power BI, Analysis Services, and Power Pivot in Excel data models.

Here are is official [DAX documentation](https://docs.microsoft.com/en-us/dax/) and the [DAX overview](https://docs.microsoft.com/en-us/dax/dax-overview), both by Microsoft.

</details>

---

:coffee: **BREAK**

> 🕰️ 10 min

---

### Session 2

> 🕰️ 40 min

#### Key Concepts

Grouping Data

- Using grouping
- Using binning

<details>
<summary> Click for Session 2 Details: Grouping Data </summary>

<br>

### Using Grouping

For this session, we’ll be using "retail_analysis_sample.pbix" (available in the `files_for_lessons_and_activities` folder).

- To start, focus your attention on the "Total Sales Variance % by FiscalMonth" clustered column chart found on the "District Monthly Sales" report.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_group1.jpg)

<br>

Now, let’s say you would like to group the sales variance on every first month of the quarter — January, April, and July.

- To start, select all of them by pressing `Ctrl+click`
- This will allow you to multi-select elements on the canvas.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_group2.jpg)

<br>

- Then, right-click on any of the points.
- Select ‘Group data’ from the options.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_group3.jpg)

<br>

Easy :wink:

<br>

### Editing Groups

In Power BI, you can modify existing groups as much as you like.

- To edit any group, right-click on its field either on the "Legend" bucket or on the Fields list (both works).
- Then, select "Edit groups" from the options.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_group4.jpg)

<br>

- You’ll then see another box open up.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_group5.jpg)

<br>

- All you have to do is click the value first, then the group where you would like to add the value.
- Then, click the ‘Group’ button below.

</details>

<details>
<summary> Click for Session 2 Details: Binning Data </summary>
  
 ### Using Binning

- Using the same visualization, delete the Axis column.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_group6.jpg)

<br>

- Now let’s create groups of people based on their yearly income categorized in buckets of two months.
- Right-click on the column name in the fields section:

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_group7.jpg)

<br>

- Select Group.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_group8.jpg)

<br>

- In the Groups window make sure Bin is selected as the group type (by default for numeric or date/time columns this will be the default).

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_group9.jpg)

<br>

- And set the size to 2 Months. This is the size that values of YearlyIncome will be split based on it.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_group10.jpg)

<br>

- Now we have created a new field.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_group11.jpg)

<br>

- If we drag this new field, this is what we have:

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_group12.jpg)

</details>

#### :pencil2: Check for Understanding - Class activity

> 🕰️ 10 min (+ 10 min Review)

<details>
  <summary> Click for Instructions: Activity 2 </summary>

> :exclamation: Note for the instructor: We have not covered DateTime functions yet, but we will in the next session. Please let the students know that the idea behind this activity is to make students get comfortable with the official documentation of Power BI. At this point, students should be able to understand the use of simple predefined functions on Power BI by looking at the documentation.

<br>

The purpose of this activity is to get students to become as familiar as possible with the official documentation.

Go through the official documentation of Power BI from Microsoft and read about Date Functions and Date Time Functions.
Read about some functions and see how they are implemented in Power BI.

</details>

<details>
  <summary>Click for Solution: Activity 2 solutions</summary>

Refer the links below:

- [Date functions](https://docs.microsoft.com/en-us/powerquery-m/date-functions)
- [DateTime functions](https://docs.microsoft.com/en-us/powerquery-m/datetime-functions)

</details>

---

:coffee: **BREAK**

> 🕰️ 10 min

---

### Session 3

#### Key Concepts

> 🕰️ 40 min

- Top N analysis using Visual Filters
- Date time functions

:exclamation: Note to the Instructor: We will cover DAX in more detail on Day 1 Week 2. So this lesson on DAX is just a quick overview. If the students are confused about how to use DAX, ask them to wait till next week when we have complete sessions on DAX.

<details> 
<summary> Click for Details: TOP N VISUAL FILTERS </summary>

<br>

### TOP N Visual Filters

The visual-level filters of a visual in Power BI allow you to reduce the number of elements in a visual. This approach makes it very easy to apply a filter to the top 10 products in a report, according to the selection required in other slicers or visuals.

> :exclamation: Note for instructor: We will continue using the "retail_analysis_sample.pbix" file.

- Open "This year Sales" visualization in the "District Monthly Sales" tab

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_top1.jpg)

<br>

- Go to filters > Visual level filters

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_top2.jpg)

<br>

- Select the filter type: TOP N
- Now, select the number of objects you want to see in your visualization

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_top3.jpg)

<br>

- Drag the type of data fields

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_top4.jpg)

<br>

- Apply filters

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_top5.jpg)

</details>

<details>
<summary> Click for Details: DateTime Functions</summary>
  
<br>

## Date time functions

These functions help you create calculations based on dates and time. Many of the functions in DAX are similar to the Excel date and time functions. However, DAX functions use a date-time data type and can take values from a column as an argument.

### DATE

- Returns the specified date in datetime format.
- Syntax: **`DATE(<year>, <month>, <day>)`**

- Definitions of terms:
  - _year_ - A number representing the year.
  - _month_ - Negative integers are not supported. Valid values are 1-12.
  - _day_ - Negative integers are not supported. Valid values are 1-31.

### DATETIFF

- Returns the count of interval boundaries crossed between two dates.
- Syntax: **`DATEDIFF(<start_date>, <end_date>, <interval>)`**

### DATEVALUE

- Converts a date in text format to date in DateTime format.
- Syntax: **`DATEVALUE(date_text)`**

### DAY

- Returns the day of the month, a number from 1 to 31.
- Syntax: **`DAY(<date>)`**

### EDATE

- Returns the date that is the indicated number of months before or after the start date.
- Use EDATE to calculate maturity dates or due dates that fall on the same day of the month as the date of issue.
- Syntax: **`EDATE(<start_date>, <months>)`**

### EOMONTH

- Returns the date in DateTime format of the last day of the month, before or after a specified number of months.
- Use EOMONTH to calculate maturity dates or due dates that fall on the last day of the month.
- Syntax: **`EOMONTH(<start_date>, <months>)`**

### HOUR

- Returns the hour as a number from 0 (12:00 A.M.) to 23 (11:00 P.M.).
- Syntax: **`HOUR(<datetime>)`**

### MINUTE

- Returns the minute as a number from 0 to 59, given a date and time value.
- Syntax: **`MINUTE(<datetime>)`**

### MONTH

- Returns the month as a number from 1 (January) to 12 (December).
- Syntax: **`MONTH(<datetime>)`**

### NOW

- Returns the current date and time in DateTime format.
- The NOW function is useful when you need to display the current date and time on a worksheet or calculate a value based on the current date and time, and have that value updated each time you open the worksheet.
- Syntax: **`NOW()`**

### TODAY

- Returns the current date.
- Syntax: **`TODAY()`**

</details>

---

:coffee: **BREAK**

> 🕰️ 5 min

---

#### :pencil2: Check for Understanding - Class activity

> 🕰️ 10 min (+ 10 min Review)

<details>
  <summary> Click for Instructions: Activity 3 </summary>

<br>

In this activity we will jump back to `financial_sample.xlsx` file.

- Create a Top N filter to find the top 2 products by sale value.

Here is what the output would look like.

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/week1_day4_activity3.png)

</details>

<details>
  <summary>Click for Solution: Activity 3 solutions</summary>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/week1_day4_activity3_solution.png)

</details>

---

:sandwich: **LUNCH BREAK**

> 🕰️ 60 min

---
