[Blog.docx](https://github.com/harshak2001/blog_app/files/13856600/Blog.docx)

# Blog_App

## Overview
This project is a full-stack application with a frontend (client) and a backend (server) component. The frontend is built using React, while the backend is built using Node.js and Express. The communication between the frontend and backend is facilitated through API calls. The backend uses MongoDB as the database to store and retrieve data.

## Project Structure

The project is organized into two main folders: `client` and `server`.
### Client (Frontend)
The frontend is a React application with the following structure:

- **src**: Contains the source code for the React application.
  - **components**: Reusable React components used throughout the application.
  - **scenes**: React components representing different pages of the application.
  - **state**: Redux-related files such as actions, reducers, and store configuration.
  - **theme.js**: Stylesheets, possibly organized by components or pages.
  - **App.js**: The main entry point for the React application.
  - **index.js**: Renders the React application into the HTML document.
- **public**: Static assets and the HTML file where the React app is rendered.
- **package.json**: Configuration file for Node.js dependencies and scripts.

### Server (Backend)

The backend is a Node.js and Express application with the following structure:

- **src**: Contains the source code for the backend application.
  - **.env**: Configuration files, such as database connection and environment variables.
  - **controllers**: Controllers handling the business logic for different routes.
  - **middleware**: Custom middleware functions.
  - **models**: Mongoose models for interacting with the MongoDB database.
  - **routes**: Express routes defining API endpoints.
  - **index.js**: Main entry point for the backend application.

- **.env**: Environment variables file for configuration settings (create if not present).

- **package.json**: Configuration file for Node.js dependencies and scripts.

## Getting Started

## Dependencies

### Client (Frontend)

- **@emotion/react**: Version 11.11.3
- **@emotion/styled**: Version 11.11.0
- **@mui/icons-material**: Version 5.15.3
- **@mui/material**: Version 5.15.3
- **@reduxjs/toolkit**: Version 2.0.1
- **@testing-library/jest-dom**: Version 5.17.0
- **@testing-library/react**: Version 13.4.0
- **@testing-library/user-event**: Version 13.5.0
- **crypto**: Version 1.0.1
- **formik**: Version 2.4.5
- **os**: Version 0.1.2
- **path**: Version 0.12.7
- **react**: Version 18.2.0
- **react-dom**: Version 18.2.0
- **react-dropzone**: Version 14.2.3
- **react-redux**: Version 9.0.4
- **react-router-dom**: Version 6.21.1
- **react-scripts**: Version 5.0.1
- **redux-persist**: Version 6.0.0
- **stream**: Version 0.0.2
- **web-vitals**: Version 2.1.4
- **yup**: Version 1.3.3

### Server (Backend)

- **bcrypt**: Version 5.1.1
- **body-parser**: Version 1.20.2
- **cors**: Version 2.8.5
- **dotenv**: Version 16.3.1
- **express**: Version 4.18.2
- **gitignore**: Version 0.7.0
- **gridfs-stream**: Version 1.1.1
- **helmet**: Version 7.1.0
- **jsonwebtoken**: Version 9.0.2
- **mongoose**: Version 8.0.3
- **morgan**: Version 1.10.0
- **multer**: Version 1.4.4
- **multer-gridfs-storage**: Version 5.0.2

### Prerequisites

- Node.js installed on your machine
- MongoDB installed and running

### Setup

1. Clone the repository:

   ```bash
   git clone <repository-url>
   ```

2. Install dependencies for both the client and server:

   ```bash
   cd client
   npm install

   cd ../server
   npm install
   ```

3. Create a `.env` file in the `server` directory and configure necessary environment variables:

   ```env
   PORT=3001
   MONGODB_URI=<your-mongodb-uri>
   JWT_SECRET=<your-jwt-secret>
   ```

   Replace `<your-mongodb-uri>` and `<your-jwt-secret>` with your MongoDB connection URI and a secret key for JWT, respectively.

### Running the Application

1. Start the server:

   ```bash
   cd server
   npm start
   ```

   The server will be running on `http://localhost:3001`.

2. In a separate terminal, start the client:

   ```bash
   cd client
   npm start
   ```

   The client will be accessible at `http://localhost:3000`.

### Testing APIs

Explore and test the APIs using tools like [Postman](https://www.postman.com/) or [Insomnia](https://insomnia.rest/). The server exposes endpoints defined in the `routes` folder.

## Additional Information

- The frontend is built with React, utilizing libraries like Material-UI for UI components and Redux for state management.

- The backend uses Express for handling HTTP requests, Mongoose for MongoDB interactions, and JWT for authentication.

- Ensure MongoDB is running and accessible. Update the `.env` file in the `server` directory with the correct MongoDB URI.

- Feel free to customize the project structure, styles, and functionality according to your project requirements.

This README provides a basic guide to set up and run the application. Further documentation can be added based on the specific features and requirements of your application.

