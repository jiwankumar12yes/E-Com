# E-Com
The Node.js app initializes an Express server with middleware for authentication and logging, routing HTTP requests to controllers, while interacting with MongoDB through Mongoose and centralizing error handling in applicationError.js, with configuration settings managed in mongoose.js and .env files.
Here's a high-level overview of the flow:

Server Entry Point (server.js):

This is the entry point of your Node.js application.
It initializes the Express server and sets up middleware, routes, and other configurations.
Middleware:

Middleware functions are executed before the request reaches the route handlers.
jwtAuth.middleware.js handles JWT authentication.
logger.middleware.js is responsible for logging incoming requests.
Routes:

Routes define the endpoints and map them to specific controller methods.
authRoutes.js handles authentication-related routes.
productRoutes.js handles routes related to product operations.
userRoutes.js handles routes related to user operations.
Controllers:

Controllers contain the application logic for handling requests and sending responses.
authController.js contains methods for authentication logic.
productController.js contains methods for product-related logic.
userController.js contains methods for user-related logic.
Models:

Models define the data schema and interact with the database using an ORM (Object-Relational Mapping) like Mongoose.
product.js defines the schema and methods for product data.
user.js defines the schema and methods for user data.
Repositories:

Repositories encapsulate database operations related to specific entities.
cartitems.repository.js contains methods for CRUD (Create, Read, Update, Delete) operations on cart items.
Error Handling:

applicationError.js defines a custom error handler for handling application errors.
Configuration:

mongoose.js contains configurations for connecting to MongoDB.
Environment Variables:

.env file(s) store environment-specific configuration variables.
Other Files:

app.js might be the main application file that initializes the Express app.
package.json and package-lock.json manage project dependencies.
logs.log appears to be a log file.

--image of folder Structure.
![image](https://github.com/jiwankumar12yes/E-Com/assets/116423769/1e4e9501-7f10-43d7-9aa0-a11c6ecc4fd1)


--Running Server
![Screenshot (145)](https://github.com/jiwankumar12yes/E-Com/assets/116423769/26766159-a628-4887-b5db-3db6730adc9b)


--Live SignUp Page
![Screenshot (147)](https://github.com/jiwankumar12yes/E-Com/assets/116423769/62dcf895-dc00-4632-b4b6-1c2eebf38ff8)


--After Submitting SignUp Deatils
![Screenshot (148)](https://github.com/jiwankumar12yes/E-Com/assets/116423769/28abb461-bb97-4808-a914-52d85b67f2b6)

--Submission Details in Database

![Screenshot (149)](https://github.com/jiwankumar12yes/E-Com/assets/116423769/bfd1ed1d-824b-483e-b27b-f51dfea4e624)




--Successful PostMan Testing


![Screenshot (150)](https://github.com/jiwankumar12yes/E-Com/assets/116423769/86472656-760c-4c4f-b59b-4e9db2922187)




--JWT Authentication Key By PostMan For LogIn.


![Screenshot (152)](https://github.com/jiwankumar12yes/E-Com/assets/116423769/37d4be5e-6943-4a17-813d-a8d360d3fcdd)





--Successfully Logged in by JWT Authentication


![Screenshot (153)](https://github.com/jiwankumar12yes/E-Com/assets/116423769/a06942b4-1611-47aa-b34b-457b02917167)





