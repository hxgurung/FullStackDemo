# CS465 Full Stack Development - MEAN

## Architecture

### Compare and contrast the types of frontend development you used in your full stack project, including Express HTML, JavaScript, and the single-page application (SPA).

During the the full stack project development, there were a few different types of front end code that were used in different parts of the application.  The customer facing site was developed originally in Express HTML and then converted over to a .hbs view to help with rendering speeds by not having to fully load every component of the site at each refresh.  HTML is static and client facing, which means it can;t interact with backend databases to dynamically update information.  Javascript is a frontend and backend coding language that is used to add dynamic elements to the webpage.  This was used to pull trip information from the MongoDB database so that the page can change dynamically based on user interaction.  A single-page application is a website that doesn't fully refresh the page based on user interactions like an HTML page would.  This is particularlly useful in giving the website a local/native application feel when interacting with the applicaiton itself. 

### Why did the backend use a NoSQL MongoDB database?

The backend used a NoSQL MongoDB database because of its ease of modifying schema based on scaling and functionality changes, as well as the ability to rapidly scale horizontally because of its non-relational nature of the database.

## Functionality

### How is JSON different from Javascript and how does JSON tie together the frontend and backend development pieces?

JSON is a standardized way to format object data that can be easily read by Javascript to form it into a literal Javascript object.  This makes it easy for Javascript to take the data and form it into a object in the Javascript language.  This ties frontend and backend development together by creating a way for data/ Javascript objects to be stored on the backend and used in different situations based on what the frontend is requesting the data for. This also means that the data just has to be stored once but can be pulled and used in a variety of ways.

### Provide instances in the full stack process when you refactored code to improve functionality and efficiencies, and name the benefits that come from reusable user interface (UI) components.

An instance that code was refactored to improve functionality and efficiency is that the trip card versus trip list components.  Having two seperate components that render the same information is inefficient, but having the each trip being rendered separately but part of the whole works better in the overall functionality of the site.  Reusing UI components is benificial because it decreases overall size of an application, makes the development process quicker, and decreases the chance of errors and vulnerabilities introduced into the system (provided the component is secure).

## Testing

### Methods for request and retrieval necessitate various types of API testing of endpoints, in addition to the difficulties of testing with added layers of security.

There are a few ways of testing endpoints prior to adding security.  The first is by just going to the localhost web address for the API endpoint to see if the page successfully loads the data or what type of error it throws if an error occurs.  An application that tests HTTP requests like Postman is ideal however, because it can also take security measures and inputs into place to test endpoints that might be protected from unauthenitcated users.

### Explain your understanding of methods, endpoints, and security in a full stack application.

In a full stack application, the methods of the website is what drives the functionality and dynamics of a webpage.  Methods like GET, POST, PUT, and DELETE are http requests that can be used to retrieve or modify the database so that the functionality can be implemented.  These are driven on the backend by using the functions of the database (.create, .findOne, .find, .findOneAndUpdate) to modify the database depending on the clients needs.  Endpoints are the results of the methods as seen by the admin or the client side of the application.  Endpoints should be tested so that they function how they should and display data properly or throw errors if an actual error occurs.  Security is another layer of code that is added to prevent unauthorized or unauthenticated users from accessing or modifying te database.  An example of this would be to add or edit a trip in the database.  These API endpoints need to be protected so that unauthorized users cant tamper with the database.

## Reflection

### How has this course helped you in reaching your professional goals? What skills have you learned, developed, or mastered in this course to help you become a more marketable candidate in your career field?

This course has helped me immensely in terms of professional development.  With working full time and going to school full time, its been hard to really nail down what I wanted to go into after school, what languages interested me, and if I wanted to work front or back end in the developement world.  This course has helped me narrow down the direction I want to go career wise and what other skills I need to pursue to be competitive in the job market.  I think that the biggest skill that I have developed in this process is that I have gained a better understanding how different modules or components of code link together and how they can be used to build a finished product.  
