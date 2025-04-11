# 🛒 E-Commerce API

A scalable and secure RESTful API for an E-Commerce platform built with **Node.js**, **Express**, and **MongoDB**. This API supports user authentication, product management, shopping cart functionality, order processing, and Stripe-based payment integration.

---

## 🚀 Features

- ✅ User registration and login with JWT authentication  
- 🔒 Secure password hashing using bcrypt  
- 🛍️ Product CRUD operations (Admin only)  
- 🛒 Cart functionality with item management  
- 💳 Stripe payment integration  
- 📦 Order creation and history tracking  
- 🛡️ Middleware for route protection and error handling  

---

## 🛠️ Tech Stack

- **Backend:** Node.js, Express.js  
- **Database:** MongoDB with Mongoose  
- **Authentication:** JWT, bcrypt  
- **Payments:** Stripe API  
- **Environment Config:** dotenv  

---

## 📦 Installation

### ⚙️ Prerequisites

- Node.js v14+  
- MongoDB (local or Atlas)  
- Stripe account

### 🧰 Setup

1. **Clone the repository:**  
   ```bash
   git clone https://github.com/yourusername/ecommerce-api.git
   cd ecommerce-api
   ```

2. **Install dependencies:**  
   ```bash
   npm install
   ```

3. **Create a `.env` file** in the root directory and add the following:

   ```env
   PORT=5000
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret_key
   STRIPE_SECRET_KEY=your_stripe_secret_key
   ```

4. **Run the server in development mode:**  
   ```bash
   npm run dev
   ```

---

## 📡 API Endpoints

### 🔐 Authentication

| Method | Endpoint              | Description             |
|--------|-----------------------|-------------------------|
| POST   | `/api/auth/register`  | Register a new user     |
| POST   | `/api/auth/login`     | Login and get JWT       |

### 📦 Products (Admin Only)

| Method | Endpoint               | Description            |
|--------|------------------------|------------------------|
| GET    | `/api/products`        | Get all products       |
| POST   | `/api/products`        | Create a product       |
| PUT    | `/api/products/:id`    | Update a product       |
| DELETE | `/api/products/:id`    | Delete a product       |

### 🛒 Cart

| Method | Endpoint               | Description            |
|--------|------------------------|------------------------|
| POST   | `/api/cart`            | Create a cart          |
| PUT    | `/api/cart/:id`        | Update cart items      |
| GET    | `/api/cart/:userId`    | Get user's cart        |

### 📦 Orders

| Method | Endpoint               | Description            |
|--------|------------------------|------------------------|
| POST   | `/api/orders`          | Create a new order     |
| GET    | `/api/orders/:userId`  | Get user's order history |

### 💳 Payments

| Method | Endpoint               | Description            |
|--------|------------------------|------------------------|
| POST   | `/api/checkout/payment`| Create Stripe session  |

---

## 📁 Folder Structure

```
ecommerce-api/
├── config/           # Database & Stripe setup
├── controllers/      # Route logic
├── middlewares/      # Auth and error handling
├── models/           # Mongoose schemas
├── routes/           # API route handlers
├── utils/            # Utility functions
├── .env              # Environment variables
├── server.js         # Entry point
└── README.md
```

---

## 📄 License

This project is licensed under the **MIT License**.
