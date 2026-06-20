# Node.js Authentication API

A secure RESTful API for user authentication built with Node.js, Express, and MongoDB.

## Features

- User registration with password hashing (Bcrypt.js)
- User login with JWT generation
- Protected routes using JWT authentication middleware
- MongoDB integration with Mongoose

## Tech Stack

- **Server:** Node.js, Express
- **Database:** MongoDB, Mongoose
- **Security:** JSON Web Tokens (JWT), Bcrypt.js
- **Environment Management:** Dotenv

## Prerequisites

- [Node.js](https://nodejs.org/) (v14 or higher)
- [MongoDB](https://www.mongodb.com/) (Local or Atlas)

## Getting Started

### 1. Clone the repository

```bash
git clone <repository-url>
cd node-auth-api
```

### 2. Install dependencies

```bash
npm install
```

### 3. Environment Setup

Create a `.env` file in the root directory and add the following variables:

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_super_secret_key
```

### 4. Run the application

**Development mode (with nodemon):**

```bash
npm run dev
```

_Note: You may need to add `"dev": "nodemon server.js"` to your `package.json` scripts if it's not already there._

**Production mode:**

```bash
npm start
```

## API Endpoints

- `POST /api/auth/register` - Register a new user
- `POST /api/auth/login` - Login user and return JWT

## Project Structure

```text
├── config/             # Database configuration
├── controllers/        # Request handlers
├── middleware/         # Auth protection middleware
├── models/             # Mongoose schemas
├── routes/             # API route definitions
└── server.js           # Application entry point
```
