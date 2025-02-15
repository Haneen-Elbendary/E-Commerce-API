
---

# 🛒 E-Commerce-API

The **E-Commerce-API** is a robust backend system designed to power an e-commerce platform. It includes features such as user authentication, product management, order processing, wishlists, and more. The project is built using **MongoDB**, **Express**, and **TypeScript**, ensuring scalability and maintainability.

---

## ✨ Features

- **👤 User Management**: Register, login, update user details, and manage user roles.
- **📦 Product Management**: Add, update, delete, and retrieve products with images.
- **❤️ Wishlist**: Users can add/remove products to/from their wishlist.
- **🛒 Shopping Cart**: Add/remove products, update quantities, and apply coupons.
- **📝 Order Management**: Create, pay, and track orders.
- **⭐ Reviews & Ratings**: Users can leave reviews and ratings for products.
- **🎟️ Coupons**: Create and manage discount coupons.
- **🏠 Address Management**: Users can manage their shipping addresses.
- **📂 Categories & Subcategories**: Organize products into categories and subcategories.

---

## 🛠️ Technologies Used

- **Backend Framework**: Express.js
- **Database**: MongoDB
- **Programming Language**: TypeScript
- **Authentication**: JWT (JSON Web Tokens)
- **Validation**: Custom validators for request data
- **Image Upload**: Multer for handling product images

---

## 🚀 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Haneen-Elbendary/E-Commerce-API.git
   cd E-Commerce-API
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Set up environment variables:
   Create a `.env` file in the root directory and add the following variables:
   ```env
   PORT=3000
   MONGODB_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret_key
   ```

4. Run the project:
   ```bash
   npm start
   ```

---

## 🌐 API Routes

### 🔐 Authentication
- **POST** `/api/v1/auth/signup` - User registration
- **POST** `/api/v1/auth/login` - User login
- **POST** `/api/v1/auth/forgetPassword` - Request password reset
- **POST** `/api/v1/auth/verifyCode` - Verify reset code
- **PUT** `/api/v1/auth/resetCode` - Reset password

### 👤 Users
- **GET** `/api/v1/users/me` - Get logged-in user details
- **PUT** `/api/v1/users/updateMe` - Update logged-in user details
- **PUT** `/api/v1/users/changeMyPassword` - Change logged-in user password
- **DELETE** `/api/v1/users/deleteMe` - Delete logged-in user account

### 📦 Products
- **GET** `/api/v1/products` - Get all products
- **POST** `/api/v1/products` - Create a new product
- **GET** `/api/v1/products/:id` - Get a specific product
- **PUT** `/api/v1/products/:id` - Update a product
- **DELETE** `/api/v1/products/:id` - Delete a product

### ❤️ Wishlist
- **GET** `/api/v1/wishlist` - Get user wishlist
- **POST** `/api/v1/wishlist` - Add product to wishlist
- **DELETE** `/api/v1/wishlist/:productId` - Remove product from wishlist

### 🛒 Cart
- **GET** `/api/v1/carts` - Get user cart
- **POST** `/api/v1/carts` - Add product to cart
- **PUT** `/api/v1/carts/applyCoupon` - Apply coupon to cart
- **PUT** `/api/v1/carts/:itemId` - Update product quantity in cart
- **DELETE** `/api/v1/carts/:itemId` - Remove product from cart

### 📝 Orders
- **GET** `/api/v1/orders` - Get all orders
- **POST** `/api/v1/orders` - Create a new order
- **GET** `/api/v1/orders/:id` - Get a specific order
- **PUT** `/api/v1/orders/:id/paid` - Mark order as paid
- **PUT** `/api/v1/orders/:id/delivered` - Mark order as delivered

### 📂 Categories & Subcategories
- **GET** `/api/v1/categories` - Get all categories
- **POST** `/api/v1/categories` - Create a new category
- **GET** `/api/v1/categories/:id` - Get a specific category
- **PUT** `/api/v1/categories/:id` - Update a category
- **DELETE** `/api/v1/categories/:id` - Delete a category

### ⭐ Reviews
- **GET** `/api/v1/reviews` - Get all reviews
- **POST** `/api/v1/reviews` - Create a new review
- **PUT** `/api/v1/reviews/:id` - Update a review
- **DELETE** `/api/v1/reviews/:id` - Delete a review

### 🎟️ Coupons
- **GET** `/api/v1/coupons` - Get all coupons
- **POST** `/api/v1/coupons` - Create a new coupon
- **PUT** `/api/v1/coupons/:id` - Update a coupon
- **DELETE** `/api/v1/coupons/:id` - Delete a coupon

### 🏠 Address
- **GET** `/api/v1/address` - Get user addresses
- **POST** `/api/v1/address` - Add a new address
- **DELETE** `/api/v1/address/:addressId` - Delete an address

---

## 🗂️ Project Structure

Here’s an overview of the project structure:

```
E-Commerce-API/
├── config/               # Configuration files
├── controllers/          # Route controllers
├── interfaces/           # TypeScript interfaces
├── locales/              # Localization files
├── middlewares/          # Custom middlewares
├── models/               # Database models
├── routes/               # API route definitions
├── source/               # Source files
├── utils/                # Utility functions and helpers
├── .gitignore            # Git ignore file
├── README.md             # Project documentation
├── app.ts                # Main application file
├── env.d.ts              # Environment type definitions
├── package-lock.json     # NPM package lock file
├── package.json          # NPM dependencies and scripts
└── tsconfig.json         # TypeScript configuration
```

---

## 🏃‍♂️ How to Run the Project

1. Ensure MongoDB is installed and running.
2. Clone the repository and install dependencies as described above.
3. Start the server:
   ```bash
   npm start
   ```
4. Use tools like **Postman** or **Insomnia** to test the API endpoints.

---

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bugfix.
3. Commit your changes with clear and descriptive messages.
4. Push your branch and submit a pull request.

---

## 📜 License

This project is protected under **Copyright © Haneen Elbendary**. All rights reserved.

---
