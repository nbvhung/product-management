# 🛒 Full-Stack E-Commerce Platform

A production-ready e-commerce platform built from scratch with separate **Customer** and **Admin** portals, powered by Server-Side Rendering.

---

## 🚀 Live Demo

> _Add your deployed URL here (e.g. Vercel, Railway...)_

---

## ✨ Features

### 👤 Customer Portal
- Register / Login with secure authentication
- OTP email verification for password recovery
- Browse products by category with search & filter
- Shopping cart with real-time quantity updates
- Checkout and order placement

### 🛠️ Admin Portal
- Dashboard with statistics (products, accounts, categories, users)
- Full CRUD for products, categories, and accounts
- Dynamic Role-Based Access Control (RBAC) — permissions configurable per role
- Cloud image upload via Cloudinary
- Rich-text product descriptions with TinyMCE
- Server-side pagination, sorting, and filtering

### 💬 Real-Time Features (Socket.IO)
- Live 1-on-1 and group chat rooms
- Typing indicator and online/offline presence
- Instant friend request system

---

## 🧱 Tech Stack

| Layer | Technology |
|---|---|
| Runtime | Node.js |
| Framework | Express.js |
| Template Engine | Pug (SSR) |
| Database | MongoDB + Mongoose |
| Real-time | Socket.IO |
| File Upload | Cloudinary + Multer |
| Auth | Cookie-based token + MD5 |
| Email | Nodemailer |
| UI | Bootstrap 4 |

---

## 📁 Project Structure

```
├── controllers/
│   ├── admin/          # Admin portal controllers
│   └── client/         # Customer portal controllers
├── models/             # Mongoose schemas
├── routes/
│   ├── admin/          # Admin routes
│   └── client/         # Client routes
├── views/
│   ├── admin/          # Admin Pug templates
│   └── client/         # Client Pug templates
├── middlewares/        # Auth, upload, cart middleware
├── socket/             # Socket.IO event handlers
├── helpers/            # Utility functions
├── validates/          # Request validation
├── public/             # Static assets (CSS, JS)
└── index.js            # Entry point
```

---

## ⚙️ Getting Started

### Prerequisites
- Node.js >= 16
- MongoDB Atlas account
- Cloudinary account

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/nbvhung/product-management
cd product-management

# 2. Install dependencies
npm install

# 3. Create environment file
cp .env.example .env
```

### Environment Variables

Create a `.env` file in the root directory:

```env
PORT=3000

# Tạo tại: https://www.mongodb.com/atlas
MONGO_URL=your_mongodb_connection_string

# Tạo tại: https://cloudinary.com
CLOUD_NAME=your_cloudinary_cloud_name
CLOUD_KEY=your_cloudinary_api_key
CLOUD_SECRET=your_cloudinary_api_secret

EMAIL_USER=your_gmail_address
EMAIL_PASS=your_gmail_app_password
```

### Run the app

```bash
# Development
npm start

# The app will be running at http://localhost:3000
```

---

## 📄 License

This project is for educational and portfolio purposes.
