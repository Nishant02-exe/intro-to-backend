# Intro to Backend API

A RESTful backend service built with Node.js, Express, and MongoDB Atlas. This application provides user authentication and post management with password encryption and persistent cloud storage.

## Key Features

- User authentication (Registration and Login) with secure password hashing via Bcrypt
- Persistent database storage using MongoDB Atlas and Mongoose schema validation
- Modular RESTful API architecture following separation of concerns (Routes, Controllers, Models)
- Global CORS configuration and JSON payload handling
- Centralized error handling for standard HTTP response statuses

## Tech Stack

- **Runtime Environment:** Node.js
- **Web Framework:** Express.js
- **Database:** MongoDB Atlas
- **ORM / ODM:** Mongoose
- **Security:** Bcrypt
- **Environment Management:** Dotenv
- **Development Tooling:** Nodemon

## Project Architecture

intro-to-backend/
├── src/
│   ├── config/
│   │   └── database.js      # Database connection configuration
│   ├── controllers/
│   │   ├── user.controller.js # Request handlers for authentication
│   │   └── post.controller.js # Request handlers for posts
│   ├── models/
│   │   ├── user.model.js     # User schema and pre-save hooks
│   │   └── post.model.js     # Post schema
│   ├── routes/
│   │   ├── user.route.js     # User endpoints setup
│   │   └── post.route.js     # Post endpoints setup
│   ├── app.js               # Express application initialization & middleware
│   └── index.js             # Server entry point
├── .env                     # Environment variables (Git-ignored)
├── .gitignore
├── package.json
└── README.md

## Getting Started

### Environment Setup

Create a `.env` file in the root directory and configure the following variables:

PORT=4000
MONGODB_URI=mongodb+srv://<username>:<password>@cluster.mongodb.net/<database>?retryWrites=true&w=majority

### Installation & Execution

1. **Clone the repository:**
   git clone https://github.com/Nishant02-exe/intro-to-backend.git
   cd intro-to-backend

2. **Install project dependencies:**
   npm install

3. **Start the development server:**
   npm run dev

## API Documentation

### User Routes (/api/v1/users)

| Method | Endpoint | Description | Request Body Example |
| :--- | :--- | :--- | :--- |
| `POST` | `/register` | Register a new user | `{"username": "nishant", "email": "nishant@test.com", "password": "password123"}` |
| `POST` | `/login` | Authenticate existing user | `{"email": "nishant@test.com", "password": "password123"}` |