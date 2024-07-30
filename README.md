# MERN Notes App

A simple web application for taking short notes.

## Tech Stack

**Client:** React + Typescript, Redux Toolkit, RTK Query, TailwindCSS  
**Server:** Node, Express, JWT Token  
**Database:** MongoDB with Mongoose

## Features

- User Authentication with JWT tokens
- CRUD operations for notes (Create, Read, Update, Delete)
- Minimal UI
- Mobile Friendly
- Optimistic updates for better user experience

## Screenshots

![App Screenshot](https://user-images.githubusercontent.com/68722478/156499720-dd8295d7-6604-4ab0-9d70-1a07437712ef.png)

## Detailed Requirements

### Backend

- **Express.js Server:**
  - Set up an Express.js server.
  - Use MongoDB to store user and notes data.
  - Implement authentication middleware to protect routes.
  
- **APIs:**
  1. **POST /signup** - Sign up a new user.
  2. **POST /login** - Authenticate a user and return a JWT token.
  3. **GET /notes** - Retrieve all notes for the authenticated user.
  4. **POST /notes** - Create a new note.
  5. **PUT /notes/:id** - Update an existing note.
  6. **DELETE /notes/:id** - Delete a note.

### Frontend

- **React App Pages:**
  - **Login** - User login page.
  - **Signup** - User signup page.
  - **Notes List** - Display a list of notes.
  - **Note Detail/Edit** - Display and edit note details.
  
- **State Management:**
  - Use Redux Toolkit for state management.
  - Implement RTK Query for API requests and caching.
  - Create a `userSlice` in Redux to manage logged-in user data and cache it to prevent data loss on tab close.

- **Optimistic Updates:**
  - Implement optimistic updates using RTK Query for a better user experience (optional but recommended).

## Deliverables

- Complete source code hosted on a GitHub repository.
- A README file with clear instructions on how to set up and run the project.
- A brief document explaining your approach, any assumptions made, and how you ensured security and efficiency in your code.

## Setup Instructions

### Backend

Navigate to the `backend` directory:

```bash
cd backend
```

1. **Install dependencies:**

    ```bash
    npm install
    ```

2. **Set up environment variables in a `.env` file:**

    ```plaintext
    MONGO_URI=your_mongo_db_uri
    JWT_SECRET=your_jwt_secret
    ```

3. **Start the server:**

    ```bash
    npm start
    ```

### Frontend

1. **Navigate to the frontend directory:**

    ```bash
    cd ../frontend
    ```

2. **Install dependencies:**

    ```bash
    npm install
    ```

3. **Start the development server:**

    ```bash
    npm start
    ```

## Approach and Assumptions

### Security

- Used JWT tokens to secure API endpoints.
- Passwords are hashed before storing in the database.

### Efficiency

- Utilized RTK Query for efficient state management and caching.
- Implemented optimistic updates to improve user experience.

### Assumptions

- Users will have unique email addresses.
- JWT tokens are stored securely on the client side.

## Conclusion

This project provides a robust foundation for a note-taking application with user authentication and note management features. The use of modern technologies ensures a seamless and efficient user experience.




