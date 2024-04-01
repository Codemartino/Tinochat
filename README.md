# TinoSocial

TinoSocial is a comprehensive social media web application built using React.js for the frontend, Express.js for the backend, and MongoDB as the database. It provides users with a platform to connect, share, and interact with each other through posts, comments, and likes.

## Features

- **User Authentication**: Users can sign up and log in securely to access the platform.
- **Profile Management**: **Users can edit their profiles, including updating their information and profile picture.**
- **Post Creation and Interaction**: Users can create posts, like posts, comment on posts, and view posts from other users.
- **Feed**: Users have access to a personalized feed displaying posts from users they follow.
- **Search**: Users can search for other users and posts based on usernames, names, or keywords.
- **Notifications**: **Users receive notifications for new likes and comments on their posts.**
- **API**: The backend provides a RESTful API for frontend communication, which can be tested using Postman.

## Technologies Used

- **Frontend**: React.js, Redux (for state management), React Router (for routing)
- **Backend**: Express.js, Node.js
- **Database**: MongoDB (with Mongoose as ODM)
- **Authentication**: JSON Web Tokens (JWT)
- **API Testing**: Postman

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Codemartino/tinosocial.git
  
   ```

2. Install dependencies for both frontend and backend:

   ```bash
   cd tinosocial/client
   npm install
   cd ../api
   npm install
   ```

3. Set up environment variables:

   Create a `.env` file in the `server` directory and add the following variables:

   
   PORT=5000
   MONGODB_URI=mongodb://localhost:27017/tinosocial
   JWT_SECRET=your_jwt_secret
   

4. Start the backend server:

   
   cd api
   npm start
   

5. Start the frontend development server:

   
   cd client
   npm start
  

6. Access the application in your browser at `http://localhost:3000`.

## API Endpoints

- **POST `/api/auth/register`**: Register a new user.
- **POST `/api/auth/login`**: Log in a user.
- **GET `/api/users/:username`**: Get user profile by username.
- **PUT `/api/users/:username`**: Update user profile by username.
- **GET `/api/posts`**: Get all posts.
- **GET `/api/posts/:id`**: Get post by ID.
- **POST `/api/posts`**: Create a new post.
- **PUT `/api/posts/:id`**: Update post by ID.
- **DELETE `/api/posts/:id`**: Delete post by ID.
- **POST `/api/posts/:id/like`**: Like a post by ID.
- **POST `/api/posts/:id/comment`**: Add a comment to a post by ID.
- **DELETE `/api/posts/:postId/comment/:commentId`**: Delete a comment on a post by post ID and comment ID.

## Usage

1. Sign up for a new account or log in with existing credentials.
2. Create a new post by clicking on the "Create Post" button.
3. Interact with posts by liking, commenting, or viewing other users' profiles.
4. Search for users or posts using the search feature.
5. Update your profile information and profile picture as needed.
6. Explore the personalized feed to discover new posts from users you follow.
7. Receive notifications for new likes and comments on your posts.

## Contribution

Contributions are welcome! If you have any ideas, suggestions, or bug fixes, feel free to open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

---

Thank you for using TinoSocial! If you encounter any issues or have feedback, please don't hesitate to reach out. Happy socializing! 🚀🌟
