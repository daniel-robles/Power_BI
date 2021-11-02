<!-- # Lab | Database Connections -->

## Introduction

As a data analyst, you will have to work with a big amount of data and different data types. Extracting meaningful insights from your data can be done by using all data sources available and learning how this could be achieved in a correct way using a BI Tool. In this lab, you will use Power BI to load multiple datasets into it, validate that data was correctly loaded, and perform simple manipulations using the PowerBI interface.

Use the **vehicles dataset from resources folder** which comes in different format types. Once you download the files, save them in a folder of your preference.

### Prerequisites

- At this point you should have installed Power BI on your laptop

If you have any doubts about the prerequisites please clarify with your instructor or teaching assistants.

<br>

## Challenge 1 - Load Multiple Datasets

<br>

if you work in a team, every time before you will find With different Data type files. One of the most common is the CSV files (Comma Separated Values) which contain a bunch of information separated by commas. Another is the `xlsx` which are the common Excel files that we are used to working, JSON which is pretty similar to a dictionary (`key: value`), and txt files which could be separated by tabs or pipes.

To solve this point you must:

- Download each file

  - CSV
  - JSON
  - XLSX
  - TXT with pipe - TXT with tab

Load properly in PowerBI (using correct file separator). Check error of loading fo reach case. If appears, describe the error and how did you figure it out.

<br>

- **Step 1:** Save the files in a folder where PowerBI will find them after you save the file.

  Be careful to keep moving the files, if the address changes, your PowerBI file will show up with an error because it doesn't found the source.

<br>

- **Step 2:** Take a look at each attribute (columns)

  It is very important to check that data types are being properly defined:

  - Date fields must be in DateTime
  - Amounts must be numbers
  - IDs must be Strings

  This will help you to create calculations in a better way later, avoiding data type errors.

<br>

## Challenge 2 - Business Sense

<br>

Now that you have loaded all the datasets into PowerBI Desktop, you should start questioning yourself about available data:

- Imagine that you're the owner of the data because it's from your business and you want to start exploring it.
- Figure out what data could help you to complement your insights and write the best approach to get it.

Remember that one of the main roles to start creating analysis that delivers insights and really meaningful data is to start asking the right questions and being eager to get data that compliments the one you already have.

<br>

- **Step 1:** Check your data

  What information do you have with these files? This is an open field but you must try to explain the best possible, go for it!:

  - Remember that you should imagine yourself running your own business and taking the data as if it were yours
  - Start questioning yourself about it. This way you'll begin creating good answers and understand or conclude answers that you didn't see before

<br>

- **Step 2:** What could compliment your data?

  If you could add or get any other data that complements your actual data, What data you'll be looking for?

  - Try to think beyond the borders, see yourself in a position where you want to be, and you'll find the data that will help you to achieve this.
  - Be realistic about this! Sometimes we're so excited with the information that we began to think about data that we won't have because it's no possible (at least you hack some sites :wink: ). Imagine if you want to get the database of the customer of Amazon! It's nearly impossible because this information is confidential, and few people in the world have access to it.

<br>

## External Resources

<br>

- [Power BI Data sources by Microsoft](https://docs.microsoft.com/en-us/power-bi/connect-data/desktop-data-sources)
- [JSON](https://fileinfo.com/extension/json)
