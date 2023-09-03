# ResultRush

ResultRush is a web application designed to help people set, track and achieve personal goals. The app provides a tool for effective goal planning and management, helping users become more productive and successful.  
<br>
<img src="https://github.com/igushkin/result-rush/assets/106703296/e1adf4f2-484c-48d0-9e98-9d64112b045f" width=500px >
<br>

The main functions of the application:  
* Creating SMART goals. Users can create their own goals following the SMART principle. The application helps users to create specific, measurable, achievable, relevant goals and set deadlines for their achievement.
* Dashboard and progress report. The application provides an informative dashboard where users can track progress towards achieving each of their goals. Users can specify which steps have already been completed and which have yet to be completed.

### Demo

[https://resultrushfront.azurewebsites.net/](https://resultrushfront.azurewebsites.net/)

### Built With

* Spring Boot Framework
* Angular Framework
* PostgreSQL
* Microsoft Azure

### Design and Architecture
The application can be represented as the work of three layers independent of each other: a frontend that is implemented using Angular, a backend written on the Spring Framework and database.
<br>
<img src="https://github.com/igushkin/result-rush/blob/main/examples/design.jpg?raw=true" width=500px>
<br>
This is an implementation of the classic three-level architecture of a web application which consists of a presentation layer, application layer and data layer.

### JWT and Spring Security 

The application implements a custom filter based on a JSON WEB Token(JWT). The JWT token can store some payload (user id e.g), which eliminates the need to make an additional request to the database.


### SQL Triggers

The application uses trigPostgreSQL gers to reduce the load on the database and simplify data retrieval requests.

### Presentation Layer

The application uses the concept of components. The components allowed me to flexibly manage the page by encapsulating all the styles, HTML structure and data into each individual component. For example, when displaying the main page, five components are involved: header component, sidebar component, categories component, goals component and footer component.

<br>
<img src="https://github.com/igushkin/result-rush/blob/main/examples/angular-components.jpg?raw=true" width=500px>
<br>

### Deployment

All three layers of the application are deployed as separate services on the Microsoft Azure cloud platform.

### Run locally
#### Prerequisites
* JDK 17
* Node.js 18.17.1
* PostgreSQL 15


```
git clone https://github.com/igushkin/result-rush
```
