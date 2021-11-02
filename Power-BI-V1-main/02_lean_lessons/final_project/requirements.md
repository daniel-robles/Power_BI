<!-- ## Power BI + Java | Final Project -->

### Basic rules

<br>

- **Individually completed project:** Final project should be completed individually, which means you shouldn't be collaborating with your classmates on this assignment. Should you need assistance, you should reach out to your instructional staff.
- **Real-world challenges + Choosing your own topic**: This project is open-ended. Because the project contains a BI part, you can choose any topic/industry application that you like. But please make sure that it is a real-world problem with some real-world dataset. You are required to present this data visually, so please pick a topic where you can get some meaningful business insights. Nevertheless, everything is allowed and you should pick a topic that interests you and that could be finished in the next two weeks. (e.g. also a _game_ that delivers some statistical data would be ok).
  ​
  :exclamation: At the end of these instructions, you would find some additional resources where you may look for free datasets. And again, that list is not exhaustive by any means. Based on the topic of your choice, you might have to conduct your own research to find the relevant data for your problem.
  ​
- **Needs to be extra challenging: This project is more open-ended than the midterm project. Use this as an opportunity to challenge yourself and learn new things.**

<br>

## Requirements

<br>

Your project must meet all of the requirements below:

<br>

- Choose a real-world problem. Choose a problem that interests you and that solution can be developed in two weeks.

- Your application should be based on Java and should use the Spring framework including the libraries that you learned to use during the course.

- Get a relevant dataset for the problem. Make sure it could be used for BI analysis. (Read further to find the hints on where to look for the dataset.) ​

- Create a model that corresponds to the data

  - You should have at least **3 tables** in your database.
  - Database design should ensure that there is **no data redundancy**, i.e. the tables should be normalized.
    <!-- _Hint_: Check this [resource](https://www.studytonight.com/dbms/database-normalization.php) on database normalization. -->

<!-- - "Seed" the database (get the data in your SQL database). -->

- Use Java JPA to map the tables to domain objects and use JPA repositories for accessing the data.

- Conduct data validation as you learned in the course.
  - You have to ensure that the **data is reliable and consistent**. For all the tables, define data validation rules and incorporate all those rules in your code before that data is made available for later analysis or some other purpose.
    <!-- _Hint 1_: Check this [resource](https://www.safe.com/what-is/data-validation/) on data validation.
    _Hint 2_: Check this [resource](https://www.precisely.com/blog/data-quality/5-characteristics-of-data-quality) on data quality characteristics. -->
    ​
- Build a robust API using a microservices architecture. The API should contain the logic and consume the data.
​
<!-- - Test the whole app with testing libraries covered so far during the class. -->

- Make sure you write tests for the important parts (at least 2 unit tests and 2 integration tests are required)
  ​
- REST-Controller: Include at least one of `GET`, `POST`, `PUT`/`PATCH` and `DELETE` routes.

- Document your REST-Controller with Swagger.
  ​
- Create endpoints for each table in your database to send data to Power BI.
  ​
  <!-- - Secure the endpoints through authentication. -->
  ​
- Use the endpoints to connect with the Power BI desktop. In the next unit, you can have lean guidelines on how to connect endpoints with Power BI. You can check them as a reference.
  ​
- After getting data in Power BI from all tables using endpoints, create an appropriate relationship between the tables.
  ​
- Create a report to provide business insights from the data.

  - What could be some KPIs to measure the health of the process, its efficiency, ways to optimize operations, etc.?

- Implement at least one Microservice (e.g. endpoints for Power BI or some services for your main application; Eureka and other frameworks are optional)
​
<!-- - Publish the report on Power BI Services and create a visually appealing dashboard. -->

<br>

## Deliverables

- Create a GitHub repository.

  - Make sure that the repository is well structured and organized.
  - Provide adequate and complete documentation of the process and results and analysis. Make sure the repository has a README file that includes a UML use case diagram describing the main use cases of your application.

- The repository should include:

  - Java code
  - Power BI file and the data files used (such as CSV, Excel, or SQL)

- Prepare a presentation/demo at the end of the two weeks.

<br>

### Optional deliverables

<br>

:exclamation: Please note that you will not be assessed on these deliverables. This would only help you learn more and grow technically.
​

- Include a front end for your application (HTML, CSS, Thymeleaf, or JSP).
- Use “Spring Batch” to build an ETL pipeline.
- Use Eureka, Feign, Circuit Breaker, and a Cloud Config Server for your Microservice.
- Use "Spring Security" for securing access to your application via username and password.
- Deploy your application using either one of the services below or any that your group chooses that is not on the following list:

  1. AWS
  2. OpenShift
  3. Heroku
  4. Google Cloud

- Publish the report on Power BI Services and create a visually appealing dashboard.
- Embed the dashboard on your web app.

<br><br>

## Additional Resources

<br>

Here are some online resources that you can look at to find data for your project.
​

- [Kaggle](https://www.kaggle.com/datasets)
- [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/index.php)
- [GitHub](https://www.github.com)
- [Quandl](https://www.quandl.com/search?filters=%5B%22Free%22%5D)
- [Data World](https://data.world/datasets/open-data)
- [Reddit](https://www.reddit.com/r/datasets/)
- [Academic Torrents](https://academictorrents.com/browse.php?cat=6)
- [Database Normalization](https://www.studytonight.com/dbms/database-normalization.php)
- [Data Validation](https://www.safe.com/what-is/data-validation/)
- [Data Quality characteristics](https://www.precisely.com/blog/data-quality/5-characteristics-of-data-quality)
- [Free public datasets](https://www.tableau.com/learn/articles/free-public-data-sets)
- [Free datasets for projects](https://www.dataquest.io/blog/free-datasets-for-projects/)
