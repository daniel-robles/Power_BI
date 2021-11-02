## Bootcamp Final Project

Final projects are to be completed individually. You may ask a classmate for help, but you need to submit an individual project build by your own. Should you need further assistance, you should reach out to your instructional staff.

This project is designed to be challenging and should be completed as

thoroughly as possible.

### Choosing your own Topic:

This project is open ended. You may choose any topic / industry application that you may like. Because the project contains a BI part, you may use a real world problem with some real world dataset. You would be required to conduct some visualizations on this data. So please pick a topic where you can get some kind of business insights. Nevertheless everything is allowed and you should pick a topic that interests you and that could be finished in the next two weeks. (e.g. also a Game that delivers some statistical data would be ok).

:exclamation: At the end of these instructions you would find some additional reources where you may look for free datasets. And again, that list is not exhaustive by any means. Based on the topic of your choice, you might have to conduct your own research to find the relevant data for your problem.

### Instructions:

- Choose problem that interests you and can be implemented in two weeks

- Your application should be based on Java and should use the Spring Framework incl. libraries that we got to know over the course

- You should have a relevant dataset for the problem at the end (that could be used for BI analysis)

- Create a model that corresponds to the data

- You should have at least 3 tables in your database. Database design should be normalized as we learned it in the course

- Use Java JPA to map the tables to domain objects and use JPA repositories for accessing the data.

- Conduct data validation as we learned it in the course

- Build services that contains the logic and consumes data

- Make sure you write tests for the important parts (at least 2 unit tests and 2 integration tests are required)

- REST-Controller: Include at least 1 GET, POST, PUT/PATCH, and DELETE routes.

- Document your REST-Controller with Swagger.

- Create endpoints for each table in your database, to send data to Power BI

- Use the endpoints to connect with Power BI desktop. You are provided with another markdown file "Connecting endpoints with Power BI.md" that has the instructions on how make the connection, for reference.

- After getting data in Power BI from all tables using endpoints, create appropriate relationship between the tables.

- Create a report to provide business insights from the data.

  - What could be some KPIs to measure the health of the process, its efficiency, ways to optimize operations etc

- Implement at least one Microservice (e.g. endpoints for Power BI or some services for you main application; Eureka and other frameworks are optional)

### Deliverables:

- Create at least one GitHub repo.

  - Structure and organize the repo well

  - Provide a readme incl. a UML use case diagram describing the main use cases of your application

- Java code (with requirements described above)

- The repo should include Power BI file

- Prepare a presentation/demo at the end of the two weeks

#### Optional deliverables:

:exclamation: Please note that you will not be assessed on these deliverables. This would only help you learn more and grow technically.

- Include a front end for your application (HTML, CSS, Thymeleaf or JSP)

- Use “Spring Batch” to build a ETL pipeline.

- Use Eureka, Feign, Circuit Breaker and a Cloud Config Server for your Microservice

- Use “Spring Security” for securing access to your application via username and password

- Deploy your application using either one of the services below or any that your group chooses that is not on the following list:

        1. AWS

        2. Openshift

        3. Heroku

        4. Google Cloud

- Publish the report on Power BI Services and create a visually appealing dashboard.

- Embed the dashboard on your web app

**SKY IS THE LIMIT**

#### Additional Resources:

Here are some online resources that you can look at to find data for your project.

1. Kaggle [https://www.kaggle.com/datasets]

2. UCI Machine Learning Repository [https://archive.ics.uci.edu/ml/index.php]

3. GitHub [https://www.github.com]

4. Quandl [https://www.quandl.com/search?filters=%5B%22Free%22%5D]

5. Data World [https://data.world/datasets/open-data]

6. Reddit [https://www.reddit.com/r/datasets/]

7. Academic Torrents [https://academictorrents.com/browse.php?cat=6]

Others useful links:

[https://www.tableau.com/learn/articles/free-public-data-sets]

[https://www.dataquest.io/blog/free-datasets-for-projects/]
