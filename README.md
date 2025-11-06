Cognifyz Internship Task 6: Database Integration and User Authentication
Overview
This project demonstrates database integration and secure user authentication using Node.js, Express, and MongoDB Atlas, as part of my Full Stack Developer internship at Cognifyz Technologies.

Features
User registration and login API

Password hashing with bcrypt

JWT-based authentication

Protected routes accessible only to authenticated users

Technologies
Node.js

Express

MongoDB Atlas & Mongoose

bcryptjs (for password security)

jsonwebtoken (JWT auth)

dotenv (environment variables)

Setup
Clone/download the repo and open in VS Code

Install dependencies:

text
npm install
Create a .env file and add:

text
MONGO_URI=your_mongodb_uri
JWT_SECRET=your_jwt_secret
Start the server:

text
npx nodemon app.js
API Endpoints
POST /api/auth/register
Register a user
Body: { "username": "...", "password": "..." }

POST /api/auth/login
Authenticate user, returns JWT
Body: { "username": "...", "password": "..." }

GET /api/auth/protected
Protected route, requires Authorization: Bearer <token> header

Demo
Demonstrated with Thunder Client (VS Code) — see video/screenshots for API testing.

Acknowledgements
Cognifyz Technologies

Internship guidelines

Hashtags for LinkedIn
#cognifyz #cognifyzTech #cognifyzTechnologies