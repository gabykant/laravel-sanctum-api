# Laravel Sanctum Authentication API

A secure and scalable REST API built with **Laravel** and **Laravel Sanctum**, designed for modern web and mobile applications.

This project demonstrates best practices for API authentication, user management, and password security in a real-world Laravel backend.

---

## 🚀 Features

-   User registration with extended profile information
-   Secure login & logout using Laravel Sanctum
-   Token-based authentication for APIs
-   Password reset (forgot & reset password)
-   Change password for authenticated users
-   Role-based access (`user`, `admin`)
-   Protected API routes
-   Swagger (OpenAPI) documentation

---

## 🛠 Tech Stack

-   **Laravel 10 / 11**
-   **PHP 8+**
-   **Laravel Sanctum**
-   **MySQL / PostgreSQL**
-   **Swagger (L5-Swagger)**
-   RESTful API architecture

---

## 📌 API Endpoints

### Authentication

POST /api/register
POST /api/login
POST /api/logout
GET /api/user

### Password Management

POST /api/forgot-password
POST /api/reset-password
POST /api/change-password

## 🔐 Authentication

This API uses **Laravel Sanctum** for secure token-based authentication.

After login, include the token in the request header:
Authorization: Bearer YOUR_ACCESS_TOKEN

## 📖 API Documentation (Swagger)

Swagger UI is available at:
http://localhost:8050/api/documentation

Use the **Authorize** button to test secured endpoints.

---

## ⚙️ Installation & Setup

### 1. Clone the repository

```bash
git clone https://github.com/your-username/laravel-auth-api-sanctum.git
cd laravel-auth-api-sanctum

### 2. Install dependencies
composer install

### 3. Environment configuration
cp .env.example .env
php artisan key:generate

Update database credentials in .env.

### 4. Run migrations & seeders
php artisan migrate --seed

### 5. Run the server
php artisan serve --port=8050

Application URL:
http://localhost:8050

📬 Mail Configuration (Password Reset)

For local testing, emails are logged:

MAIL_MAILER=log

You can use MailJet, SMTP, or any email provider for production.

👨‍💻 Author

Gabriel Kwaye
Senior Laravel Developer – APIs & Authentication
GitHub: https://github.com/your-username
Email: g.kwaye@ksoft-solutions.com
Upwork: https://www.upwork.com/freelancers/~01b294ea71fb12952f

📄 License

This project is open-source and available under the MIT License
```
