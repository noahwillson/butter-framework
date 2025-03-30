# HTTP Server with Authentication and Post Management

This project is a simple HTTP server built using a custom framework called `Butter`. It provides basic authentication, user management, and post management functionalities. The server is designed to handle JSON-based API requests and serve static files for a front-end application.

## Features

- **User Authentication**:

  - Login with username and password to receive a session token.
  - Logout to invalidate the session token.

- **User Management**:

  - Retrieve user information.
  - Update user details (username, name, and optionally password).

- **Post Management**:

  - Retrieve a list of posts with author information.
  - Create new posts.

- **Static File Serving**:

  - Serve `index.html`, `styles.css`, and `scripts.js` for the front-end.

- **Middleware**:
  - JSON body parsing for API requests.
  - Authentication middleware to protect specific routes.

## API Endpoints

### Authentication Routes

- **POST `/api/login`**  
  Logs in a user and returns a session token.  
  **Request Body**:
  ```json
  {
    "username": "liam23",
    "password": "string"
  }
  ```
