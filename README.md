# taxi-service
Web application with basic UI interface which simulates taxi service work. 
It allows you to create cars, manufacturers, drivers and attach drivers to the cars.
## Features
- driver registration;
- driver authentication;
- create/update/remove a manufacturer;
- create/update/remove a car;
- create/update/remove a driver;
- display list of all manufacturers;
- display list of all cars;
- display list of all drivers;
- display list of all cars by current driver;
- add driver to car.

You can access all of them from the main /index page
after registering as a new driver at /drivers/add page
and signing in at /drivers/login page (you will be redirected to this page if you try to access pages which are not allowed for unsigned drivers).
After that you will have access to all the pages and their functions.
## Project structure (3-layer architecture):
- DAO - Data access layer
- Service - Application logic layer
- Controllers - Presentation layer
## Technologies:
- Java 15
- Git
- Apache Maven
- Apache Tomcat
- MySQL
- JDBC
- Javax Servlet
- JSP
- JSTL
- HTML/CSS
- Checkstyle plugin
## How to run:
1) Download and install TomCat v9.0.52 and MySQL v8.0.28
2) Add a TomCat local configuration:
  - TomCat server - local
  - Deployment - war exploded
  - Application context - /
3) Run SQL script in src/main/resources/init_db.sql to set up database
4) Configure src/main/java/taxi/util/ConnectionUtil.java with your URL, USERNAME, PASSWORD and JDBC_DRIVER