<!-- # Lab | DAX Functions -->

## Introduction

It’s easy to create a new Power BI Desktop file and import some data into it. You can even create reports that show valuable insights without using any DAX formulas at all. But, what if you need to analyze growth percentage across product categories and for different date ranges? Or, you need to calculate year-over-year growth compared to market trends?

DAX formulas provide this capability and many other important capabilities as well. Learning how to create effective DAX formulas will help you get the most out of your data. When you get the information you need, you can begin to solve real business problems that affect your bottom line. This is the power of Power BI, and DAX will help you get there.

# Prerequisites

- At this point you should have installed Power BI on your laptop
- Open `tallest_buildings.pbix` which you can find in the [Power BI resources](https://github.com/ironhack-edu/power-bi-resources/tree/master/tallest_buildings_all_resources) repository

If you have any doubts about the prerequisites, please clarify with your instructor or teaching assistants.

<br>

## Challenge 1 - Create Calculated Columns with DAX

<br>

In this challenge, we will practice creating calculated columns, dividing one column by another, and avoiding any divide-by-zero errors.

These guidances are helpful to train your problem-solving thinking and to learn how to work around problems.

Below is an overview of the steps:

Open the Power BI file in the above folder. You should see that it contains a list of the 61 tallest buildings in the world.

Create a calculated column in the `Buildings` table to show the average height of each floor for each building (divide the Metres column by the Floors column).

- If you add this column to your table and sort by it, you'll see Giant Owl Towers appear at the top.
- The problem is that this building has zero floors. Amend your formula so that it shows a blank for the average floor height for buildings with no floors.
- Much better - if you sort the buildings by ascending order by average floor height, Giant Owl Towers appears at the top of the list.

There are at least 3 ways to do this, using either `DIVIDE`, `ISERROR` or `IF`.

<br>

## Challenge 2 - More Calculated Columns with DAX

<br>

- Create a calculated column to show the average height from the whole table.
- Create a calculated column that shows min-height from the whole table.
- Create a calculated column that shows max height from the whole table.
- Create a calculated column that shows the number of rows.
- Create a visualization with the recently created table.
- Compare the MIN, MAX, and AVERAGE heights.

<br>

## External Resources

<br>

- [`ISERROR` Function](https://docs.microsoft.com/en-us/dax/iserror-function-dax)
