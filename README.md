Full Stack Ecommerce-App: -
# BuySmart---An-E-Commerce-Platform

This is a full-stack E-commerce application that allows users to browse, filter, and purchase products. It is built using the MERN stack (MongoDB, Express, React, Node.js), with payment integration via Braintree.

## Features

- **User Authentication:** Login and register functionalities using JSON Web Tokens (JWT).
- **Product Management:** CRUD operations for products, categories, and orders.
- **Filters:** Filter products by category and price range.
- **Shopping Cart:** Add products to the cart and proceed to checkout.
- **Payment Gateway:** Secure payments using Braintree.
- **Email Notifications:** Send notifications using SendGrid.

## Tech Stack

### Backend (Server-Side)
- **Node.js**
- **Express.js**
- **MongoDB**
- **Mongoose**
- **JWT Authentication**
- **Braintree for Payment Processing**
- **SendGrid for Emailing**

### Frontend (Client-Side)
- **React.js**
- **Ant Design (UI components)**
- **React Router DOM for navigation**
- **Axios for API requests**
- **React Toast for notifications**

## Project Structure

```
.
├── client                   # Frontend (React)
│   ├── public
│   ├── src
│   └── package.json
├── config                   # Configuration files (e.g., database, environment variables)
├── controllers              # Route controllers
├── helpers                  # Utility functions
├── middlewares              # Authentication and other middleware
├── models                   # Mongoose models for MongoDB
├── routes                   # API routes
├── server.js                # Main server file
├── .env                     # Environment variables
└── package.json             # Backend dependencies
```

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Saksham0070/BuySmart---An-E-Commerce-Platform.git
   cd BuySmart---An-E-Commerce-Platform
   ```

2. **Install dependencies:**

   For the server (backend):
   ```bash
   npm install
   ```

   For the client (frontend):
   ```bash
   cd client
   npm install
   ```

3. **Configure environment variables:**

   Create a `.env` file in the root directory and add the following:

   ```env
   PORT=8080
   DEV_MODE=development
   MONGO_URL=your_mongodb_url
   JWT_SECRET=your_jwt_secret
   BRAINTREE_MERCHANT_ID=your_braintree_merchant_id
   BRAINTREE_PUBLIC_KEY=your_braintree_public_key
   BRAINTREE_PRIVATE_KEY=your_braintree_private_key
   ```

4. **Run the application:**

   In the root directory, you can run both the client and server concurrently:
   ```bash
   npm run dev
   ```

   Alternatively, you can start the server and client separately:
   - **Server:** `npm run server`
   - **Client:** `npm run client`

5. **Access the application:**
   - The frontend will be accessible at `http://localhost:3000`
   - The backend API will run on `http://localhost:8080`

## Dependencies

### Backend
- **express:** Web framework for Node.js
- **mongoose:** MongoDB object modeling tool
- **jsonwebtoken:** For token-based authentication
- **bcrypt:** For password hashing
- **dotenv:** Environment variable management
- **nodemon:** Development utility for auto-restarting the server
- **concurrently:** To run both client and server simultaneously
- **braintree:** Payment gateway integration
- **@sendgrid/mail:** Email sending functionality

### Frontend
- **react:** JavaScript library for building user interfaces
- **react-router-dom:** For routing in React
- **axios:** HTTP client for making API requests
- **antd:** Ant Design component library for UI
- **react-toastify & react-hot-toast:** For displaying toast notifications

## Future Enhancements

- **Product Reviews:** Allow users to leave product reviews.
- **Wishlist Feature:** Add products to a wishlist for future purchase.
- **Order Tracking:** Implement order tracking functionality.
- **Admin Dashboard:** A separate dashboard for managing users, products, and orders.
