# E-Commerce API

A scalable and secure RESTful API for an E-Commerce platform built with Node.js, Express, and MongoDB. It includes features such as user authentication, product management, cart functionality, order processing, and Stripe-based payments.

---

## Features

- User registration and login with JWT authentication
- Secure password hashing using bcrypt
- CRUD operations for products (admin only)
- Shopping cart with item management
- Checkout process with Stripe payment integration
- Order creation and history tracking
- Middleware for route protection and error handling

---

## Technologies Used

- **Backend:** Node.js, Express.js
- **Database:** MongoDB with Mongoose ODM
- **Authentication:** JWT (JSON Web Tokens), bcrypt
- **Payments:** Stripe API
- **Environment Variables:** dotenv

---

## Getting Started

### Prerequisites

Make sure you have the following installed:

- Node.js (v14+)
- MongoDB (local or Atlas)
- Stripe account (for secret keys)

---

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/ecommerce-api.git
cd ecommerce-api

