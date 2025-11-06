# Cognifyz Internship Task 6: Database Integration and User Authentication

## 📚 Overview
This project demonstrates secure user authentication and database integration using Node.js, Express, and MongoDB Atlas. It was completed as part of my Full Stack Developer internship at Cognifyz Technologies.

## 🚀 Features
- User registration and login API
- Password hashing with bcrypt
- JWT-based user authentication
- Protected API routes (accessible only with a valid JWT)

## 🛠️ Technologies Used
- **Node.js** (backend runtime)
- **Express** (web framework)
- **MongoDB Atlas** & **Mongoose** (NoSQL database and ORM)
- **bcryptjs** (password hashing)
- **jsonwebtoken** (JWT-based authentication)
- **dotenv** (environment variable management)

## ⚙️ Setup Instructions

1. **Clone this repository and open in VS Code**
git clone https://github.com/yourusername/Cognifyz_Task6.git
cd Cognifyz_Task6

text

2. **Install dependencies**
npm install

text

3. **Create a `.env` file** in the root directory (refer `.env.example` for structure):
MONGO_URI=your_mongodb_atlas_uri
JWT_SECRET=your_secret_string

text

4. **Start the server**
npx nodemon app.js

text
or
node app.js

text

5. **Test the endpoints** using a REST client such as Thunder Client (VS Code) or Postman.

## 🧪 API Endpoints

| Method | Endpoint                | Description                            | Body Example                                | Headers                         |
|--------|-------------------------|----------------------------------------|---------------------------------------------|---------------------------------|
| POST   | `/api/auth/register`    | Register a new user                    | `{ "username": "user", "password": "pw" }`  |                                 |
| POST   | `/api/auth/login`       | Login, returns JWT token               | `{ "username": "user", "password": "pw" }`  |                                 |
| GET    | `/api/auth/protected`   | Protected route, JWT token required    |                                             | `Authorization: <token>`        |

## 🖥️ Demo

- Tested using **Thunder Client** (VS Code REST client).
- See demo/video files (if submitted) for request/response examples.

## 🙏 Acknowledgements

- **Cognifyz Technologies** — Internship provider and guideline source.
- All mentors and contributors in the Node.js/MongoDB/Express communities.

While building this project, I learned the importance of using environment variables for security and enjoyed integrating JWT authentication for the first time.