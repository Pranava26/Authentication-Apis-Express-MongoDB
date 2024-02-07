Authentication APIs with Express and MongoDB:
Overview:
This project provides a set of RESTful APIs for user authentication built using Express.js and MongoDB. It includes APIs for user registration (signup), user login, fetching user details, and more. Additionally, it implements protected routes using middleware for authentication, ensuring that certain endpoints are accessible only to authenticated users.

Features:
1. User Authentication APIs:
   1. Signup Endpoint: Allows users to create an account by providing necessary information such as username, email, and password.
   2. Login Endpoint: Enables users to authenticate themselves by providing valid credentials (username/email and password).
   3. User Details Endpoint: Retrieves details of the authenticated user, such as username and email.

2. Protected Routes:
   1. Utilizes middleware to protect certain routes from unauthorized access. Users must be authenticated to access these routes.

3. JWT Token Authentication:
   1. Implements JSON Web Tokens (JWT) for authentication and authorization.
   2. Upon successful login, a JWT token is generated and provided to the client. This token is then used to authenticate subsequent requests.

Usage:
1. Register a new user: POST /api/signup
   1. Provide username, email, and password in the request body.
2. Login with existing credentials: POST /api/login
   1. Provide username/email and password in the request body.
3. Get user details: GET /api/userdetails
   1. Requires a valid JWT token obtained during login.

Dependencies:
1. Express.js: Web framework for Node.js
2. MongoDB: NoSQL database for storing user information
3. jsonwebtoken: Library for generating and verifying JWT tokens
4. bcryptjs: Library for hashing passwords securely

Contributing:
Contributions are welcome! If you have suggestions, improvements, or feature requests, feel free to open an issue or create a pull request.
