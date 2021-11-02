# Lab | Dashboard Solution

<br>

## Challenge 1 - Create your first Dashboard

<br>

In this challenge, we will practice (once again) creating dashboards.

Let's start!

Use the `crime_2018.xlsx` file. You can find this file in the [Power BI resources](https://github.com/ironhack-edu/power-bi-resources) repository. It contains a list of all of the crimes reported in the area around our Manchester training room in 2018.

<br>

![](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/8.08-lab3.jpg)

<br>

Below is an overview of the steps:

1. Add a gauge to show the number of crimes with a target (invented!) of 4000 and a range from 0 to 5000.

   - Select gauge chart

   <br>

   ![](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/8.08-lab4.jpg)

   <br>

2. Switch to the formatting properties of the gauge to set an absolute minimum and maximum value.
3. Create Max Value (5000) and Target Value (4000) columns.

   ```
   max_value = 5000
   ```

   ```
   target_value = 4000
   ```

   <br>

   ![](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/8.08-lab5.jpg)

   <br>

   - Change Title Format and Color

4. Now add a KPI to show the number of crimes by month.

<br>

![](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/8.08-lab6.jpg)

<br>

- Select KPI chart
- Drag Crime ID (Count)
- Drag Date to Trend Axis
- Format Title

The figure shown is the number of crimes for the final month in the period - for this visual, there doesn't seem to be any obvious way of altering the number shown.

5. Next, add a column chart comparing crime figures by category and quarter.

<br>

![](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/8.08-lab7.jpg)

<br>

- Select Stacked Column Chart
- Drag Date and keep Quartes hierarchy on Axis
- Drag Category to Legend
- Drag Crime ID (values)
- Format Legend
- Format Title

6. Finally, add a map with the location of each crime.

<br>

![](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/8.08-lab8.jpg)

<br>

- Select map visualization
- Drag Latitude and Longitude to each pane
- Drag Crime ID as Count to Size
- Format Title

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
