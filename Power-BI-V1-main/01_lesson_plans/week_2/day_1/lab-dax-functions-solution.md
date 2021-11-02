# Lab | DAX Functions Solution

<br>

## Challenge 1 - Create Calculated Columns with DAX

In this challenge, we will practice creating calculated columns, dividing one column by another, and avoiding any divide-by-zero errors.

These guidances are helpful to train your problem-solving thinking and to learn how to work around problems.

Below is an overview of the steps:

Open the Power BI file in the above folder. You should see that it contains a list of the 61 tallest buildings in the world.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/8.02-lab1.gif)

<br>

Create a calculated column in the `Buildings` table to show the average height of each floor for each building (divide the Metres column by the Floors column).

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/8.02-lab4.gif)

<br>

```
Average Floor Height = Buildings[Metres] / Buildings[Floors]
```

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/8.02-lab2.gif)

- If you add this column to your table and sort by it, you'll see Giant Owl Towers appear at the top.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/8.02-lab3.gif)

<br>

- The problem is that this building has zero floors. Amend your formula so that it shows a blank for the average floor height for buildings with no floors.

- Much better - if you sort the buildings by ascending order by average floor height, Giant Owl Towers appears at the top of the list.

There are at least 3 ways to do this, using either `DIVIDE`, `ISERROR` or `IF`.

<br>

#### Using `IF`

<br>

```
IF_FUNCTION = IF(  Buildings[Floors]  = 0 , 0 , Buildings[Metres] / Buildings[Floors])
```

<br>

#### Using `ISERROR`

<br>

```
ISERROR_FUNCTION = IF( ISERROR( Buildings[Metres] / Buildings[Floors] ) , BLANK(), Buildings[Metres] / Buildings[Floors])
```

<br>

#### Using `DIVIDE`

<br>

```
DIVIDE_FUNCTION = DIVIDE( Buildings[Metres] , Buildings[Floors] )
```

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/8.02-lab5.gif)

<br>

## Challenge 2 - More Calculated Columns with DAX

- Create a calculated column to show the average height from the whole table.

```
AVERAGE_function = AVERAGE (Buildings[Metres])
```

- Create a calculated column that shows min-height from the whole table.

```
MIN_function = MIN (Buildings[Metres])
```

- Create a calculated column that shows max height from the whole table.

```
MAX_function = MAX (Buildings[Metres])
```

- Create a calculated column that shows the number of rows.

```
COUNT_function = COUNT(Buildings[Built])
```

- Create a visualization with the recently created table.

- Compare the MIN, MAX, and AVERAGE heights.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-2/8.02-lab8.jpg)
