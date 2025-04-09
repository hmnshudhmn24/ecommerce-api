# E-Commerce API

## Features

- User Authentication (Register/Login)
- Product Catalog Management
- Shopping Cart System
- Checkout and Stripe Payment Integration

## Tech Stack

- **Backend:** Node.js, Express
- **Database:** MongoDB
- **Authentication:** JWT
- **Payments:** Stripe

## Getting Started

### Prerequisites

- Node.js
- MongoDB or MongoDB Atlas
- Stripe account

### Installation

```bash
git clone https://github.com/yourusername/ecommerce-api.git
cd ecommerce-api
npm install
```

### Environment Variables

Create a `.env` file in the root directory and add:

```
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
STRIPE_SECRET_KEY=your_stripe_secret_key
```

### Running the Server

```bash
npm start
```

## API Endpoints

### Auth
- `POST /api/auth/register`
- `POST /api/auth/login`

### Products
- `GET /api/products`
- `POST /api/products` (admin)

### Cart
- `GET /api/cart`
- `POST /api/cart`

### Checkout
- `POST /api/checkout`

## License

This project is licensed under the MIT License.