# Mini Project 2 - Part 1 Solution

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

### Solutions

<br>

- Load the `great_lakes.xlsx`, open the `lakes_info` tab:

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/mini_project/solution_mini_project_1.jpg)

<br>

- Click on Transform Data Button
- We have the following columns: `Year`, `Superior`, `Michigan`, `Huron`, `Erie`, `Ontario`, `All Lakes`) but we have to _Unpivot_ this table
  - Select the `Year` column, right click and then click on _Unpivot Other Columns_,

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/mini_project/solution_mini_project_2.jpg)

<br>

- Now we have only three columns (`Year`, `Attribute` and `Value`),
  - Rename columns as Lake (Attribute), Coverage (Value)

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/mini_project/solution_mini_project_3.jpg)

<br>

**Note**: Make sure that the column `Year` is a whole number (integer).

Now, on canvas:

- Select Matrix visualization.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/mini_project/solution_mini_project_4.jpg)

<br>

- Drag Coverage to Values
- Drag Lake to Columns
- Drag Year to Rows

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/mini_project/solution_mini_project_5.jpg)

<br>

- Order values as Desc Year
- Delete Rows and Columns subtotals
- Change Text Size to 12pt
- Right click on Coverage. Select Conditional Formatting, Background color

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/mini_project/solution_mini_project_6.jpg)

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/mini_project/solution_mini_project_7.jpg)

<br>

- Format by rule option, following the next groups `0-24.99`, `25-49.99`, `50-74.99`, `75-99.99`, and `100`,
- Select the background color from the lighter to darker for this groups,

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/mini_project/solution_mini_project_8.jpg)

<br>

- Right click on Coverage. Select Conditional Formatting, Font Color
- Format by rule option, when Coverage is lower to 75 select black and when coverage is over 75 select white color

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/mini_project/solution_mini_project_9.jpg)

<br>

- Right click on Coverage. Select Conditional Formatting, Icons
- Format by rule option, when Coverage is 100 then select Star Icon

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/mini_project/solution_mini_project_10.jpg)

<br>

- For this point the student will be free to create their own visualizations (at least 2) or recreate this example.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/mini_project/solution_mini_project_11.jpg)

<br>

If the path is recreated first we will create the slice filter:

- Select Slicer at Visualizations Pane
- Drag Year, DONE!
- Then, select a Line Chart.
- Drag Year to Axis
- Drag Coverage to Values
- Now, click on Analytics and Select Trend Line

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/mini_project/solution_mini_project_12.jpg)

<br>

- Finally, Select a Stacked column chart
- Drag Lake to Axis
- Drag Values to Coverage
- Change calculation (Coverage) to Max
- Click on Format and activate Data labels
- DONE!

<br>

The main point of this is practice and let the students bring all their knowledge to create a simple dashboard.
