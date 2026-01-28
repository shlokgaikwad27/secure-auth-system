# Secure Authentication System

A simple backend authentication system built using Flask and JWT.  
This project demonstrates secure user registration, login, and protected routes.

---

## 🚀 Features
- User Registration
- Secure Password Hashing using bcrypt
- User Login with JWT Token
- Protected API Routes
- SQLite Database

---

## 🛠 Tech Stack
- Python
- Flask
- Flask-JWT-Extended
- bcrypt
- SQLite

---

## ⚙️ How to Run the Project

### 1️⃣ Install Dependencies
```bash
pip install flask flask-jwt-extended bcrypt
2️⃣ Run the Application
python app.py
API Endpoints
🔹 Register User

POST /register

{
  "username": "admin",
  "password": "admin123"
}

🔹 Login User

POST /login

Response:

{
  "access_token": "JWT_TOKEN"
}

🔹 Protected Route

GET /profile

Header:

Authorization: Bearer JWT_TOKEN
