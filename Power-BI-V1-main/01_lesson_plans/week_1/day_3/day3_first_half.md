# Lesson 7.5 - Manipulating Data with Power BI

<br><br>

### Lesson Duration: 4 hours

<br>

**Purpose**: The purpose of this lesson is to identify the various data types available in Power BI and to learn their properties. The students will also develop knowledge about basic data profiling and manipulate data using PBI.

<br>

## Pre-requisites

To successfully take this class, the students would need:

- Completed all previous lessons
- Power BI desktop
- Access to all datasets used in class and lab (students have access to this [repository](https://github.com/ironhack-edu/power-bi-resources) - liked to their Student Portal)

---

## Learning Objectives

After this lesson, students will be able to:

- Identify the types and properties of data in PBI
- Examine data structures
- Identify data anomalies
- Manipulate data using PBI

<br><br>

### Session 1

> 🕰️ 40 min

#### Key Concepts

- Data types in PBI

  - Number
  - Date /time
  - Text
  - True false
  - Blanks / nulls
  - Binary Data
  - Table data

- Properties of different data types
- Understanding the data types in the dataset
- Fixing data types (transform column data types)

> :exclamation: Note to the instructor: In this lesson, we will use the "financial_sample.xlsx" file. Explain the data types by looking at the columns in the "financials" table.

<details>
<summary> Click for Session Detail: Data Types in Power BI</summary>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3_1.png)

<br>

- **Number type**

  - _Decimal numbers_: Represents a 64 bit (eight-byte) floating-point number. It’s the most common number type and corresponds to numbers as you usually think of them. The Decimal Number type can handle negative values from -1.79E +308 through -2.23E -308, 0, and positive values from 2.23E -308 through 1.79E + 308. for example, 34, 34.01, and 34.000367063 are all valid decimal numbers.The decimal number type corresponds to how Excel stores its numbers.
  - _Fixed decimal number_: Has a fixed location for the decimal separator. The decimal separator always has four digits to its right and allows for 19 digits of significance. The largest value it can represent is 922,337,203,685,477.5807 (positive or negative). The fixed decimal number type is useful in cases where rounding might introduce errors. Since the values that pass the four digits to the right of the decimal separator are truncated, the fixed decimal type can help you avoid these kinds of errors. If you’re familiar with SQL Server, this data type corresponds to SQL Server’s Decimal (19,4), or the Currency Data type in Power Pivot.
  - _Whole number_: Represents a 64 bit (eight-byte) integer value. Because it’s an integer, it has no digits to the right of the decimal place. It allows for 19 digits; positive or negative whole numbers between -9,223,372,036,854,775,807 (-2^63+1) and 9,223,372,036,854,775,806 (2^63-2). It can represent the largest possible precision of the various numeric data types. As with the fixed decimal type, the whole number type can be useful in cases where you need to control rounding.

- **Date/time type**: Power BI Desktop supports five Date/Time data types in Query View. Both Date/Time/Timezone and Duration are converted during load into the model. The Power BI Desktop data model only supports date/time, but they can be formatted as dates or times independently.

  - _Date time_: Represents both a date and time value. Underneath the covers, the Date/Time value is stored as a decimal number type. So you can actually convert between the two. The time portion of a date is stored as a fraction to whole multiples of 1/300 seconds (3.33 ms). All dates between the years 1900 and 9999 are supported.
  - _Date_: Represents just a Date (no time portion). When converted into the model, a Date is the same as a Date/Time value with zero for the fractional value.
  - _Time_: Represents just Time (no Date portion). When converted into the model, a Time value is the same as a Date/Time value with no digits to the left of the decimal place.
  - _Date/Time/Timezone_: Represents a UTC Date/Time with a timezone offset. It’s converted into Date/Time when loaded into the model. The Power BI model doesn't adjust the timezone based on a user's location or locale etc. If a value of 09:00 is loaded into the model in the USA, it will display as 09:00 wherever the report is opened or viewed.

- **Text type**

  - _Text_: A Unicode character data string. Can be strings, numbers, or dates represented in a text format. Maximum string length is 268,435,456 Unicode characters (256 mega characters) or 536,870,912 bytes.

- Boolean (`true`/`false`) type: A boolean data type can have only 2 values: either a `true` or a `false`.

- _Table data type_: DAX uses a table data type in many functions, such as aggregations and time intelligence calculations. Some functions require a reference to a table; other functions return a table that can then be used as input to other functions. In some functions that require a table as input, you can specify an expression that evaluates to a table; for some functions, a reference to a base table is required.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3_2.png)

<br>

The Data Type drop-down in Power Query Editor has two data types not currently present in Data or Report View: Date/Time/Timezone and Duration. When a column with these data types is loaded into the model and viewed in Data or Report view, a column with a Date/Time/Timezone data type will be converted into a Date/Time, and a column with a Duration data type is converted into a Decimal Number.

</details>

<br>
    
<details>
<summary> Click for Session Detail: Basic data profiling </summary> 
    
> :exclamation: We will continue using the "financial_sample.xlsx" file. 
    
The data profiling tools provide new and intuitive ways to clean, transform, and understand data in Power Query Editor. They include:

- Column quality
- Column distribution
- Column profile

<br>

Open the Power Query Editor by clicking on the "Transform Data" button.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/power_query_editor.png)

<br>

To enable the data profiling tools, go to the View tab on the ribbon. Enable the options you want in the Data preview group, as shown in the following image.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3_7.png)

<br>

After you enable the options, you'll see something like the following image in Power Query Editor.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3_8.png)

<br>

You can select different columns by clicking on them and then see the **Column Statistics** and **Value Distribution**:

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3_8_1.png)

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3_8_2.png)

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3_8_3.png)

<br>

### Column quality

The column quality feature labels values in rows in three categories:

- `Valid`, shown in green
- `Error`, shown in red
- `Empty`, shown in dark grey

These indicators are displayed directly underneath the name of the column as part of a small bar chart, as shown in the following image.

The number of records in each column quality category is also displayed as a percentage.

By hovering over any of the columns, you are presented with the numerical distribution of the quality of values throughout the column. Additionally, selecting the ellipsis button (...) opens some quick action buttons for operations on the values.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3_10.png)

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3_10_a.png)

<br>

To move across different columns in the view, use the "Go To Columns" option and select any column for which you want to see the distribution of data.

> :exclamation: Note to the instructor: At this stage, the instructor may talk about what is meant by data distribution.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3_10_b.png)

<br>

</details>

<br>

#### :pencil2: Check for Understanding - Class activity

> 🕰️ 10 min (+ 10 min Review)

<details>
  <summary> Click for Instructions: Activity 1 </summary>

In the lesson, we spoke about some of the data types that are there in Power BI. We did not speak about Binary type though. Do the research and respond to the following questions (and learn much more):

- What is a binary type?
- What could be some possible use cases for it?

</details>

<br>

<details>
  <summary>Click for Solution: Activity 1 solutions</summary>

- The Binary data type can be used to represent any other data with a binary format, for example, images.
- The Binary data type is currently not supported outside of the Power Query Editor. Inside the Power Query Editor, you can also use it when loading binary files if you convert it to other data types before loading it to the Power BI model. Binary columns aren't supported in the Power BI data model. It exists in the Data View and Report View menus for legacy reasons but if you try to load binary columns to the Power BI model you may run into errors.
- Use Case: Suppose you import data from a SQL database, and it contains the binary representation of an image. Then you can use that data and display an actual image in a report.
- Also sometimes when you read data from any other file or database, it may contain data in the binary format. (This happens often with tables in SQL databases when the column with the primary key is read in binary format automatically). It can then be converted into some other format as applicable in that particular case.

</details>

---

:coffee: **BREAK**

> 🕰️ 10 min

---

### Session 2

> 🕰️ 40 min

#### Key Concepts

Descriptive Statistics

- What is mean, median, mode, and standard deviation
- Interrogate column statistics

<details>
<summary> Click Session Detail: Descriptive Statistics </summary>

Mean, median, and mode are three kinds of "averages". There are many "averages" in statistics, but these are the three most common and are certainly the three you are most likely to encounter.

### Mean

The "mean" is the "average" you're used to, where you add up all the numbers and then divide by the number of numbers.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3_3.png)

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3_4.png)

### Median

The "median" is the "middle" value in the list of numbers. To find the median, your numbers have to be listed in numerical order from smallest to largest, so you may have to rewrite your list before you can find the median.

:exclamation: When there are even numbers in the list, then the median is the average of the two central numbers.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/median_formula.jpg)

<br>

### Mode

The "mode" is the value that occurs most often. If no number in the list is repeated, then there is no mode for the list.

The "Standard Deviation" is a measure of how spread out numbers are.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3_6.PNG)

</details>
    
    
<details>
<summary> Click Session Detail:Explore statistical Properties</summary>

Data is often intertwined with statistics because statistics are one way in which you can explore your data. Statistics show you the distribution of your data and help you to identify key takeaways and trends and determine whether outliers exist.

The statistical summary is the information that provides a quick and simple description of your data. Power BI has many functions that help you to conduct statistical analysis, such as Data Analysis Expressions (DAX) functions, visuals such as histograms and bell curves, advanced analytics visuals, and statistical programming languages such as Python and R.

Power BI Desktop has a number of DAX functions that you can use to get quick statistics based on your data. You can access these quick functions by right-clicking the Values field in the Visualizations pane, as illustrated in the following image.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3_13.png)

</details>

#### :pencil2: Check for Understanding - Class activity

> 🕰️ 10 min (+ 10 min Review)

<details>
  <summary> Click for Instructions: Activity 2 </summary>

Take a look at this dataset:
`84, 87, 67, 99, 87, 76, 93, 84, 87, 99, 84`.

<br>

1. Can data have more than one _mode_? We see in the previous dataset that both, 87 and 84, are represented three times each. What would be the mode in this case?
2. Find the mean and median in the above case as well.
3. How would the mean and median change if the dataset was `84, 87, 67, 99, 87, 76, 93, 84, 87, 99, 84, 10`?
   - Do you see any change in the values of mean and median?
   - Can you see the effect of _outliers_ in the data?

</details>

<details>
  <summary>Click for Solution: Activity 2 solutions</summary>

For this list: `84, 87, 67, 99, 87, 76, 93, 84, 87, 99, 84`:

- Mode would be both 84 and 87
- Mean is 86.0909
- Median is 87

For this list: `84, 87, 67, 99, 87, 76, 93, 84, 87, 99, 84, 5`:

- Mode would be both 84 and 87
- Mean is 79.33
- Median is 85.5

**Conclusion**: Outliers have a more significant effect on mean as compared to medians.

</details>

---

:coffee: **BREAK**

> 🕰️ 10 min

---

### Session 3

> 🕰️ 40 min

#### Key Concepts

- Data Manipulation
- Hiding columns
- Sorting data
- Applying filters
- Using slicers
- Concatenate

<details>
<summary> Click for Session Detail: Simple manipulation using power BI: Removing Rows and Columns </summary>

:exclamation: We will work inside the query editor:

<br>

### Remove columns

Select the column, go to the Home tab and click on "Remove columns" to remove the column that you selected. Or you can also choose "Remove Other Columns" to remove the columns other than what you selected.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/remove_columns.png)

<br>

OR select the column or row that you want to remove, next right-click on it and select the "remove" option from the context menu.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/remove_columns_2.png)

<br>

:exclamation: Note that you can undo the changes by clicking on the close option in the Applied Steps section.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/remove_columns_1.png)

<br>
<br>

### Remove rows

Select the Home tab, click on the "Remove Rows" drop-down menu. Click on "Remove Rows" again and you will get 6 options. Click on "Remove Top Row" and enter the number of rows that you want to remove from the top and click on "Ok".

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/remove_rows_a.png)

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/remove_rows_b.png)

<br>

_Remove from the bottom_: Select the Home tab, click on the "Reduce Rows" drop-down menu. Click on "Reduce Rows" again and you will get 6 options, click on "Remove Bottom Rows". Enter the number of rows that you want to remove from the bottom. Click on "Ok" and your last two lines will be removed.

<br>

_Remove Alternate Row_: This is required when you want to remove the row from the middle. Once you click on this you will get three fields to be filled:

- First row to remove: Enter the row number(index or position) that you want to remove or you want to skip from.
- Number of rows to remove: Enter the number of rows you want to remove each time.
- Number of rows to keep: Enter the number of rows you want to keep.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/keep_rows.png)

</details>

<details>
<summary> Click for Session Detail: More data manipulation using power BI</summary>

### Hiding columns

1. Get data
2. Open the power query window by click on "transform data"
3. Select the table in the tab column

Click right Hide in report view:

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/hide_columns.png)

<br>

### Filters

You can apply filters in the Filters pane, or make selections in slicers directly on the report page itself. The Filters pane shows the fields in individual visuals, and any other filters the report designer adds.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/Day3_24.png)

<br>

There are four standard types of filters that you create in the Filters pane.

- _Visual filter_ applies to a single visual on a report page. You see visual level filters when you select a visual on the report canvas. Even if you can't edit a report, you can select a visual and filter it.
- _Page filter_ applies to all the visuals on the report page.
- _Report filter_ applies to all pages in the report.
- _Drillthrough filter_ is used to create a destination report page that focuses on a specific entity, such as a supplier. From the other report pages, users can right-click a data point for that entity and drill through to the focused page.

<br>

#### Basic and advanced filtering

<br>

By default, report readers can switch from Basic to Advanced filtering.

- Basic filters show a list of all the values in the field. You can search in the page, visual, and report filters, in the Reading or Editing view, to find and select the value you want.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/Day3_25.png)

<br>

A filter with the word All next to it is unfiltered, showing all the values in the field.

- Advanced filters: You could search for values that contain or don't contain, start with, or don't start with, a specific value.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/Day3_26.png)

<br>

#### Filters in reading or editing view (Power BI service or Power BI desktop)

- **Reading view**: You can interact with any filters that already exist in the report, and save the selections you make. You can't add new filters.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/Day3_27.png)

<br>

Each visual has filters for all the fields in the visual. When you create a report, you can add more. In this Filters pane, the visual has three filters.

In Reading view, you explore the data by modifying the existing filters. You're only filtering your view of the report. When you exit the report, the changes you make are saved with your view of the report, even if you open the report in a mobile app. To undo your filtering and return to the defaults set by the report author, select Reset to default from the top menu bar.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/Day3_28.png)

<br>

- **Editing view**: You can add all kinds of filters. When you save the report, the filters are saved with the report, even if report readers open it in a mobile app. People looking at the report in Reading view interact with the filters you added, but can't add new filters.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3_29.png)

<br>

#### Cross-filter and cross-highlight

<br>

- **Cross-highlighting**: Selecting a value in one visual highlights the related data in visuals such as column and bar charts. Cross-highlighting doesn't remove the unrelated data from those visuals. The unrelated data is still visible but dimmed.
- **Cross-filtering**: Selecting a value in one visual acts more like a filter in other visuals, such as line charts and scatter charts. In those visuals, only the related data remains visible. The unrelated data isn't visible, just as you'd see with a filter.

To remove the highlighting, select the value again, or select any empty space in the same visual.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3_30.gif)

<br>

#### Drill-down filters

<br>

Get automatically added to the filter pane when you use the drill-down functionality for a visual in your report. If you can edit a report, you can edit or clear the filter in the pane. You can't delete, hide, lock, rename, or sort this filter because it's associated with the drill-down functionality of visuals.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/Day3_31.png)

<br>

#### Cross- drill filters

<br>

Cross-drill filters are automatically added to the pane when a drill-down filter is passed to another visual on the report page via the cross-filter or cross-highlight feature. Even if you can edit a report, you can't delete, clear, hide, lock, rename, or sort this filter because it's associated with the drill-down functionality of visuals. You also can't edit this filter because it comes from drilling down in another visual

<br>

#### Drill-through filters

<br>

There are two types of drill-through filters. The first type is the one that invokes the drill-through. If you can edit a report, you can edit, delete, clear, hide, or lock this type of filter. The second type is the drill through filter that gets passed to the target, based on the page-level filters of the source page. You can edit, delete, or clear this transient type of drill through filter. You can't lock or hide this filter for end users.

<br>

#### URL filters

<br>

URL filters get added to the pane by adding a URL query parameter. If you can edit a report, you can edit, delete, or clear the filter in the pane. You can't hide, lock, rename or sort this filter because it's associated with the URL parameter. To remove the filter, you remove the parameter from the URL.

<br>

#### Pass-through filters

<br>

Pass-through filters are visual-level filters created through Q&A. If you can edit a report, you can delete, hide, or sort these filters in the pane. However, you can't rename, edit, clear, or lock these filters.

<br>

### Slicers in Power BI

<br>

Slicers are another way of filtering. They narrow the portion of the dataset that is shown in the other report visualizations.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/Day3_32.gif)

<br>

Slicers are a great choice when you want to:

- Display commonly used or important filters on the report canvas for easier access.
- Make it easier to see the currently filtered state without having to open a drop-down list.
- Filter by columns that are unneeded and hidden in the data tables.
- Create more focused reports by putting slicers next to important visuals.

<br>

#### Create a Slicer

<br>

1. On the left pane, select the Report icon to open the file in the Report View.
2. On the Overview page, with nothing selected on the report canvas, select the Slicer icon in the Visualizations pane to create a new slicer.
3. With the new slicer selected, from the Fields pane, select District > DM to populate the slicer.

The new slicer is now populated with a list of district manager names and their selection boxes.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/Day3_33.png)

<br>

Resize and drag the elements on the canvas to make room for the slicer. Note that if you resize the slicer too small, its items are cut off.
Select names on the slicer and notice the effects on the other visualizations on the page. Select names again to deselect them, or hold down the Ctrl key to select more than one name. Selecting all names has the same effect as selecting none.

Alternately, select Format (paint roller icon) in the Visualizations pane to format your slicer.

Slicer list items are sorted in** ascending order**, by default. To reverse the sort order to descending, select the _ellipsis_ (...) in the top right corner of the slicer and choose Sort descending.

<br>

#### Control the slicers

<br>

As you choose values in the list and date sliders you just created, notice the effects on the other visualizations. The filtered data is an intersection of the values selected in both slicers. Use visual interactions to exclude some page visualizations from being affected by others

1. Go to the Overview page of the report, and then select the slicer you previously created.
2. On the Power BI Desktop menu, select the Format menu under Visual Tools and then select Edit interactions.
3. Filter controls, each with a Filter and a None option, appear above all the visuals on the page. Initially, the Filter option is preselected on all the controls.
4. Select the None option in the filter control above the visualization chart to stop the slicer from filtering it.
5. Select the OpenDate slicer, and then select the None option above the visualization chart to stop this slicer from filtering it.

Now, as you select names and date ranges in the slicers, the visualization chart is unchanged.

#### Sync slicers

With the Sync slicers pane, you can sync the slicer to these pages, so that slicer selection on any page affects visualizations on all three pages.

1. On the Power BI Desktop View menu, select Sync slicers

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3_34.png)

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3_35.png)

<br>

2. On the page of the report, select the slicer.
3. In the Sync column of the Sync slicers pane, select the pages. This selection causes the slicer to sync across these three pages.
4. In the Visible column of the Sync slicers pane, select the New Stores page.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3_36.png)

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3_37.png)

<br>

5. Observe the effects of syncing the slicer and making it visible on the other pages.

<br>

If you sync a slicer to a page but don't make it visible on that page, slicer selections made on the other pages still filter the data on the page.

<br>

#### Filtering slicers

<br>

You can apply visual-level filters to slicers to reduce the list of values that are displayed in the slicer. For example, you might filter out blank values from a list slicer, or filter out certain dates from a range slicer. When you do this it only affects the values that are shown in the slicer, not the filter that the slicer applies to other visuals when you make a selection.

<br>

#### Format slicers

<br>

Different formatting options are available, depending on the slicer type. By using Horizontal orientation, Responsive layout, and Item coloring, you can produce buttons or tiles rather than standard list items, and make slicer items resize to fit different screen sizes and layouts.

1. With the District Manager slicer selected on any page, in the Visualizations pane, select the Format icon to display the formatting controls.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day3_38.png)

<br>

2. Select the drop-down arrows next to each category to display and edit the options.

- General options (format)
- Under Format, select General, select a color under Outline color
- For Orientation, Vertical is selected by default. Select Horizontal to produce a slicer with horizontally arranged tiles or buttons, and scroll arrows to access items that don't fit in the slicer.
- Turn On the Responsive layout to change the size and arrangement of slicer items according to the view screen and slicer size.
- Concatenate: `CONCATENATE(<text1>, <text2>)`
- Parameters:
  - `text1` - The text strings to be joined into a single text string. Strings can include text or numbers.
  - `text2` - You can also use column references.
- Return value: The concatenated string.

<br>

**Remarks**:

<br>

- The `CONCATENATE` function joins two text strings into one text string. The joined items can be text, numbers, or Boolean values represented as text, or a combination of those items. You can also use a column reference if the column contains appropriate values.
- The `CONCATENATE` function in DAX accepts only two arguments, If you need to concatenate multiple columns, you can create a series of calculations or, better, use the concatenation operator (&) to join all of them in a simpler expression.
- If you want to use text strings directly, rather than using a column reference, you must enclose each string in double quotation marks. This function is not supported for use in DirectQuery mode when used in calculated columns or row-level security (RLS) rules.

Here is an example:

```shell
CONCATENATE(Customer[LastName], CONCATENATE(", ", Customer[FirstName]))
```

</details>

---

#### :pencil2: Check for Understanding - Class activity

> 🕰️ 10 min (+ 10 min Review)

<details>
  <summary> Click for Instructions: Activity 3 </summary>

1. What are the different standard filters available in Power BI?
2. What are the differences between filters and slicers?

</details>

<details>
  <summary>Click for Solution: Activity 3 solutions</summary>
    
1. What are the different standard filters available in Power BI?
    
- Visual filter applies to a single visual on a report page. You see visual level filters when you select a visual on the report canvas. Even if you can't edit a report, you can select a visual and filter it.
- Page filter applies to all the visuals on the report page.
- Report filter applies to all pages in the report.
- Drill-through filter With drill0through in the Power BI service and Power BI Desktop, you create a destination report page that focuses on a specific entity, such as a supplier. From the other report pages, users can right-click a data point for that entity and drill through to the focused page.

2. What are the differences between filters and slicers?

- [Power BI Slicers and filters by prologika.com](https://prologika.com/power-bi-slicers-and-filters/)
- [Comparison between Power BI slicer and filter by addendanalytics.com](https://addendanalytics.com/comparison-between-power-bi-slicer-filter/)

</details>

---

:sandwich: **LUNCH BREAK**

> 🕰️ 60 min

---
