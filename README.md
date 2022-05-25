# :oncoming_taxi: Taxi Service :oncoming_taxi:
<p align = "center">
<img alt="Taxi picture" height="500" src="src/main/resources/images/Daniel.jpg">
  </p>

# :closed_book: General info:
Taxi service App is a web-app, built based on SOLID principles, with connection to database powered by JDBC.

### :globe_with_meridians: You can use this project [online](https://tax1-service.herokuapp.com/)

# :eyes: About project:
This is taxi service, where we first need to register or authenticate and after we can:

- Add/Delete/ShowAll driver
- Add/Delete/ShowAll manufacturer
- Add/Delete/ShowAll car
- Add driver to car

# :abacus: Technologies used:

- Java 11
- Apache Maven
- Apache Log4j2
- Apache Tomcat 9
- Custom Injector
- Java Servlets
- JDBC
- MySQL

# :computer: If you want to run this project on your computer, you need:
1. To have or install MySQL and Apache Tomcat 9.0.50
2. Clone this project:
```bash
git clone https://github.com/VladyslavLn/taxi-service.git
```
3. Create DB schema and tables using `init_db.sql` file from `resources` directory
4. Configure `ConnectionUtil` class to create connection to db:
```java
public class ConnectionUtil {
    private static final String URL = "YOUR_MySQL_URL";
    private static final String USERNAME = "YOUR_MySQL_USERNAME";
    private static final String PASSWORD = "YOUR_MySQL_PASSWORD";
}
```
6. add Tomcat configuration to your project. Use `/` as your Tomcat application context
7. configure `log4j2.xml` from `resources` directory. Add correct path to the `app.log` file

After all these steps you will be able to run this project locally.