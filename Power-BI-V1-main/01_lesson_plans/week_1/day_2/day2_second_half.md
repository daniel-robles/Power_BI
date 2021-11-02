# Lesson 7.4 - Creating Visualizations

<br><br>

### Lesson Duration: 4 hours (including Lab)

<br>

**Purpose**: After a brief introduction to Power BI, its different functionalities, offerings in the BI space, its features, and then getting comfortable with the GUI, we will now conduct hands-on for creating some first simple visualizations.

<br>

## Pre-requisites

To successfully take this class, the students would need:

- Power BI desktop
- Lesson 7.3 completed
- Access to all datasets used in class and lab (students have access to this [repository](https://github.com/ironhack-edu/power-bi-resources) - liked to their Student Portal)

---

## Learning Objectives

After this lesson, students will be able to:

- Create visualizations
- Understand the main properties of the visualization

<br><br>

### Session 1

> 🕰️ 40 min

#### Key Concepts

- Create a simple visualization
  - Get data
  - Transform and shape data
  - Build a visualization

:exclamation: Note for instructor: This is a simple example where the students will get comfortable using the interface more. The idea is to create a very simple plot. It doesn't have to be the most visually appealing plots.

<br>

<details>
<summary> Click for session detail </summary>

On the Power BI Desktop Home tab, select Get Data > Web to connect to a web data source.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day2_18.png)

<br>

In the From the Web dialog box, paste the address `https://www.bankrate.com/retirement/best-and-worst-states-for-retirement/` into the URL field, and select OK.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day2_19.png)

<br>

At this point, you can select Load to load the table, or Transform data to make changes in the table before you load it.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day2_20.png)

<br>

When you select Transform data, Power Query Editor launches, with a representative view of the table. The Query Settings pane is on the right, or you can always show it by selecting Query Settings on the View tab of Power Query Editor.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day2_21.png)

<br>

Notice that the Applied Steps in Query Settings already contain a few steps. You can select each step to see its effect in the Power Query Editor. - First, you specified a web source - Then you previewed the table in the Navigator window - In the third step, Changed type, Power BI recognized whole number data when importing it, and automatically changed the original web Text data type to Whole numbers.
As you would see from the data, the headers of the data do not look well. We need the header names as "State", "Overall Rank", "Affordability", "Crime", "Culture",...
But this is currently being read as another row in the table. So we will perform a couple of simple data transformations to read the data properly for analysis. 1. We will set the top row as header first 2. Then we will remove the first row. Refer to the screenshots below for reference.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day2_transform2.png)

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day2_transform3.png)

<br>

After you make the changes, click on "Close and Apply" on the left corner of the screen.
Also, note that the transformation steps are on the right-hand side.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day2_transform5.png)

<br>

This is what the data will look like now.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day2_transform4.png)

<br>

To create a simple visualization, just select any field in the fields list, or drag the field from the Fields list onto the canvas.
For example, drag the State field from "Ranking of Best and Worst States for Retirement" onto the canvas, and see what happens.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day2_14.png)

<br>

Power BI Desktop recognized that the State field contained geolocation data and automatically created a map-based visualization. The visualization shows data points for the 40 states from your data model.

The Visualizations pane shows information about the visualization and lets you modify it.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day2_15.png)

<br>

The icons show the type of visualization created. You can change the type of a selected visualization by selecting a different icon, or create a new visualization by selecting an icon with no existing visualization selected.
The Fields option in the Visualization pane lets you drag data fields to Legend and other field wells in the pane.
The Format option lets you apply formatting and other controls to visualizations.
The options available in the Fields and Format areas depend on the type of visualization and data you have.
Drag the Weather field from the Fields pane into the By value field, and then select Apply filter.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day2_23.png)

<br>

You now see only the top 10 weather states in the map visualization.

Retitle your visualization by selecting the Format icon in the Visualization pane, selecting Title, and typing Top 10 weather states under the Title text.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day2_24.png)

<br>

To add a visualization that shows the names of the top 10 weather states and their ranks from 1 to 10, select a blank area of the canvas and then select the Column chart icon from the Visualization pane. In the Fields pane, select State and Weather. A column chart shows the 40 states in your query, ranked from highest to lowest numerical rank, or worst to best weather.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day2_25.png)

<br>

To switch the order of the ranking so that number 1 appears first, select the More options ellipsis at the upper right of the visualization, and select Sort ascending from the menu.

:exclamation: Note to the instructor: Please note that there is no activity followed by this session. The students can straight jump to the lab

</details>

---

:coffee: **BREAK**

> 🕰️ 10 min

---

### :pencil2: Practice - Lab

> 🕰️ 120 min (to finish the Lab) + 60 mins (to discuss)

<details>
<summary> Click for Instructions: Lab </summary>

For maintenance purposes and to have a single source of truth, use this link to get to the lab instructions. This link will take you to the same content that is presented to students.

- [Lab | Database connection](https://github.com/haggarw3/Power-BI-V1/blob/main/02_lean_lessons/week_1/day_2/lab-7.04-database_connections.md)

</details>

<details>
  <summary>Click for Solution: Lab solutions</summary>

The solution is provided as an MP4 file, a link to the [recording can be found here](https://ironhack.zoom.us/rec/share/RfvUVNgBmqA6t6qbuVfp6PMtXaIF5jUlsUf0zK4vT32SMLYcKtuC-MeIq56z7Dzk.6VGOBI4tj2UxPLaR?startTime=1623415797000).

</details>

---

> End of the day
