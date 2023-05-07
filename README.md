# CRUD-AND-JWT ASSIGNMENT 
**Tasks:**

1. Set up a new Node.js project and install the required dependencies (TypeScript, Express.js, JWT library, database driver, etc.).
2. Create a database schema for the items table, and write the necessary queries to perform CRUD (Create, Read, Update, Delete) operations on the database.
3. Implement the authentication system using JWT. Users should be able to register, log in, and log out.
4. Create middleware functions to handle common tasks such as error handling, request logging, and authentication checks.
5. Create RESTful endpoints for the API that allows users to create, read, update, and delete items from the database. Use the middleware functions from Step 4 to handle these requests.
6. Write tests to ensure that the API functions as expected, covering all possible use cases.

-----------------------------------------
JWT ASSIGNMENT: 

1. server.js:
Configure middleware functions to handle JSON parsing and URL encoding.
Implement the /register route to handle user registration. It checks if the username is available, hashes the password, and inserts the user into the database.
Implement the /login route to handle user login. It verifies the credentials, generates a JWT token, and sends it back to the client.
Implement the /logout route to handle user logout. It invalidates the current JWT token and sends a response to the client.

2. auth.js:
Implements helper functions for user authentication and token generation/validation.
Defines a function to generate a JWT token with the provided payload and expiration time using the jsonwebtoken library.
Defines a middleware function to authenticate incoming requests by verifying the JWT token in the Authorization header.

3. index.html:
Provides a simple HTML form for user registration and login.
Displays success alerts when a user is registered, logged in, or logged out.

4. index.js:
Handles form submissions for user registration and login.
Sends POST requests to the server with the entered username and password.
Displays success alerts on successful registration, login, or logout.
Updates the UI to show the logout button when the user is logged in.
