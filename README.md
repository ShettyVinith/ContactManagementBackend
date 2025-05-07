# 📦 Node.js Express JWT Authentication API

A simple user authentication API built with **Node.js**, **Express**, **MongoDB**, **bcrypt**, and **JWT (JSON Web Token)**.  
This API allows users to **register**, **login**, and access **protected routes** using token-based authentication.

---

## 📑 Features

- 📌 User registration with hashed passwords using `bcrypt`
- 📌 User login with email & password verification
- 📌 JWT token generation for authenticated users
- 📌 Protected routes secured using token verification middleware
- 📌 Clean error handling with `express-async-handler`

---

## 🛠️ Tech Stack

- **Node.js**
- **Express**
- **MongoDB**
- **Mongoose**
- **bcrypt**
- **jsonwebtoken**
- **dotenv**

---

## 📦 Installation & Usage

### 1️⃣ Clone the repository

```bash
git clone https://github.com/yourusername/your-repo-name.git
cd your-repo-name

## 📦 Installation & Usage

### 2️⃣ Install dependencies

```bash
npm install

### 3️⃣ Set up environment variables

Create a `.env` file in your project root with the following content:

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
ACCESS_TOKEN_SECRET=your_secure_secret_key

### 4️⃣ Start the server

```bash
npm run dev

Server will run at: http://localhost:5000

## 📬 API Endpoints

| Method | Endpoint               | Description              | Access    |
|:--------|:----------------------|:--------------------------|:-----------|
| POST    | `/api/users/register` | Register a new user       | Public     |
| POST    | `/api/users/login`    | Login user and get token  | Public     |
| GET     | `/api/users/current`  | Get current user info     | Protected  |

## 🔒 Token Usage

After logging in, include the JWT token in the **Authorization** header for protected routes:

```http
Authorization: Bearer <token>

## 📸 Sample Request Payloads

### 📥 Register User

```json
{
  "username": "john_doe",
  "email": "john@example.com",
  "password": "securepassword"
}

### 📥 Login User

```json
{
  "email": "john@example.com",
  "password": "securepassword"
}

## 📄 License

This project is open-source and free to use.

📄 License
This project is open-source and free to use.
