# E-Commerce API

A scalable and secure RESTful API for an E-Commerce platform built with Node.js, Express, and MongoDB. It includes features such as user authentication, product management, cart functionality, order processing, and Stripe-based payments.

## Features

- User registration and login with JWT authentication  
- Secure password hashing using bcrypt  
- CRUD operations for products (admin only)  
- Shopping cart with item management  
- Checkout process with Stripe payment integration  
- Order creation and history tracking  
- Middleware for route protection and error handling  

## Technologies Used

- Backend: Node.js, Express.js  
- Database: MongoDB with Mongoose ODM  
- Authentication: JWT (JSON Web Tokens), bcrypt  
- Payments: Stripe API  
- Environment Configuration: dotenv  

## Getting Started

### Prerequisites

Make sure you have the following installed:

- Node.js (v14 or newer)  
- MongoDB (local or MongoDB Atlas)  
- Stripe account (to obtain secret keys)

### Installation

1. Clone the repository:

   git clone https://github.com/yourusername/ecommerce-api.git  
   cd ecommerce-api

2. Install dependencies:

   npm install

3. Create a `.env` file in the root directory and configure your environment variables:

   PORT=5000  
   MONGO_URI=your_mongodb_connection_string  
   JWT_SECRET=your_jwt_secret_key  
   STRIPE_SECRET_KEY=your_stripe_secret_key

4. Start the development server:

   npm run dev

## API Endpoints

### Authentication

- POST /api/auth/register – Register a new user  
- POST /api/auth/login – Login user and receive JWT  

### Products

- GET /api/products – Get all products  
- POST /api/products – Create a new product (admin only)  
- PUT /api/products/:id – Update a product (admin only)  
- DELETE /api/products/:id – Delete a product (admin only)  

### Cart

- POST /api/cart – Create a cart  
- PUT /api/cart/:id – Update cart items  
- GET /api/cart/:userId – Get user's cart  

### Orders

- POST /api/orders – Create a new order  
- GET /api/orders/:userId – Get user's order history  

### Payments

- POST /api/checkout/payment – Stripe checkout session
