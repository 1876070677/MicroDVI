# Migrating Monolithic Web Applications to Microservice Architectures Considering Dependencies on Databases and Views
This folder contains replication packages accompanying our paper.

## Subject web applications
+ ### JPetStore2
    - JPetStore2 is an online pet store system. It is built on top of the frameworks Spring 3 and MyBatis 2.
    - https://github.com/KimJongSung/jPetStore
+ ### JPetStore6
    - JPetStore6 is an online pet store system. It uses Spring 5, Stripes, and MyBatis 3.
    - https://github.com/mybatis/jpetstore-6
+ ### PetClinic
    - PetClinic is a veterinary clinic information system based on Spring Boot. It uses Spring Data JPA to interact with a database and Thymeleaf to create user interfaces.
    - https://github.com/spring-projects/spring-petclinic
+ ### ShoppingApp
    - ShoppingApp is a small online store system, which follows JSP Model 2 architectures.
    - https://github.com/manhduydl/Shopping-web-Jsp-Servlet
+ ### DayTrader
    - DayTrader is an online stock trading system using Java EE, JSP Model 2, JSF, EJB, and JDBC.
    - https://github.com/WASdev/sample.daytrader7
## Project structure
+ ### Ground truth
    - This folder contains the microservice identification results identified by experts for the subject web applications.
    - For each web app, the labels refer to the following microservices.
    - JPetStore2: 
        + 0 (Order service), 1 (Account service), 2 (Cart service), 3 (Catalog service), C (Common component), N/U (Not used)
    - JPetStore6:
        + 0 (Order service), 1 (Account service), 2 (Cart service), 3 (Catalog service), C (Common component)
    - PetClinic:
        + 0 (Vet service), 1 (Visit service), 2 (Customer service), N/U (Not used)
    - ShoppingApp:
        + 0 (Order service), 1 (Account service), 2 (Cart service), 3 (Catalog service), C (Common component)
    - DayTrader:
        + 0 (Benchmarking service), 1 (Account service), 2 (Portfolio service), 3 (Quotes service), 4 (System configuration service), C (Common component), N/U (Not used)
+ ### Baselines
    - This folder contains the microservice identification results of baselines.
    - ### **MEM:** 
    - reference: 
        + https://github.com/gmazlami/microserviceExtraction-backend
        + https://github.com/gmazlami/microserviceExtraction-frontend
    - ### **Bunch:** 
    - reference: 
        + https://github.com/ArchitectingSoftware/Bunch
    - ### **Mono2micro:** 
    - reference: 
        + https://github.com/rahlk/ASE21-Tutorial
+ ### Results
    - This folder contains the results used in the research questions.