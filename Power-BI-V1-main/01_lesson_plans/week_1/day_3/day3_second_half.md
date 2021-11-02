# Lesson 7.6 - Statistics in Power BI

<br><br>

### Lesson Duration: 4 hours (including Lab)

<br>

- **Purpose**: In this lesson, students will learn how to identify and manage data inconsistencies using Power BI. The inconsistencies or irregularities can be either in numerical data or categorical data or both. The students will see implementation of some basic descriptive statistics that we learnt in the previous class.

- **(Additional Content)** - We will also talk about the drill down and drill up feature in Power BI which is really useful to conduct a deep dive analysis.

<br>

## Pre-requisites

To successfully take this class, the students would need:

- Completed all previous lessons
- Power BI desktop
- Access to all datasets used in class and lab (students have access to this [repository](https://github.com/ironhack-edu/power-bi-resources) - liked to their Student Portal)

---

## Learning Objectives

After this lesson, students will be able to:

- Perform data cleaning, remove data inconsistencies
- Create visualizations
- Use drill down and drill up feature (**Additional Content**)

> :exclamation: Note for instructor: The additional content is added here. You can use your discretion to take up this topic now or later as well.

<br><br>

### Session 1

> 🕰️ 40 min

#### Key Concepts

- Resolve data quality issues with numerical and categorical data
- Resolve inconsistencies
- Unexpected or null values, and data quality issues
- Create visualizations (could be repeat of the kind of plots that the students have seen already or some other plots)

<details>
<summary> Click for session details: Resolve data inconsistencies with numerical and categorical data </summary>

<br>

### Resolve data inconsistencies with numerical and categorical data

Errors messages can appear in a variety of places such as in the Queries & Connections pane, within the Power Query Editor, or maybe just as a value in a field.

#### We have grouped errors into three types:

- Process creation errors
- Software bugs
- Data processing errors

### Process creation errors

Process creation errors occur as we to build our query. These are driven by either errors in the `M` code, or users not understanding how Power Query operates.
**Note**: `M` can be considered as a query formula language and it can be used in the Power BI Query Editor in order to prepare data before it can be loaded into the Power BI model. This is beyond the scope of this class and the students can learn about `M` code later in their own time.

### Custom Columns

Custom Columns contain a warning at the bottom of the screen to help guide us with our formulas. Unless we’ve been working with Power Query for a while, we won’t understand what many of these messages mean, and even then, those error messages can be confusing.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3_error6.jpg)

<br>

The screenshot above shows the `Token RightParen` expected message. This is just one of many potential messages. As we type into the formula box, the message will change. Therefore, it is not worthing looking at this message until we think the formula finished. If the Show error option is visible, we can click it to take us to exactly where the problem is.

<br>

Once you know what the messages mean they are not as difficult as might seem. The most common warnings you’ll come across are:

- _Token Literal expected_ means the next thing in the formula is expected to be a value, column name, or a function.
- _Token Then expected_, or _Token Else expected_ means the words then or else are expected to be entered next. These will appear when writing an if statement.
- _Token RightParen_ expected means that a closing bracket, or parentheses depending on your local vernacular, is expected to close a formula.
- _A Comma cannot precede a RightParen_ means what it says; a comma can not be directly in front of a closing bracket, there are no circumstances in M where this should be necessary.
- _Invalid literal_ indicates there is an issue with the value entered as the literal (this often occurs when a test string has not been closed using the double quotation character.
- _Token EoF expected_ usually occurs when an invalid function name is used, or it uses the wrong case (for example, if is a valid command, while If with an upper case I is invalid).
- _The formula is incomplete_ is usually an indication that no formula has been entered (only the equals symbol in the formula box).

### Software bugs

As Power Query is continually being updated, bugs can come and go quickly as newer versions are released. Now, the software has become robust and now rarely suffers from issues.

### Data processing errors

#### Data type

Data type errors will not prevent the data loading into the query; instead, those cells will be loaded as blank.

Data type errors occur when:

- Data is converted from one type to another – for example, trying to change a text string into a decimal data type.
- Incorrect data types is used within functions – for example trying to use a number function on a text data type, or trying to multiply non-numeric data types

Let's try loading the next file as a Data Source as an easier example.

**Note**: The following instructions will only work for data processing errors.

- Download `error_test.xls` file
- Load it as a data source

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3_error2.jpg)

<br>

- Before clicking on "Load", click "Transform Data" button
- Change "Sales" column by right click over column name --> Change Type --> Whole number

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3_error3.jpg)

<br>

- Now we can observe an error on row 3.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3n_14.png)

<br>  
  
- After clicking the word “Error” within the Preview Window it will provide details about the specific issue.
       
<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3n_15.png)

<br>

To remove rows with errors in Power Query, first select the column that contains errors. On the Home tab, in the Reduce rows group, select Remove rows. From the drop-down menu, select Remove errors

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3n_16.png)

<br>

The result of that operation will give you the table that you're looking for.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3n_17.png)

<br>

### Replace errors

If instead of removing rows with errors, you want to replace the errors with a fixed value, you can do so as well. To replace rows that have errors, first select the column that contains errors. On the Transform tab, in the Any column group, select Replace values. From the drop-down menu, select Replace errors.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3n_18.png)

<br>

In the Replace errors dialog box, enter the value 10 because you want to replace all errors with the value 10.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3n_19.png)

<br>

The result of that operation will give you the table that you're looking for.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3n_20.png)

<br>

#### Create your own visualizations - 1

1. Open Retail Analysis Sample
2. In the Visualizations pane, select the paint roller icon to reveal the format options.
3. Select Title to expand that section.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3n_21.png)

<br>

4.Move the Title slider to On.
5.To change the title, enter Store count by month opened in the Title text field.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3n_22.png)

<br>

6.Change Font color to white and Background color to blue
a. Select the drop-down and choose a color from Theme colors, Recent colors, or Custom color.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3n_23.png)

<br>

b. Select the drop-down to close the color window.
7.Increase the text size to 16 pt.
8.The last customization you'll make to the chart title is to align it in the center of the visualization.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3n_24.png)

If you ever need to revert all of the changes, select Revert to default, at the bottom of the Title customization pane.

#### Create your own visualizations - 2

Let's practice how to create another visualization.  
**Note**: We will use the "financial_sample.xlsx" dataset.

- Download "financial_sample.xlsx" file
- Load it as a data source
- Select a clustered column chart visualization

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3_viz1.png)

<br>

When you click on the desired visualization, a template is created in the report workspace.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3_viz2.png)

<br>

- Now that we have selected a visualization

- We are going to visualize sales and profits on Y-axis and date on X-axis. ie drag and drop sales and Profit to values section and date to axis section.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3_viz3.png)

<br>

**Note**: Make sure that you have selected the correct aggregation measure for the plot. Here we need sum of sales and sum of Profit. You can edit the date on the X axis as well.

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3_viz4.png)

<br>

- Done :wink:
- Now is your turn to create another visualization.

</details>

<br>

<details>
<summary> Click for session details: Drill Down and Drill Up Feature</summary>
  
<br>

In Power BI, we can create data hierarchies to conduct deep dive analysis. We will see what that means by taking a look at a couple of examples. In these examples we will continue using the `financial_sample.xlsx` file.

### Using pre-defined hierarchies in Power BI.

In this case, we will create a simple "Column Chart"

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/drilldown1.png)

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/drilldown2.png)

<br>

Now drag and drop "Date" from fields pane in the Axis and "Sale" in the values sections

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/drilldown3.png)

<br>

As you can see, Power BI automatically creates a hierarchy in the Axis where "Date" is. To drill down on this hierarchy in the plot, click on the Drill Down button. This would activate the drill down feature.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/drilldown4.png)

<br>

Now you can click on any of the bars , either for 2013 and 2014 and that would take you to next data level. You can continue doing it to move deeper into data as you like.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/drilldown5.png)

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/drilldown6.png)

<br>

You can click other features such as "Drill Up", "Go to the next level in hierarchy", and "Expand all down one level in the hierarchy", to see how these options work

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/drilldown10.png)

<br>

### Creating your own hierarchies

Go to a new page in Power BI and select "Clustered Column Chart" from visualization pane

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/drilldown2.png)

<br>

First drag and drop "Country" column on the axis and then drag drop "Product" under it in the Axis. Use "Sales" in the values.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/drilldown7.png)

<br>

Activate hierarchies again by clicking on the drill down button. Then select any country you would like, you would see that you will now see the sales values of "Product" categories for that particular country.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/drilldown8.png)

<br>

Here we have selected Mexico.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/drilldown9.png)

<br>

You can click other features such as "Drill Up", "Go to the next level in hierarchy", and "Expand all down one level in the hierarchy", to see how these options work

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/drilldown10.png)

</details>

---

:coffee: **BREAK**

> 🕰️ 10 min

---

### :pencil2: Practice - Lab

> 🕰️ 120 min (To Finish the Lab) + 60 mins (To discuss)

<details>
  <summary> Click for Instructions: Lab </summary>

For maintenance purposes and to have a single source of truth, use this link to get to the lab instructions. This link will take you to the same content that is presented to students.

- [Lab | Data manipulation](https://github.com/haggarw3/Power-BI-V1/blob/main/02_lean_lessons/week_1/day_3/lab-7.06-data_manipulation.md)

</details>

<details>
  <summary> Click for Solution: Lab solutions </summary>

The solution is provided as an MP4 file, a link to the [recording can be found here](https://ironhack.zoom.us/rec/share/RfvUVNgBmqA6t6qbuVfp6PMtXaIF5jUlsUf0zK4vT32SMLYcKtuC-MeIq56z7Dzk.6VGOBI4tj2UxPLaR?startTime=1623417151000).

The solution file is also provided in the folder. Name of the file is [lab-data-manipulation-solution.pbix](https://github.com/haggarw3/Power-BI-V1/blob/main/01_lesson_plans/week_1/day_3/lab-data-manipulation-solution.pbix)

</details>

---

> End of the day
