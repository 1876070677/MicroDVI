# Migrating Monolithic Web Applications to Microservice Architectures Considering Dependencies on Databases and Views
This folder contains replication packages accompanying our paper.

## Subject web applications
+ ### JPetStore2
    - JPetStore 2 is a web application built on Spring 3, Spring Web MVC, and MyBatis 2.
    - https://github.com/KimJongSung/jPetStore
+ ### JPetStore6
    - JPetStore 6 is a web application built on Spring 5, Stripes, and MyBatis 3.
    - https://github.com/mybatis/jpetstore-6
+ ### PetClinic
    - PetClinic is a web application built on Spring Boot, Thymeleaf, and Spring Data JPA.
    - https://github.com/spring-projects/spring-petclinic
+ ### ShoppingApp
    - ShoppingApp is a web application built on JSP Model 2 and JDBC.
    - https://github.com/manhduydl/Shopping-web-Jsp-Servlet
+ ### DayTrader
    - DayTrader is a web application built on Java EE, JSP Model 2, JSF, EJB, and JDBC.
    - https://github.com/WASdev/sample.daytrader7
## Project structure
+ ### Ground truth
    - This folder contains the microservice identification results is identified by experts for the subject web applications.
    - A raw of ground truth consists of the component name, the component type, and component's microservice label.
    - For each web app, the labels refer to the following microservices.
    - JPetStore2: 0 (Order service), 1 (Account service), 2 (Cart service), 3 (Catalog service), C (Common component), U (Utility), N/U (Not used)
    - JPetStore6: 0 (Order service), 1 (Account service), 2 (Cart service), 3 (Catalog service), U (Utility)
    - PetClinic: 0 (Vet service), 1 (Visit service), 2 (Customer service), U (Utility), N/U (Not used)
    - ShoppingApp: 0 (Order service), 1 (Account service), 2 (Cart service), 3 (Catalog service), C (Common component), U (Utility)
    - DayTrader: 0 (Benchmarking service), 1 (Account service), 2 (Portfolio service), 3 (Quotes service), 4 (System configuration service), C (Common component), U (Utility), N/U (Not used)
+ ### Baselines
    - This folder contains the microservice identification results of baselines.
    - Bunch produces different results each time for the same input data, so we get 10 results from Bunch and use the best one.
    - ### **MEM:** 
    - MEM utilizes a web app stored in a repository (e.g., GitHub) as its input and the MST (Minimum Spanning Tree) algorithm in terms of  semantic, logical, and contributor coupling. We use semantic coupling.
    - reference: https://github.com/gmazlami/microserviceExtraction-backend
    https://github.com/gmazlami/microserviceExtraction-frontend
    - ### **Bunch:** 
    - Bunch utilizes a module dependency graph (MDG) as its input and the hill climbing algorithm for clustering.
    - reference: https://github.com/ArchitectingSoftware/Bunch
    - ### **Mono2micro:** 
    - Mono2Micro utilizes execution traces and the hierarchical clustering algorithm.
    - reference: https://github.com/rahlk/ASE21-Tutorial
+ ### Results
    - This folder contains the results used in the research questions.
    - ### RQ1
    - This section uses table and view information to validate how they affect the accuracy of clustering.
    - ### RQ2
    -
    - ### RQ3
    -
    - ### RQ4