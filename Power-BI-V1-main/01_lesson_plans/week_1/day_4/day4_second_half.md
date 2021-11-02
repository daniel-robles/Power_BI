# Lesson 7.8 - Analyzing with Power BI

<br><br>

### Lesson Duration: 4 hours (including Lab)

<br>

- **Purpose**: The purpose of this lesson is to reiterate the things that students have learned in the week and put it all together in the form of a case study. We will first discuss the case study in class - explain what is the business problem being solved here, what is the data available, and what process we would follow to answer the business questions. We will also touch on one additional topic in this class - how to use the Analytics pane. The students will see how to use trend lines.

<br>

## Pre-requisites

To complete this lesson the student would need:

- Completed all previous lessons
- Installed Power BI Desktop
- Analysis_test.xlsx file
- Access to all datasets used in class and lab (students have access to this [repository](https://github.com/ironhack-edu/power-bi-resources) - liked to their Student Portal)

---

## Learning Objectives

After this lesson, students will be able to:

- Demonstrate understanding of Power BI based on a real-world example (Case Study)
- Use the Analytics pane

<br><br>

### Session 1

> 🕰️ 40 min

#### Key Concepts

- Use the Analytics pane in Power BI Desktop
- Case Study discussion

<details>
<summary> Click for Session Detail:  Use the Analytics pane in Power BI Desktop </summary>

In visualization and BI, once you've got your report and visuals ready, you might still want to do some further analysis. For example, you might want to highlight a line indicating the minimum, mean or maximum values in the chart. In Power BI, the analytics pane captures all the analytical options available for any selected chart at your disposal. In this guide, you will learn how to explore and implement the analytics pane in the Power BI desktop.

**Note**: Load `analytics_test.xlsx` as a data source on Power BI Desktop. Students will have access to this file in the Resources folder (with all other files).

To begin, you will need a chart, table, or matrix:

- Create a clustered column chart
- Drag the variable Month into the Axis field
- and `Loan_disbursed` in the Values field

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_analytics_1.jpg)

<br>

- Once you have a chart selected, you might want to perform several analytical operations on it.
- To look at the options available, select the chart, and look at the Analytics option.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_analytics_2.jpg)

<br>

It looks like a little magnifying glass.

- Click on the Min line option as shown above and click Add.
  You can change the Color and Transparency as shown below, and this will create the resulting output.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_analytics_3.jpg)

<br>

- Repeat the process for the Max line option, and you can keep a different color for contrast.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_analytics_4.jpg)

<br>

The minimum and maximum lines are good, but often, as analysts, you want to look at the average line.

- Click on the Average line and click Add. You can change the Color and Transparency as shown below. This will create the resulting output.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_analytics_5.jpg)

<br>

Outlier detection is an important task in business intelligence and machine learning. One of the common techniques of doing this is to cap the outlier points with certain percentile values. In this case, you will select the tenth and ninetieth percentile points for outlier detection.

- Start by removing the lines by clicking on the x sign. This is not necessary, but you can do it to understand the percentile line better.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_analytics_6.jpg)

<br>

- Click on the Percentile line and click Add. Set the percentile value to 90.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_analytics_7.jpg)

<br>

The output shows that the line around the ninetieth percentile value is plotted in the chart.

- To add the tenth percentile value, click again on Add as shown above, and set the percentile value to 10.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day4_new/day4_analytics_8.jpg)

<br>

Now you have the chart with the required percentile values. The values outside these two percentile lines will be considered outliers. In this case, the values $24 million, $48 million, and $49 million are outliers.

Analytical skills are one of the most sought-after and in-demand skillsets of this decade. It is a sector-agnostic skill and is used in every organization across sectors. Power BI Desktop provides many useful analytical features in the analytics pane, and this knowledge will help you strengthen your analytics and business intelligence capabilities.

</details>

<details>
<summary> Click for Session Detail: Discuss the case study </summary>

> :exclamation: Note for instructor: Refer the [case study file](https://github.com/haggarw3/Power-BI-V1/blob/main/02_lean_lessons/week_1/day_4/case-study.md) for the instructions on this session. Students have access to the same file.

> :exclamation: Note for instructor: This is more like a "Code Along" where the students will replicate the plots as the instructor would go over them.

> :exclamation: Note for instructor: We will not have the Class Activity for this session as the students will work on the lab with the same case study.

</details>

---

:coffee: **BREAK**

> 🕰️ 10 min

---

### :pencil2: Practice - Lab

> 🕰️ 120 min (To Finish the Lab) + 60 mins (To discuss)

<details>
  <summary> Click for Instructions: Lab </summary>

For maintenance purposes and to have a single source of truth, use this link to get to the lab instructions. This link will take you to the same content that is presented to students.

- [Lab | Case Study](https://github.com/haggarw3/Power-BI-V1/blob/main/02_lean_lessons/week_1/day_4/lab-7.08-case_study.md)

</details>

<details>
  <summary>Click for Solution: Lab solutions</summary>

The solution is provided as an MP4 file, a link to the [recording can be found here](https://ironhack.zoom.us/rec/share/RfvUVNgBmqA6t6qbuVfp6PMtXaIF5jUlsUf0zK4vT32SMLYcKtuC-MeIq56z7Dzk.6VGOBI4tj2UxPLaR?startTime=1623418961000).

</details>

---

> End of the day
