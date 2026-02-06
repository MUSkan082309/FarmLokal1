# JWT Authentication Template (Node.js + TypeScript)

A simple and clean JWT authentication starter template built with **Node.js, Express, MongoDB, and TypeScript**.  
Includes user registration, login, and protected routes with strong type safety.

---

## 🚀 Features
- User Registration & Login
- JWT-based Authentication
- Password Hashing
- Protected Routes
- TypeScript Support

---

## 📌 Routes
- **POST** `/api/user/register`  
  Register a new user (name, email, password)

- **POST** `/api/user/login`  
  Login user and receive JWT token

- **GET** `/api/protected`  
  Protected route (requires JWT)  
  Header: `Authorization: Bearer <token>`

---

## ⚙️ Setup

1. Rename `.env.example` to `.env`
2. Add the following environment variables:

```env
JWT_SECRET=your_secret_key
JWT_LIFETIME=30d
MONGO_URI=your_mongodb_connection_string
PORT=3000
