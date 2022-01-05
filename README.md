# Ehopping Application program template

This is based upon the Shopping Cart Using Spring with Bootstrap in session 6



### To run using stand alone spring boot maven plugin

at base of project do a build
```
mvn clean install
```
move to web module and run project
```
cd web
mvn spring-boot:run
```
the project will be served at http://localhost:8080/index.html

### To run using stand alone cargo maven plugin

Alternatively you can use the cargo plugin
```
mvn cargo:run
```
then navigate to http://localhost:8080/shoppingCartApplication/


### To run the project using  in Netbeans embedded Tomcat server

If you right click on the webfacade-example1 project in netbeans and select 'run' netbeans will spin up a tomcat instance and launch your application.

If you are asked for username and password just use the default admin admin.
 
(You must make sure you have stopped any maven started tomcat before you do this.)

You will be able to see the application at http://localhost:8080/shoppingCartApplication/

Note that sometimes the browser caches the old index.html so you may need to enter the correct url to access the app

http://localhost:8080/shoppingCartApplication/home

not

http://localhost:8080/shoppingCartApplication/home.jsp

# System Requirements
The system requirements for this project is listed below 

- Java version 11 or newer.
- Apache Maven 3.8 or newer
- Tomcat 9
- Firefox
# Objective for this project 
The purpose of this project is to create a basic web-based catalogue and shopping cart system that allows users to search for items, add them to a shopping cart, and then purchase them.

## Admin point of view

| Admin | Action | Response|
|------|--------|---------|
| 1 | Admin logs in | Redirects to the admin side of the website | 
| 2 | Admin can view and modify users in the system| leads to a page that only administrators may access|
| 3 | Admin can modify orders | by adding items to the catalogue for the admin and user|
| 4 | Admin can remove users | Deletes the user from the system |
| 5 | Admin can see all the users orders| In the my orders page, the admin may see all of the orders.|

## User point of view

|User | Action | Response|
|------|--------|---------|
| 1 | User enters application Web address in web browser | Links back user to home page |
| 2 | The user must log in to the programme | the user is then taken to the home page
| 3 | The user can add products to their shopping cart using the add button| the item is then added to the shopping cart |
| 4 | Items in the basket or shopping cart can be removed by the user | Removes the item and removes the amount immediately|
| 5 | By tapping the pucharse button, the user can purchase the things | takes the user to the checkout |
| 6 | The right card information is entered by the user | The program verifies the credit card information and validates it
| 7 |If the user forgets to submit his or her credit card information | An error notice appears, informing the user that further information is required|
| 8 | If the user provides incorrect information| To correct the information, an error notice appears |
| 9 | If the user inputs the correct information | A verification notice will appear on the screen |
| 10 | The my orders page allows users to view their orders | its takes them to the order page where their orders have been choosen|



