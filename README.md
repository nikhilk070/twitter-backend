Backend Project Description: Social Media Platform API
Overview
This project is a backend API built using Node.js, Express.js, and MongoDB for a basic social media platform. Users can create accounts, log in, make posts, like posts, and upload profile pictures. It features secure authentication and authorization using JWT (JSON Web Tokens) and bcrypt for password hashing.

Features
1. User Authentication
Sign Up: Users can create an account by providing a username, email, and password.
Login: Users can log in using their registered email and password.
Password Hashing: Passwords are securely stored using bcrypt.
JWT Authentication: Secure endpoints with token-based authentication for user sessions.
2. User Profile
Profile Picture Upload: Users can upload and update their profile picture.
Profile Management: Users can view and update their profile details.
3. Posts
Create Post: Users can create new posts with text and optional image uploads.
View Posts: Users can view all posts or specific user posts.
Delete Post: Users can delete their posts.
4. Likes
Like Post: Users can like and unlike posts.
Like Count: Each post displays the number of likes it has received.
Technology Stack
Node.js: Server-side JavaScript runtime.
Express.js: Web framework for building RESTful APIs.
MongoDB: NoSQL database for storing user data and posts.
Multer: Middleware for handling multipart/form-data, used for profile picture and post image uploads.
JWT: For securing endpoints and managing user sessions.
Bcrypt: For hashing passwords to enhance security.
Cloudinary (optional): For hosting and managing images if not storing locally.
API Endpoints
User Authentication
POST /api/signup: Register a new user.
POST /api/login: Log in an existing user.
User Profile
GET /api/user/:id: Get user profile details.
PUT /api/user/:id: Update user profile details.
POST /api/user/upload-profile-pic: Upload a new profile picture.
Posts
POST /api/posts: Create a new post.
GET /api/posts: Retrieve all posts.
GET /api/posts/:id: Retrieve a specific post.
DELETE /api/posts/:id: Delete a post.
Likes
POST /api/posts/:id/like: Like a post.
POST /api/posts/:id/unlike: Unlike a post.
