# Taxi Service

Taxi Servise help you with organization of your workers and cars.


### Features of this app :
- Create, delete, update our cars, manufacturers where were build there cars, also work with information about driver.
- Service can add drivers who drive one car, as well as cars that are driven by one driver
- See all created cars, manufacturers or drivers.
- Work with features this app access can only for registered drivers
- In the development we used 3-layered architecture, that means if we need to expand our features It will be easy to implement
***
### Technologies which was used in app :
* Apache Tomcat (v9.0.56)
* Servlet
* JDBC
* MySQL
* HTML, CSS
* JSTL
* JSP
***
### Things that we need to do for correct working application:
1. Firstly we need to install our additional applications. Such as :
    * Apache Tomcat (v9.0.56)
    * MySQL, MySQL Workbench 8.0
   

2. Configure Tomcat in IDE


3. Create a schema in MySQL Workbench using file `src/main/resources/init_db.sql`

    
4. In `src/main/java/mate/util/ConnectionUtil.class` we need to do some changes, and replace with yours :
    * USERNAME, PASSWORD, URL and JDBC_DRIVER
   ```
     //example
     private static final String URL = "jdbc:mysql://localhost:3306/taxi";
     private static final String USERNAME = "root";
     private static final String Password = "qwerty";
     private static final String JDBC_DRIVER = "com.mysql.cj.jdbc.Driver";

5. In src/main/resources/log4j2.xml we need to change fileName:
    * Change fileName to absolute path to file
```
//example
<File name="LogToFile" fileName="C:\*****\IdeaProjects\taxi-service\logs\app.log">
