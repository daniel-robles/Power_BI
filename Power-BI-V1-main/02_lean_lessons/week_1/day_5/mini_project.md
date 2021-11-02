<!-- # Mini Project -->

### Duration: 4 hours

<br>

## Learning Objectives

<br>

Now that we have come to the end of the week, it is time to practice everything that we’ve already learned and add something that will complement already gained knowledge!

Keep in mind that if you do not know how to do something, your first circle of help should be Google. Always ask Google, as it has a huge database and for sure someone experienced the same problem you are facing now.

The mission here will be to **create a report** where you can combine several types of graphics which will use calculated fields.

_We have not discussed reports in class this week. We will discuss it in more detail next week. Just to give you a quick idea - the report is nothing but a group of visualizations put together to bring some insights from the data, and to tell the user a story._

We will do some data transformations and then use the data to build some visualizations to bring some insights from the data.

<br>

### Data sources

<br>

We are going to use **`financial_sample.xlsx`** file. You have been using this file during this week, but if you have to download it again refer to the [Power BI resources](https://github.com/ironhack-edu/power-bi-resources) repository.

<br>

## Instructions - Calculations part

1. Check the data types of all the columns and correct them if they are not in the correct format.

2. Fix the errors in the columns "discounts" and "profit". You might encounter these errors when converting the data type from the current one to the correct types.

3. Verify the profits in the data by using a simple calculation: `profit = units sold * sale price - (discount + COGS)`. _COGS_ is the cost of goods sold. Create another column _`profit_calc`_.

4. Create another column _`profit_verify`_ that checks if the values in the columns `profit_calc` and `profit` match. This should result in a boolean output. Check how many rows do not match. Find the reason why values in the two columns are not matching. Can you reduce the number of un-matches there?

5. In the country column, replace the values "United States of America" with "US".

6. Create another column called _`year`_ that will store the year values from the column _`date`_.

7. Create another column called _`month`_ that will store the month values from the column _`date`_. Instead of having the months as numbers, can you have them as January, February, etc?

8. Hide the column _`date`_. Can you delete the column _`date`_, if you do not wish to see the column in your dataset?

9. We will create two measures in our dataset. We will give you the formulas on how to create them. Click on "New Measures" and use the following formula to create a measure. We will talk more about Measures in the next week when we will cover DAX (Data Analysis eXpressions).

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/mini_project/new_measures.png)

<br>

```
profit_2013 =
  VAR
    CurrentDate = "01/01/2015"
  RETURN
    CALCULATE(
     SUM(financials[Profit]),
     financials[Year] = YEAR(CurrentDate)-2
    )
```

<br>

```
profit_2014 =
  VAR
    CurrentDate = "01/01/2015"
  RETURN
    CALCULATE(
     SUM(financials[Profit]),
     financials[Year] = YEAR(CurrentDate)-1
    )
```

10. Now create a measure to calculate the Year on Year percentage change in profit:

```
YoY = DIVIDE([profit_2014],[profit_2013],0)-1
```

<br>

_Hint_: Remember that we want to see the percentage of growth _YoY_, not the difference between the two years.

Perfect! Now we have the calculations for our visualizations!

<br>

## Instructions - Visualization part

So, this is what we are going to do:

1. **Create a KPI visualization**.

   This visualization is intended to see how much are we growing YoY, MoM, DoD, ...

2. Create a **Gauge visualization**.

   With this one, we can see the completion rate of a specific goal. For this example, we are going to see the gross sales completion rate. Our _max_ value for this indicator will be 120000000 and our goal 90000000.

3. **Create a map**.

   The map is useful to work with geographic data and numerical values. For this one, we want to see (still using the _financials_ table) the total population per country and the size of the dot must be calculated by this field. We will use another dataset to get the population numbers. Load the `population.xlsx` file in Power BI (also can be found in the [Power BI resources](https://github.com/ironhack-edu/power-bi-resources) repository). Before you use the table, do the following simple transformation:

   - Rename the table `Population` if it is loaded with a different name.
   - Replace values in the column `location` from "United States of America" to the US.
   - Replace US (and dependencies) to the US.

   Now, create a map with location from the "Financials" table and population numbers from the "Population" table. Add filter for the year 2014 from the population table.

4. **Create a table**.

   We have worked with this before and remember that this is important or useful to show raw numbers and data easily. We want to see in the _financials_ the Gross Sales, Profit, YoY Percent Change, Sales 2 years ago and sales last year, all of that per country. You should format all amounts to be *int*s and the ones that are currency to have the `$` symbol.

5. Add two slicers:

   - One for the Country in Financial
   - Another for the Year
   - Be sure that you can filter from here to all graphics.

   Now you've finished all the great stuff and calculations, here comes "the cherry on top of the cake". You must create visualizations that engage your audience and go all the way to do it. You will practice the usage of Images and Themes in PowerBI.

   - Add a Title for the dashboard.
   - Add an image/logo of your preference.
   - Apply a Theme to your whole dashboard. It will change all font colors and designs to one predefined.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/mini_project/insert_image.png)

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/mini_project/themes.png)

<br>

## Deliverables

<br>

Remember that you're free to create and order your report as you want. Finally, save it and export it as a PDF. This is an easy way to share your report with people within your team that don’t have PowerBI or with anyone outside of your company.

Be sure that all graphics are visible and no information is missing from your calculations (separate it in two PDFs, one for each year), and be careful with visualizations' size and order.

<br>

## Additional Tips and Hints

- _Be concise_: Try to make your visualizations as simple as possible. Remember that "less is more", don't try to saturate the dashboard with too many visualizations.
- _Read and understand your data_: The more you understand it, the most you'll get out of it.
- _Ask for a hint/help_: If you think you don't have any idea on how to do any bullet in the challenge, ask for help or Google it.

<br><br>

## Additional Resources

<br>

- [KPI Visualization](https://docs.microsoft.com/en-us/power-bi/visuals/power-bi-visualization-kpi)
- [Data Analysis](https://managementhelp.org/businessresearch/analysis.htm)
- [Arcgis PowerBI](https://doc.arcgis.com/en/power-bi/get-started/about-maps-for-power-bi.htm)
