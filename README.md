# Newsify

## Introduction
Newsify is an innovative and dynamic web application designed to revolutionize the way users consume news. In an era of information overload, Newsify aims to provide a streamlined and personalized news experience, ensuring that users stay informed about the topics that matter most to them.

## Features
- User Authentication (Register, Login, Logout)
- Personalized News Feed
- Create, Edit, and Delete Posts
- Comment on Posts
- Upload and Manage Images
- Secure API with JWT Authentication
- Responsive UI for seamless experience across devices

## Tech Stack
- **Frontend**: React, React Router, Context API, Axios
- **Backend**: Node.js, Express.js, MongoDB, Mongoose, Multer, dotenv, CORS, Cookie-Parser

## Project Structure
```
C:.
├───backend
│   ├───controller
│   ├───models
│   └───routes
└───frontend
    ├───public
    └───src
        ├───assets
        ├───components
        ├───context
        ├───images
        ├───pages
        └───styles
```

## Installation and Setup
### Prerequisites
Ensure you have the following installed:
- Node.js & npm
- MongoDB (local or cloud-based)
- Environment Variables (in `.env` file)

### Backend Setup
```sh
cd backend
npm install
npm start
```

### Frontend Setup
```sh
cd frontend
npm install
npm start
```

## Environment Variables
Create a `.env` file in the backend root directory and add:
```env
MONGO=<your-mongodb-uri>
JWT_SECRET=<your-secret-key>
```

## API Routes
### Authentication
- `POST /api/auth/register` - Register a new user
- `POST /api/auth/login` - Login user
- `POST /api/auth/logout` - Logout user
- `GET /api/auth/refetch` - Refetch user details

### Users
- `GET /api/users/:id` - Get user details
- `PUT /api/users/:id` - Update user details
- `DELETE /api/users/:id` - Delete user

### Posts
- `POST /api/posts` - Create a post
- `GET /api/posts` - Get all posts
- `GET /api/posts/:id` - Get a single post
- `PUT /api/posts/:id` - Update a post
- `DELETE /api/posts/:id` - Delete a post

### Comments
- `POST /api/comments` - Add a comment
- `GET /api/comments/:postId` - Get comments for a post
- `DELETE /api/comments/:id` - Delete a comment

### Image Upload
- `POST /api/upload` - Upload an image

## Deployment
To deploy the frontend:
```sh
npm run build
```
Deploy the backend on platforms like **Heroku**, **Render**, or **DigitalOcean**.

## Happy Coding
