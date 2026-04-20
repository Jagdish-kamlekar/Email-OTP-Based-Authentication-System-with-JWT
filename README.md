# 🔐 Email & OTP Authentication System

A secure authentication system built using **Spring Boot** and **React.js** that supports:

* Email OTP Verification
* Mobile OTP Verification (Twilio)
* JWT Authentication
* Forgot Password with Reset Link
* Redis for OTP & Token storage

---

## 🚀 Features

✅ User Registration (Email + Mobile)
✅ Email & SMS OTP Verification
✅ JWT-based Login Authentication
✅ Secure Password Encryption (BCrypt)
✅ Forgot Password (Email/SMS Link)
✅ Reset Password with Token Validation
✅ Redis-based OTP & Token Expiry
✅ Protected APIs with Spring Security

---

## 🛠️ Tech Stack

### Backend:

* Java 17
* Spring Boot
* Spring Security
* JWT (JSON Web Token)
* Redis
* JPA (Hibernate)
* MySQL

### Frontend:

* React.js
* Axios
* React Router
* Tailwind CSS

### External Services:

* Twilio (SMS OTP)
* SMTP / Email Service

---

## 🔁 Authentication Flow

### 🔐 Registration Flow

1. User registers with email & mobile
2. OTP sent to Email & Mobile
3. User verifies OTP
4. Account activated

---

### 🔑 Login Flow

1. User logs in with email & password
2. JWT token generated
3. Token used for protected APIs

---

### 🔄 Forgot Password Flow

1. User enters email/mobile
2. Reset link sent via Email/SMS
3. User clicks link → frontend opens reset page
4. New password submitted with token
5. Password updated securely

---

## 📌 API Endpoints

### Auth APIs

| Method | Endpoint              | Description     |
| ------ | --------------------- | --------------- |
| POST   | /auth/sign-up         | Register user   |
| POST   | /auth/verify-otp      | Verify OTP      |
| POST   | /auth/login           | Login           |
| POST   | /auth/forgot-password | Send reset link |
| POST   | /auth/reset-password  | Reset password  |

---

## ⚙️ Setup Instructions

### 🔹 Backend

```bash
git clone https://github.com/your-username/email-otp-auth-system.git
cd backend
```

Update `application.properties`:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/db_name
spring.datasource.username=root
spring.datasource.password=your_password

jwt.secret=your_secret_key
```

Run:

```bash
mvn spring-boot:run
```

---

### 🔹 Frontend

```bash
cd frontend
npm install
npm run dev
```

---

## 🔐 Security Highlights

* Password encrypted using BCrypt
* JWT token-based authentication
* Token expiry handling
* Redis-based OTP expiration
* One-time reset token validation

---

## 📸 Screens (Optional)

* Register Page
* OTP Verification Page
* Login Page
* Forgot Password Page
* Reset Password Page

---

## 👨‍💻 Author

Jagdish Kamlekar

---

## ⭐ Give a Star

If you like this project, give it a ⭐ on GitHub!
