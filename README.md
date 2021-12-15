![](images/header.png)
# Taxi Service

This application created to help taxi services to keep their data and convenient manipulate it.
#### Functionality before authentication:

* Register a new driver.
* Login registered driver to a system.
* 
#### Additional functionality after authentication:

* Add a new car to database
* Add a new manufacturer to database
* Display all cars, registered in system
* Display all drivers, registered in system
* Display all manufacturers, registered in system
* Connect driver and car
* Display all cars for authenticated driver 
* Logout

### Implementation details
This project implements 3-tier architecture
*Presentation layer (controllers)
*Service layer (services)
*Data access layer (DAO)

Project compiles with SOLID principles.

All data stored in MySQL tables.
Relations between them are described at image below:

![](images/join-db-diagram.png)

### Technologies used

*Java 
*Maven
*log4j
*MySQL
*JDBC
*Servlet
*JSTL
*Apache Tomcat
*HTML, CSS

### Setup

* Install IntellijIDEA Ultimate version [from here](https://www.jetbrains.com/idea/download/)
* Configure Apache Tomcat [version 9.0.56](https://tomcat.apache.org/download-90.cgi)
* for Windows: check if you have [Microsoft Visual C++ Redistributable Latest Version](https://docs.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-170)
* Install MySQL and MySQL Workbench [from here](https://dev.mysql.com/downloads/) (you can use installers)
* Create new database and create connection
* Customize your connection here: ```src/main/java/taxi/util/ConnectionUtil.java```
* Copy and run script from ```src/main/resources/init_db.sql``` at MySQL Workbench
* Change fileName path in ```src/main/resources/log4j2.xml``` to your own. Feel free you use absolute path
* Configure ```src/main/java/taxi/controller/InjectDataController.java``` to inject test data to your database
* Run Tomcat
* Go to the main page
* Register new driver or login as existing one
* Enjoy :)