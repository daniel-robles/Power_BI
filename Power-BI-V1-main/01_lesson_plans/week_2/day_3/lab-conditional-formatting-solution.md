# Lab | Conditional Formatting - Solution

<br>

## Challenge 1 - Apply conditional formatting

<br>

In this challenge, we will practice conditional formatting.
These guidances are helpful to train your problem-solving thinking and to learn how to work around problems.

Below is an overview of the steps:

- Using the `age_specific_genres.xlsx` file in the above folder create a matrix showing the Count of films by Certificate rating and Genre.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/8.06-lab1.jpg)

<br>

Your matrix will have all the certificates listed.

- First, you need to load Certificate, Genre, Fils as separate data sources.
- Create Joins between tables using CertificateID and GenreID fields (If doesn't apply automatically).
- Notice how the certificates are in alphabetical order? CertificateID is in a more sensible order; use this to reorder the Certificate column.

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/8.06-lab2.jpg)

<br>

You now have a more familiar order.

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/8.06-lab3.gif)

<br>

- To apply conditional formatting, select the Matrix visualization.
- In the Visualizations pane, right-click or select the down-arrow next to the field in the Values well that you want to format.
- Select Conditional formatting, and then select the type of formatting to apply.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/8.06-lab4.jpg)

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/8.06-lab6.jpg)

<br>

**NOTE**: To remove conditional formatting from a visualization, select Remove conditional formatting from the field's drop-down menu, and then select the type of formatting to remove.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/8.06-lab5.jpg)

<br>

## Challenge 2 - More and More Visualization

<br>

Start by creating the following chart, or as close to it as you can get.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/8.06-lab7.jpg)

<br>

Color saturation has been set to color charts according to Oscars Wins, and data labels applied outside each one.

- Drag Genre to Legend
- Drag Oscar Wins to Values
- Make sure that the Label position is selected as Outside
- Format Title as the example
- Change Data Colors

Now let's create the following chart where we want to display if the budget is proportional to the number of Oscar wins, in other words, when the budget was bigger the movie won more Oscars.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/8.06-lab8.jpg)

<br>

- Select Line and Stacked Column chart
- Drag Genre to Shared Axis
- Drag Budget Dollars to Column
- Drag OscarWins to Line Value
- Format Title as the example

<br>

Now you can answer which genre is the most awarded and if the budget was proportional to the number of wins.

When you finish the last 3 tables/visualizations you can filter all when you select any Genre on Pie Chart, for example.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/8.06-lab9.jpg)
