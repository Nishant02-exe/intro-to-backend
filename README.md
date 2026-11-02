# Node.js, Express & MongoDB Backend API

A RESTful backend API built with Node.js, Express, MongoDB Atlas, and Mongoose featuring user authentication and post management.

## 🚀 Tech Stack

- **Runtime Environment:** Node.js
- **Framework:** Express.js
- **Database:** MongoDB Atlas with Mongoose ORM
- **Authentication:** Password Hashing via `bcrypt`
- **Development Tooling:** Nodemon, Dotenv

## 📁 Project Structure

```text
├── src/
│   ├── config/
│   │   └── database.js
│   ├── controllers/
│   │   ├── user.controller.js
│   │   └── post.controller.js
│   ├── models/
│   │   ├── user.model.js
│   │   └── post.model.js
│   ├── routes/
│   │   ├── user.route.js
│   │   └── post.route.js
│   ├── app.js
│   └── index.js
├── .env
├── .gitignore
├── package.json
└── README.md

## 🛠️ Getting Started

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/Nishant02-exe/intro-to-backend.git](https://github.com/Nishant02-exe/intro-to-backend.git)
   cd intro-to-backend