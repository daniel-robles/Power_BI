# Lesson 7.3 - Power BI Intro

<br><br>

### Lesson Duration: 4 hours

<br>

**Purpose:** This lesson is a short introduction to Power BI and the differences between the different products that are offered in the Power BI ecosystem including PBI services and PBI PRO. We will look at Power BI in more detail, which we will be using majorly through this week and the next to learn how to use the Business Intelligence tool.

<br>

## Pre-requisites

To successfully take this class, the students would need:

- Power BI Desktop Installed

---

## Learning Objectives

After this lesson, students will be able to:

- Identify the differences between PBI desktop, PBI services, and Power BI PRO
- Identify and connect the databases to PBI
- Explore the different windows in Power BI

<br><br>

### Session 1

> 🕰️ 40 min

#### Key Concepts

<details>
<summary> Click for Key Concepts </summary>
    
- What is Power BI 
    - Concept
    - Collection PBI 
    - PBI and your role 
    - The workflow in PBI 
- PBI products ( brief description of each one) 
    - Desktop 
    - Pro
    - Premium 
    - Mobile 
    - Embedded 
- What is PBI desktop
    - Common uses for PBI
- What is PBI Service 
    - Concept
- Comparing the Power BI desktop and PBI services:
    Diagram of comparison 
    - Main features in Power BI 
    - Main features in Power BI services
- Power BI connections 
    Get data from (description): 
    - File
    - Database
    - Power Platform 
    - Azure
    - Online services
    - Other 
     
</details>

:exclamation: Note for instructor: This is only an introduction. We just need to give students an overview of the different tools in the Power BI ecosystem and their macro-level differences in features.

<details>
<summary> Click for Session Details: What is Power BI</summary>

- What is Power BI

  - **_Concept_**
    Microsoft’s Power BI is a cloud-based, business analytics service for analyzing and visualizing data.
    Power BI gives you a platform to be productive and creative with reports and analytics. Churning out useful information from the data and creating visual reports is a multi-step process, let me brief you about the steps

  - **_Collection PBI_**
    Power BI is a collection of software services, apps, and connectors that work together to help you create, share, and consume business insights in the way that serves you and your business most effectively. The Microsoft Power BI service ([app.powerbi.com](app.powerbi.com)), sometimes referred to as Power BI online, is the SaaS (Software as a Service) part of Power BI. In the Power BI service, dashboards help you keep a finger on the pulse of your business. Dashboards display tiles, which you can select to open reports for exploring further.
    Dashboards and reports connect to datasets that bring all of the relevant data together in one place.

  - **_PBI and your role: Four roles are available:_**

    - _Viewer_: This role provides read-only access to workspace items. Read access does provide report/dashboard consumers the ability to not only view but also interact with visuals. Interaction does not mean changing a visual. Also, note that users in this view do not require a Pro License to view reports if the workspace is in Premium mode. Without Premium content, a Pro License is required. (see this tip for some details on license details (Power BI: What I wish I knew when I started?).

    - _Contributor_: This role can access and interact with reports and dashboards. Additionally, this role can create, edit, copy, and delete items in a workspace, publish reports, schedule refreshes, and modify gateways.

    - _Member_: This role can access and interact with reports and dashboards. Additionally, this role can create, edit, copy, and delete items in a workspace, publish reports, schedule refreshes, and modify gateways. Finally, members of this role can also feature dashboards on the service, share items, allow others to re-share items, publish or republish, and APP. This role is also able to add other users to the viewer or contributor role.

    - _Admin_: This role can do all the functions above plus add and remove all users including other Admins.

</details>
    
<br>
    
<details>
<summary> Click for Session Details: Workflow </summary>
    
**Workflow in PBI**: Below is a diagram that shows the analysis workflow in Power BI

<br>
    
![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day2_2.png)

<br>

- **Get Data**: We have two types of sources where you can get data from:
  One is, you can get data from your local sources that means Excel, text files, CSV, SQL on-premises, etc. This is essential all the data that you have at your disposal locally stored in your machine

  Then you can get data from online sources and Power BI both the Desktop and Service offers you a few connectors to do that.

- **Clean data**: Remember GIGO (Garbage IN, Garbage OUT)?
  This essentially means that if you use bad data for analysis, then you will get bad results as well. When we download data from a source, there are usually many inconsistencies with the data. The data is never 100% clean. There we must perform a bunch of operations to improve the quality of the data. Some of them include remove unnecessary columns, add columns (feature extraction) using existing columns, remove products, products that you have to change names. There is a very powerful tool in Power BI to help you do that and it is **Power Query**

- **Model the data**: This includes connecting the right pieces of information together and putting all the right data together for analysis. This is usually done using join operations such as joining tables, joining columns. You also conduct `vlookups` just to make a big table with all the necessary information needed for conducting Business Intelligence and then start analyzing data.

- **Visualize your data**:
  Visualize it and then share it. You have different kinds of charts such as line charts, bar charts, column charts, and map charts. There are also matrices, pivot tables. In power BI there are many kinds of visualizations but if for any reason the visualization that you want is not there, you can go to the office marketplace and try to find the visualization there.
  Some developers develop more visualizations for Power BI and most of them are free, but there are some premium visualizations also, which are paid. If you still don’t find your visualization you can still create your own, we will talk about it on Power BI for developers.

- **Share the data, report**:
  We can publish it to the cloud and share it both publicly or internally with your colleagues, your friends, your partners, and/or on the web.
  We also have the possibility to embed the report somewhere else so we don’t have to use Power BI dot-com. You can just take our report and put it in your app or on a platform or a website.

</details>

<br>

<details>
<summary> Click for Session Details: Power BI products </summary>

- PBI products

  - Desktop

    Power BI Desktop is a free application that you can install on your local computer. The application lets you connect to, transform, and visualize your data. With Power BI Desktop, you can connect to multiple different sources of data, and combine them (often called modeling) into a data model. This data model lets you build visuals, and collections of visuals you can share as reports, with other people inside your organization. Most users who work on business intelligence projects use Power BI Desktop to create reports, and then use the Power BI service to share their reports with others. This is the general process followed by analysts in the industry.

  - Pro

    Power BI Pro is the full version of Power BI, complete with the ability to use Power BI for both building dashboards and reports and unlimited viewing, sharing, and consumption of your created reports (and reports shared by others) - the latter not possible with Power BI Desktop.

    Power BI Pro’s differences against Power BI Desktop:

        - Ability to embed Power BI visuals into apps (PowerApps, SharePoint, Teams, etc)
        - Native integration with other Microsoft solutions (Azure Data Services)
        - Share datasets, dashboards, and reports with other Power BI Pro users
        - Can create App Workspaces and peer-to-peer sharing

  - Premium

    Power BI Premium is the most expensive tier of Power BI currently available and very distinct from the other two versions available on the market. On top of the features and functionality standard to all versions of the service, users of Power BI Premium get: - Increased data capacity limits and maximum performance - Access to one API surface - Ability to embed Power BI visuals into apps (PowerApps, SharePoint, Teams, etc) - Larger storage sizes for extended deployments - Geo distribution, higher refresh rates, isolation, pin to memory, read-only replicas

  - Power BI Report Server

    Power BI Report Server is an on-premises server that lets your business build your BI initiatives on local hardware, and publish and share both Power BI reports and traditional paginated reports created with SQL Server Reporting Services from within your organization’s firewall.
    This option is included with Power BI Premium and suits businesses who want to build their reporting infrastructure on-premises, apply their own governance and policies, and have an investment in a cloud-ready data analytics solution that will seamlessly scale with a future move to the cloud. Power BI Report Server also lets you use the same number of virtual cores provisioned in the cloud on-premises, without the need to split the capacity.

  - Mobile

    By default, all of Power BI’s versions - Desktop, Pro, and Premium - are mobile responsive.
    There are also native smartphone and tablet Power BI Mobile applications for Android, iOS, and Windows devices. These apps act as a complimentary service to view your reports on the go.

  - Embedded

    Power BI Embedded is intended to simplify how ISVs (independent software vendors)and developers use Power BI capabilities with embedded analytics. Power BI Embedded simplifies Power BI capabilities by helping you to quickly add stunning visuals, reports, and dashboards to your apps.

  <br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day2_1.png)

</details>

<br>

#### :pencil2: Check for Understanding - Class activity 1

> 🕰️ 10 min (+ 10 min Review)

<details>
  <summary> Click for Instructions  </summary>

Answer the following questions:

1. Which of the following is not a building block of Power BI?
   - Visualizations
   - Datasets
   - Reports
   - Dashboards
   - Tiles
   - None of the above
2. Components of Power BI include Power Query, Power Pivot, Power View, Power Map, and Power Q&A. What are these components. Do your research and read about them. Discuss the components in class

Refer to the link for help: [Components of Power BI by Intellipaat](https://intellipaat.com/blog/tutorial/power-bi-tutorial/components-of-power-bi/)

</details>

<br>

<details>
  <summary>Click for Solution: Activity 1 solutions</summary>

1. Which of the following is not a building block of Power BI? _A: None of the above_

   - Visualizations: Visualization is a chart, graph, or similar visual representation of data.
   - Datasets: A dataset is the group of data used to create a visualization, such as a column of sales figures. Datasets can be combined and filtered from different sources using built-in connectors.
   - Reports: A report is a group of visualizations on one or more pages; for example, charts, graphs, and maps can be combined to create a report.
   - Dashboards: A dashboard lets you share a one-page visualization with others, who can then interact with your dashboard.
   - Tiles: A tile is a visualization on your dashboard or in your report. As the creator, you can move tiles around.

2. Components of Power BI include Power Query, Power Pivot, Power View, Power Map, and Power Q&A. What are these components. Do your research and read about them. Discuss the components in class.

<br>

### Components of Power BI

<br>

- Power Query: Power Query is the data transformation and mash up the engine. It enables you to discover, connect, combine, and refine data sources to meet your analysis need. It can be downloaded as an add-in for Excel or can be used as part of the Power BI Desktop.

- Power Pivot: Power Pivot is a data modeling technique that lets you create data models, establish relationships, and create calculations. It uses Data Analysis Expression (DAX) language to model simple and complex data.

- Power View: Power View is a technology that is available in Excel, Sharepoint, SQL Server, and Power BI. It lets you create interactive charts, graphs, maps, and other visuals that bring your data to life. It can connect to data sources and filter data for each data visualization element or the entire report.

- Power Map: Microsoft's Power Map for Excel and Power BI is a 3-D data visualization tool that lets you map your data and plot more than a million rows of data visually on Bing maps in 3-D format from an Excel table or Data Model in Excel. Power Map works with Bing maps to get the best visualization based on latitude, longitude, or country, state, city, and street address information.

- Power Q&A: The Q&A feature in Power BI lets you explore your data in your own words. It is the fastest way to get an answer from your data using natural language. An example could be what was the total sales last year? Once you've built your data model and deployed that into the Power BI website, then you can ask questions and get answers quickly.

</details>

---

:coffee: **BREAK**

> 🕰️ 10 min

---

### Session 2

> 🕰️ 40 minutes

#### Key Concepts

- Identify and connect Data sources
  - Connect to Data
  - Transform and clean data
- Change data sources settings
- Select a dataset or create a local dataset
- Select a storage mode

:exclamation: Note for instructor: It might be a good idea to ask the students to open the different files for eg `.xlsx`, `.csv`, and `.txt` using some text editor. For Windows PC they can use Notepad while Mac users can use TextEdit.

<br>

<details>
<summary> Click for Session Details - Connect to Data </summary>

- Identify and connect Data sources

  - Connect to Data
    In this quickstart, you will connect to data using Power BI Desktop, which is the first step in building data models and creating reports.
    With Power BI Desktop, you can connect to many different types of data. These sources include basic data sources, such as `.xlsx`, `.csv`, `txt` etc. You can also connect to online services that contain all sorts of data, such as Salesforce, Microsoft Dynamics, Azure Blob Storage, and many more.

    Follow the tutorial or close the dialog to start with a blank canvas. The canvas is where you create visuals and reports from your data.

  <br>
    
    1. To connect to data, from the Home ribbon select Get data.

  </br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day2_3.png)

<br>
    
    2. The Get Data window appears. You can choose from the many different data sources to which Power BI Desktop can connect.

</br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day2_4.png)

<br>

    3. Since this data source is an Excel file, select Excel from the Get Data window, then select the Connect button.
    Power BI prompts you to provide the location of the Excel file to which to connect. The downloaded file is called "Financial Sample". Select that file, and then select Open.

</br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day2_5.png)

<br>

    4. Power BI Desktop then loads the workbook and reads its contents, and shows you the available data in the file using the Navigator window. In that window, you can choose which data you would like to load into Power BI Desktop. Select the tables by marking the checkboxes beside each table you want to import. Import both available tables.

</br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day2_6.png)

<br>
    5. Once you've made your selections select Load to import the data into Power BI Desktop
    Once you've loaded the tables, the Fields pane shows you the data. You can expand each table by selecting the arrow beside its name. In the following image, the financials table is expanded, showing each of its fields.
</br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day2_7.png)

</details>

<br>

:exclamation: Note to the Instructor: The next part is only an overview to get the students comfortable with the interface of Power BI. We will talk about data types, data cleaning and processing, and data formatting later in more detail.

<br>

<details>
<summary> Click for Session Details - Transform and clean data  </summary>

- **Data cleansing and transformation**
  Data cleansing is the process of removing and detecting inaccurate records from a recordset. It is used to alter data in a given storage resource to make sure that it is accurate and correct. Transformation is a process of filtering out unusable records of the database in the Power BI desktop. The data which is not useful to make a report and analysis, this type of data should be cleaned from our database.

- **Why use data cleansing and transformation?**
  When any data is in the incorrect format and gets some error while creating a visual report then we need to clean the data and transform it so that we can remove incorrect records from the dataset. When we import two or more dataset in Power BI then we need to manage relationships between two or more tables and due to a cleaning issue, this is not done. Then we get some different problems. Now in this situation, we follow the process of data cleansing and data transformation which resolve the issue using power query and save again to the imported file. Because it can solve the issue and establish the relation easily.

Go to the Home Ribbon and click on edit queries.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day2_8.png)

<br>

After that open the edit window on the Power Bi desktop. We can select any one file in one-time power BI to edit the query. When you move to the editor then you can perform many tasks using the editor window function.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day2_9.png)

<br>

When you open the edit window for any table in Power BI then you can perform many operations if you need to change the data type of any column.
Then right-click on the column name and get the data type list of a column. We can change the data type from it.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day2_10.png)

<br>

From this step, we can change the data type of any column of the table. Using Power query editor you can perform the following steps on the table:

- You can merge columns using merge query.
- You can add the column from Add column tab.
- You can import new data using a new source according to requirement.
- You can also edit a new dataset using the enter data table.
- Create parameter and edit parameters from manage parameters.
- You can give the reference, delete and duplicate from the manage tab.
- You can choose the column and remove the column.
- You can keep the row and remove the row.
- You can split the column into two parts.
- You can replace value.
- You can create an append new query.
- You can transpose, revert and count rows.
- You can change the format also.
- You can make a connection to the R script using Run R Script.
- You can use condition formatting on data.
- If you get a new requirement and need to create code in Power BI You can write code in advanced editors.
- You can manage query dependencies from the database.
- You can set the setting of the editor according to requirements.
- You can refresh and load the report using properties in the query editor.

</details>

<br>

<details>
  <summary> Click for Session Details: Storage Modes </summary>

- Select a storage mode
  In Microsoft Power BI Desktop, you can specify the storage mode of a table. The storage mode lets you control whether the Power BI Desktop caches table data in memory for reports. Setting the storage mode provides many advantages. You can set the storage mode for each table individually in your model. This action provides the following benefits:

- Query performance: As users interact with visuals in Power BI reports, Data Analysis Expressions (DAX) queries are submitted to the dataset. Caching data into memory by properly setting the storage mode can boost the query performance and interactivity of your reports.

- Large datasets: Tables that aren't cached don't consume memory for caching purposes. You can enable interactive analysis over large datasets that are too large or expensive to completely cache into memory. You can choose which tables are worth catching, and which aren't.

- Data refresh optimization: You don't need to refresh tables that aren't cached. You can reduce refresh times by caching only the data that's necessary to meet your service level agreements and your business requirements.

- Near-real time requirements: Tables with near-real-time requirements might benefit from not being cached, to reduce data latency.

- Writeback: Writeback enables business users to explore what-if scenarios by changing cell values. Custom applications can apply changes to the data source. Tables that aren't cached can display changes immediately, which allows instant analysis of the effects

As mentioned before, the Storage mode property is a property that you can set on each table in your model and controls how Power BI caches the table data. To set the Storage mode property (or view its current setting), first select the table whose properties you want to view or set:

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day2_11.1.png)

<br>

In the Properties pane, expand the Advanced section, and expand the Storage mode drop-down.

</br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day2_11.2.png)

<br>

You set the Storage mode property to one of these three values:

- Import: Imported tables with this setting are cached. Queries submitted to the Power BI dataset that return data from Import tables can be fulfilled only from cached data.

- DirectQuery: Tables with this setting aren't cached. Queries that you submit to the Power BI dataset—for example, DAX queries—and that return data from DirectQuery tables can be fulfilled only by executing on-demand queries to the data source. Queries that you submit to the data source use the query language for that data source, for example, SQL.

- Dual: Tables with this setting can act as either cached or not cached, depending on the context of the query that's submitted to the Power BI dataset. In some cases, you fulfill queries from cached data. In other cases, you fulfill queries by executing an on-demand query to the data source.

Changing the Storage mode of a table to Import is an irreversible operation. Once set, this property can't later be changed to either DirectQuery or Dual.

</details>

<br>

#### :pencil2: Check for Understanding - Class activity

> 🕰️ 10 min (+ 10 min Review)

<details>
  <summary> Click for Instructions: Activity 2 </summary>

1. Which of the following are data sources that can be used in Power BI?

   - Excel
   - Csv
   - Power BI datasets
   - web
   - SQL Server
   - all of the above

2. What can be some of the possible consequences of using the data that is not clean? You can also refer to it as dirty data, inconsistent data, or poor quality data. Think about cases for eg. missing values in the dataset, data with outliers, text information that is not standardized, etc.

Refer to the following links for reference:

- [Most common types of dirty data and how to clean them](https://www.ringlead.com/blog/the-7-most-common-types-of-dirty-data-and-how-to-clean-them/)
- [What is dirty data](https://towardsdatascience.com/what-is-dirty-data-d96abbdf254e)

</details>

<br>

<details>
  <summary>Click for Solution: Activity 2 solutions</summary>

1. What of the following are data sources used in Power BI?

   - all of the above

2. Discuss the link [https://www.ringlead.com/blog/the-7-most-common-types-of-dirty-data-and-how-to-clean-them/](https://www.ringlead.com/blog/the-7-most-common-types-of-dirty-data-and-how-to-clean-them/)

   Cases include:

   - Duplicate values
   - Outdated data
   - Typos
   - Outliers
   - Date time format incorrect
   - Too many missing pieces of information
   - Skewness in the data (more related to Data Science)

</details>

---

:coffee: **BREAK**

> 🕰️ 10 min

---

### Session 3

> 🕰️ 40 min

#### Key Concepts

- Browsing the Interface
  - Common tasks (File, home, insert, modeling, view, help)
  - Canvas area
  - Pages tab
  - Filters pane
  - Visualizations pane
  - Fields pane

:exclamation: Note for instructor: Encourage the students to play around with the interface and learn.

<br>

<details>
<summary> Click for Session Details </summary>

In the Power BI Desktop Report view, you can build visualizations and reports. The Report view has six main areas:

:exclamation: Note to the Instructor: Please note that the Tables in the field section are "Best States for Sunglasses" and "State Codes" but we are not using those tables right now. We are using data from "financial_sample.xlsx". The screenshot below is only for explanatory purposes.

:exclamation: Note to the Instructor: You can continue using the same example as you have used in the previous session.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day2_12.png)

1. The ribbon at the top, which displays common tasks associated with reports and visualizations.
2. The canvas area in the middle, where visualizations are created and arranged.
3. The pages tab area at the bottom, which lets you select or add report pages.
4. The Filters pane, where you can filter data visualizations.
5. The Visualizations pane, where you can add, change, or customize visualizations, and apply drill-through.
6. The Fields pane, which shows the available fields in your queries. You can drag these fields onto the canvas, the Filters pane, or the Visualizations pane to create or modify visualizations.

You can expand and collapse the Filters, Visualizations, and Fields panes by selecting the arrows at the tops of the panes. Collapsing the panes provides more space on the canvas to build cool visualizations.

:exclamation: Note to the Instructor: Please note that the Tables in the field section are "Best States for Sunglasses" and "State Codes" but we are not using those tables right now. We are using data from "financial_sample.xlsx". The screenshot below is only for explanatory purposes.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day2_13.png)

<br>

To create a simple visualization, just select any field in the fields list, or drag the field from the Fields list onto the canvas. For example, drag the Country field from the "Financials" table onto the canvas, and see what happens.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day2_14.png)

<br>

Look at that! Power BI Desktop recognized the names of the countries from the Country field. It contained geolocation data and automatically created a map-based visualization. The Visualizations pane shows information about the visualization and lets you modify it.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day2_15.png)

<br>

The icons show the type of visualization created. You can change the type of a selected visualization by selecting a different icon, or create a new visualization by selecting an icon with no existing visualization selected.
The Fields option in the Visualization pane lets you drag data fields to Legend and other field wells in the pane.
The Format option lets you apply formatting and other controls to visualizations.
The options available in the Fields and Format areas depend on the type of visualization and data you have.
You can show different visualizations on different report pages. To add a new page, select the + symbol next to the existing pages on the pages bar, or select Insert > New Page in the Home tab of the ribbon. To rename a page, double-click the page name in the pages bar, or right-click it and select Rename Page, and then type the new name. To go to a different page of the report, select the page from the pages bar.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day2_16.png)

<br>

Share your work. There are a few ways to share your work. You can distribute the report `.pbix` file like any other file, you can upload the `.pbix` file from the Power BI service, or you can publish directly from Power BI Desktop to the Power BI service. You must have a Power BI account to be able to publish or upload reports to the Power BI service.

To publish to the Power BI service from Power BI Desktop, from the Home tab of the ribbon, select Publish.

<br>

![Image](https://education-team-2020.s3.eu-west-1.amazonaws.com/power-bi/week-1/day2_16.1.png)

<br>

</details>

---

#### :pencil2: Check for Understanding - Class activity

> 🕰️ 10 min (+ 10 min Review)

<details>
  <summary> Click for Instructions: Activity 3 </summary>

1. What is a Power BI report view and what is it used for?
2. Pick any 5 visualization types available in Power BI and describe what they are and how and when are they used (for what kind of data and to conduct what kind of analysis)
   For eg., a scatter plot is used to check the relationship between two variables ie., how a change in one variable impacts the other. Pie charts are used for understanding percentage shares between things.
   Do your own research and discuss.

</details>

<br>

<details>
  <summary>Click for Solution: Activity 3 solutions</summary>

1. What is a Power BI report view, and what is it used for?

   Power BI Desktop includes a Report view, where you can create any number of report pages with visualizations. Report view in Power BI Desktop provides a design experience to create, move visualizations around, copy and paste, merge, and so on. You can work with your queries and model your data to make sure your data supports the best insights in your reports. You can then save your Power BI Desktop file wherever you like, whether it's your local drive or to the cloud.

2. Reference: [https://blog.hubspot.com/marketing/types-of-graphs-for-data-visualization](https://blog.hubspot.com/marketing/types-of-graphs-for-data-visualization)

</details>

---

:sandwich: **LUNCH BREAK**

> 🕰️ 60 min

---
