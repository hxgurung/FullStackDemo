# FullStackDemo

Executive Summary

The Travlr application has three main parts which are index, user and travel files. The view files contains the files which are used to view the websites by the end users. The handlerbars are used to format the application page to format the code by using hbs tags instead of hard coding the same code in every page. The controllers does the input and send the results as required. 

MEAN stack is used for the development of this application with the combination of Angular.js, express.js and MongoDB. The application used MEAN methodology where MongoDB is the database, Express is the webserver , Angular is used for front end and the Node is being used as the backend for the application. It is highly depended on internet connection and may cause loss or corruption of data if the internet connection is not stable. MVC routing is highly used to integrate all the parts handlebars allowed to reuse and format the code.


Design Constraints

In terms of MEAN stack, it is better for developing large scale applications where frequents updates are pushed. The major design constraints would be the financial issues with this project. Considering the financial cost , we wont be able to get best developers to work with and also time will be a great constraint. The project may not be properly tested if we lack enough developers to test the code for the application. These all issues revolves around the financial constraints. The other constraints are minimal with this application, MongoDB is widely used for storing data in cloud.
 


System Architecture View

Component Diagram

 

A text version of the component diagram is available: CS 465 Full Stack Component Diagram Text Version. 


The three main components are client, server, and database. The server and clients are hosted with ports and the data stored in database are passed to the client when the server receives the request from the client. The server does all the authentication, and the information are accessed based on the request from database.

The client session is built as soon as the application is started and specific url request are sent. As we all know it does require a steady internet connection and compatible web browser as well as all the database should also be up and running. The client requested data are fetched from database and before that the client will need to establish the session with server where authenticating part will let the user to send the request to server. Followed by the authorized request, the server returns all the client requests as per the code and information from Database are accessed and provided to client. 
Sequence Diagram
 

Here in the diagram, it shows the component of application where Angular is used for Client-side and NodeJS/Express/Mongoos is used for Server-side. The Actor send the request which is received by the controller. The controller identifies the request types and send the http request using various controller functions as per the client request. The data request is later abstracted by Mongoose and is processed. The processed information is later sent by callback function and later displayed to the actor through the webpages.


 

Class Diagram

 
The class diagram shows the process of the application execution during its use.  It covers the various features of the applications like hotel and trip details, membership level and even the flight and cruise details. Whenever a user tries to access the websites through a secure connection, the website allows the user to navigate and help them get the information which they are seeking. If the user wants the trip details, the http client will get connected with database and fetch the trip information to display. It is a a flow of website interactions for various interaction within the websites.

The travel agent class does the functioning like booking hotel, flights, hotels, and cruises. It collects the information from all the other classes to present a itinerary class. The booking class provides the data to itinerary class from the information gathered from all the booking classes where dates, trip information are stored. The booking class has various features like prices, seat , cabins and even the star rating of the hotel. 
Whereas in the user/member side, the Member_Account class has the member information like member number, status. The Membership_Admin class consists of the rewards information for the member like credit points, and validate the credits against the user profile.

API Endpoints

<Exposing RESTful endpoints is a design approach to enable an application to participate in a larger ecosystem. Document each endpoint in the table below, including the HTTP method, purpose, URL, and notes.>

Method	Purpose	URL	Notes
GET	Retrieve all the list of trips	<api/trips>	Retrieves a list of all trips in the database.
GET	Retrieve a particular detailstrip	api/trips/:tripsId	Return the particular trip details from the database

The User Interface
  
  
 
Angular and Express are both frameworks used for web development, but they serve different purposes and have different project structures. Angular is a front-end JavaScript framework for building single-page applications (SPAs) while Express is a back-end framework for building web applications and APIs. 
Angular project structure usually includes a directory for components, services, modules, and assets. The components handle the presentation logic and interact with the services, which handle the business logic. Express projects typically have a simpler structure, with a main server file that sets up the server and routes, and a public directory for serving static assets such as HTML, CSS, and JavaScript files. 
In summary, the Angular project structure is more complex and organized than the Express HTML customer-facing page structure, reflecting the different purposes and capabilities of these two frameworks. 
To test the functionality of SPA and all the REST APIs can be done by creating a local testing environment which is the local host server. First step would be ensuring the application compiles perfectly and we can also add console.log to debug the issues and also utilize dev tools and google chrome resources.
The process of testing an Angular SPA to ensure that it is working with an API to GET and PUT data in the database involves creating a separate testing environment, writing unit, integration, and end-to-end tests, running the tests, and fixing any issues that are identified. Studio3t can be used to verify the APIs are updating the data in database and the Postman can assist to test these APIs.

