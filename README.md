# burger
A burger logger with MySQL, Node, Express, Handlebars and a homemade ORM 

## Synopsis

Eat-Da-Burger! is a restaurant app that lets users input the names of burgers they'd like to eat. 
Whenever a user submits a burger's name, the app will display the burger on the left side of the page -- waiting to be devoured. Each burger in the waiting area also has a Devour it! button. When the user clicks it, the burger will move to the right side of the page. The app will store every burger in a database, whether devoured or not. Uses Node and MySQL to query and route data into app, and Handlebars to generates the HTML.

## Project Structure

### NPM Packages  

  * express
  * method-override
  * body-parser

### MySQL Table (burgers)

  * **d:** an auto incrementing int that serves as the primary key.
  * **burger_name:** a string.
  * **devoured:** a boolean.
  * **date:** a TIMESTAMP.
  
### orm.js
Creates the methods that will execute the necessary MySQL commands in the controllers. These are the methods retrieve and store data in database.
  
  * **selectAll()**
  * **insertOne()**
  * **updateOne()**

## Motivation

Use Node and MySQL to query and route data in an app, and Handlebars to generate the HTML within an application.
