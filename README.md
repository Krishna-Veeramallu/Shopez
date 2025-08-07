# ShopEZ - Full Stack E-commerce Application

ShopEZ is a full-stack e-commerce web application with a React frontend and a Node.js/Express/MongoDB backend. This project allows users to browse products, manage a cart, place orders, and includes admin features for managing products, users, and orders.

---

## Project Structure


Code/
  client/   # React frontend
  server/   # Node.js/Express backend


---

## Features

### Frontend (client)
- Built with React and Material-UI
- User authentication (register/login)
- Product browsing, search, and filtering
- Shopping cart management
- Order placement and order history
- Admin dashboard for managing products, users, and orders

### Backend (server)
- RESTful API with Express.js
- MongoDB for data storage (via Mongoose)
- JWT-based authentication
- Product, user, order, and banner management
- Image upload support (Multer)

---

## Getting Started

### Prerequisites
- Node.js (v16+ recommended)
- npm
- MongoDB (local or cloud instance)

### 1. Clone the repository
bash
git clone <your-repo-url>
cd Code


### 2. Install dependencies
#### Frontend
bash
cd client
npm install

#### Backend
bash
cd ../server
npm install


### 3. Configure environment variables
- Backend: Create a .env file in server/ (optional, for JWT secret, MongoDB URI, etc.)

### 4. Start the development servers
#### Backend (default: http://localhost:5000)
bash
cd server
node server.js

#### Frontend (default: http://localhost:3000)
bash
cd client
npm start


---

## API Endpoints (Backend)
- POST   /api/auth/register   - Register a new user
- POST   /api/auth/login      - Login and receive JWT
- GET    /api/products        - List/search/filter products
- POST   /api/products        - Add new product (admin)
- PUT    /api/products/:id    - Update product (admin)
- DELETE /api/products/:id    - Delete product (admin)
- POST   /api/orders          - Place an order (user)
- GET    /api/orders          - Get user orders
- GET    /api/users           - List users (admin)
- GET    /api/banner          - Get homepage banners

---

## Technologies Used
- *Frontend:* React, Material-UI, Axios, React Router
- *Backend:* Node.js, Express, MongoDB, Mongoose, JWT, Multer, bcryptjs, dotenv

---

## License
This project is licensed under the MIT License.

---

## Acknowledgements
- [Create React App](https://github.com/facebook/create-react-app)
- [Material-UI](https://mui.com/)
- [Express.js](https://expressjs.com/)
- [MongoDB](https://www.mongodb.com/)
