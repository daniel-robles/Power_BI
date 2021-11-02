<!-- # Power BI Mini Project 2 -->

### Duration: 4 hours

<br>

## Learning Objectives

In the Power BI Mini project 2, students will practice the topics covered in the course during this and the previous week in relation to Power BI. Please read the instructions carefully. The set of deliverables for this mini-project are also provided.

<br>

## Instructions for Mini Project Part 1

<br>

### Data sources

<br>

We are going to use **`great_lakes.xlsx`** file. You can find this file in the [Power BI resources](https://github.com/ironhack-edu/power-bi-resources) repository.

<br>

### Your tasks

<br>

1. Find a Power Query transformation that will change the individual lake columns into rows.
   _Hint 1_: You should end up with only three columns loaded into your data model.)
   _Hint 2_: Use the "Unpivot Others" function to keep only 3 columns.

2. Create a matrix visual that displays ice coverage by a lake (on columns) and year (on rows).

3. Include major format options as seen in the sample, such as removing row and column totals.

4. Find the "lake" you need to filter out and add a page-level or report-level filter to exclude it.

5. Matrix conditional formatting:

- Background Color:
  - Build a set of conditional formatting Rules (not the default gradient Color Scale option).
  - Use five different colors for ice coverage consisting of 0-24.99, 25-49.99, 50-74.99, 75-99.99, and 100
- Font Color:
  - Only use black (`#000000`) or white (`#FFFFFF`) font colors.
  - Build and apply Rules so that the contrast between your background colors and white or black font color.

8. Add a star next to any value where the maximum ice coverage is 100%.

9. Add at least two supporting visuals around your matrix. You only have three fields, so be creative!

<br>

### Deliverables - part 1

<br>

- Final Power BI file named as `Lake_Analysis`
- Answer the following questions:
  - Which lake has frozen completely over most often?
  - Is ice coverage trending _upward_ overtime for any lake?

<br>
<br>

## Instructions for Mini Project Part 2

<br>

### Data sources

<br>

We are going to use **`mini_project2_sample_data.pbix`** file. You can find this file in the [Power BI resources](https://github.com/ironhack-edu/power-bi-resources) repository.

<br>

<!-- If you are not able to access the file on GitHub, please use the link below to access it on Google Drive
[https://drive.google.com/file/d/1wXYF5g9EtkCNfLLApNIvnpR5lCL8BFLM/view?usp=sharing] -->

Here you will find information on the sales of certain products made by some manufacturers across North America (US, Mexico, and Canada) and in Europe (France and Germany).
A sales table is a calculated table that consists of other calculated columns from other tables in the dataset. You can go through the formulas in the table to check DAX formulas for them.

### Objective

Your objective will be to re-create a report as shown below. You can either rewrite DAX formulas yourself or you can use the existing calculations provided in the model. To check the relationship between tables, you can click on the "Model" tab. Here is a screenshot of the relationship diagram between the tables.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/mini_project/relationship_diagram.png)

<br>

### Your tasks

<br>

1. Create a Sales Report and a Trend Report. The reports that you have to recreate are shown below.

<br>

#### Sales Report

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/mini_project/sales_report.png)

<br>

<details style="font-size: 14px; cursor: pointer; outline: none;">
  <summary> Click here for Details on the plots in Sales Report  </summary>

<br>

1. Date slicer

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/mini_project/sales_report.png)

<br>

2. Stacked bar chart of Total Sales by Category and Segment

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/mini_project/sales_by_category_segment.png)

<br>

3. Treemap of Total Sales by Manufacturers

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/mini_project/treemap_sales_by_manufacturers.png)

<br>

4. Scatter plot - Total sales vs total units by Segment

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/mini_project/scatter_sales_by_segment.png)

<br>

5. Map of total sales by country

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/mini_project/map_by_country.png)

</details>

<br><br><br>

#### Trend Report

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/mini_project/trend_report.png)

<br>

<details style="font-size: 14px; cursor: pointer; outline: none;">
  <summary> Click here for Details on the plots in Trends Report  </summary>

<br>

1.Slicers based on Category, Segment, and Country

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/mini_project/trend_slicer.png)

<br>

2.  Total sales and total units by year

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/mini_project/mp_1.png)

<br>

3. Change in sales by year (sales variation)

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/mini_project/mp_2.png)

<br>

4. Total sales and total units by year - for van Arsdel

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/mini_project/mp_3.png)

<br>

5. Change in sales by year (sales variation) - for van Arsdel

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/mini_project/mp_4.png)

</details>
