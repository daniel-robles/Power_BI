<!-- # Lab | Dashboard -->

## Introduction

A Power BI dashboard is a single page, often called a canvas, that uses visualizations to tell a story. Because it is limited to one page, a well-designed dashboard contains only the most important elements of that story.

<br>

![](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/8.08-lab1.png)

<br>

The visualizations you see on the dashboard are called **tiles** and are pinned to the dashboard by report designers. In most cases, selecting a tile takes you to the report page where the visualization was created.

The visualizations on a dashboard come from reports and each report is based on one dataset. In fact, one way to think of a dashboard is as an entryway into the underlying reports and datasets. Selecting a visualization takes you to the report that was used to create it.

<br>

![](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/8.08-lab2.png)

# Prerequisites

- At this point, you should have installed Power BI on your laptop
- Open the `crime_2018.xlsx` file
- Open `desktop_report.pbix` file

**Note**: You can find both of these files in the [Power BI resources](https://github.com/ironhack-edu/power-bi-resources) repository.

If you have any doubts about the prerequisites, please clarify with your instructor or teaching assistants.

<br>

## Challenge 1 - Create Dashboard (Desktop view)

<br>

In this challenge, we will practice (once again) creating dashboards.

Let's start!

Use the `crime_2018.xlsx` file. You can find this file in the [Power BI resources](https://github.com/ironhack-edu/power-bi-resources) repository. It contains a list of all of the crimes reported in the area around our Manchester training room in 2018.

<br>

![](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/8.08-lab3.jpg)

<br>

Below is an overview of the steps:

1. Add a gauge to show the number of crimes with a target (invented!) of 4000 and a range from 0 to 5000.
2. Switch to the formatting properties of the gauge to set an absolute minimum and maximum value.
3. Create Max Value (5000) and Target Value (4000) columns.

   - Change Title Format and Color

4. Now add a KPI to show the number of crimes by month.

<br>

![](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/8.08-lab6.jpg)

<br>

The figure shown is the number of crimes for the final month in the period - for this visual, there doesn't seem to be any obvious way of altering the number shown.

5. Next, add a column chart comparing crime figures by category and quarter.

<br>

![](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/8.08-lab7.jpg)

<br>

6. Finally, add a map with the location of each crime.

<br>

![](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/8.08-lab8.jpg)

<br>

## Challenge 2 - Power BI Mobile Visualization

<br>

The `desktop_report.pbix` file (in the Power BI resources repository) contains a report, originally designed only for desktop and sadly hasn't been optimized for mobile.

<br>

![](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/8.08-lab9.jpg)

<br>

1. To fix this problem, choose Phone Layout from the View tab.
   Keep in mind that this doesn't replace the desktop version; instead, it gives an alternative when needed.

2. Click on Top Pane on View Option

<br>

![](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/8.08-lab10.jpg)

<br>

3. Then click on Mobile Layout

<br>

![](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/8.08-lab11.jpg)

<br>

4. Rearrange the visuals to fit on the screen and consider which are needed.
5. Optionally save this as a Mobile report, and with this step, we are done with this lab.

<br><br>

## Additional Resources

<br>

- [View a Dashboard](https://docs.microsoft.com/en-us/power-bi/consumer/end-user-dashboard-open)
