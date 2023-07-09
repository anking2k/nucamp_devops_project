# Cookies Management Application
The Cookies Management Application is a web-based application that allows users to manage user information and gather details on their favorite cookie. The fictional use-case is for a bakery that desires to stay on top of favorite cookie flavors from their user's database so that they can continually stay informed on what "new flavors" may be a hit at the bakery. It provides features for creating users, retrieving user information, updating user details, and deleting users. Additionally, it allows users to create cookies, retrieve cookie information, update cookie details, and delete cookies. The application is built using Flask, a Python web framework, and utilizes a PostgreSQL database for data storage.

**Features**
The Cookies Management Application offers the following features:

**User Management:** Users can create a new user, retrieve information about a specific user, update user details, and delete users.
**Cookie Management:** Users can create a new cookie, retrieve information about a specific cookie, update cookie details, and delete cookies.
**API Endpoints**
The application provides the following API endpoints:

**User Management Endpoints**
Create a new user:

**HTTP Verb: POST**
Endpoint URL: /users/
Special Details: The request body should contain the user's information (username, email).
Retrieve a specific user:

**HTTP Verb: GET**
Endpoint URL: /users/{user_id}/
Special Details: The user_id parameter represents the unique identifier of the user.
Update the information of a user:

**HTTP Verb: PUT/PATCH**
Endpoint URL: /users/{user_id}/
Special Details: The user_id parameter represents the unique identifier of the user. The request body should contain the updated user information.
Delete a user:

**HTTP Verb: DELETE**
Endpoint URL: /users/{user_id}/
Special Details: The user_id parameter represents the unique identifier of the user.
Cookie Management Endpoints
Create a new cookie:

**HTTP Verb: POST**
Endpoint URL: /cookies/
Special Details: The request body should contain the cookie's information (flavor).
Retrieve a specific cookie:

**HTTP Verb: GET**
Endpoint URL: /cookies/{cookie_id}/
Special Details: The cookie_id parameter represents the unique identifier of the cookie.
Update the information of a cookie:

**HTTP Verb: PUT/PATCH**
Endpoint URL: /cookies/{cookie_id}/
Special Details: The cookie_id parameter represents the unique identifier of the cookie. The request body should contain the updated cookie information.
Delete a cookie:

**HTTP Verb: DELETE**
Endpoint URL: /cookies/{cookie_id}/
Special Details: The cookie_id parameter represents the unique identifier of the cookie.
Database Tables
The application utilizes a PostgreSQL database for data storage and consists of the following tables:

**Users**
Columns:
id (Primary Key, Integer)
username (String, Unique)
email (String, Unique)

**Cookies**
Columns:
id (Primary Key, Integer)
flavor (String)

**Getting Started**
To run the Users and Cookies Management Application locally, follow these steps:

- Install the necessary dependencies specified in the requirements.txt file.
- Set up a PostgreSQL database and update the database connection details in the application configuration.
- Run the application using the appropriate command (e.g., python app.py).
- Access the application using the provided API endpoints and test its functionality.

**Contributors**
Andre' King

**License**
This project is licensed under the MIT License. Feel free to customize the README file as per your project's requirements.
