# Anjali Clothing E-commerce Website

A full-stack e-commerce application built with React, Node.js, Express, and MongoDB.

## Features

- **Frontend**: React-based user interface with shopping cart, product display, and user authentication
- **Admin Panel**: Product management system for adding and removing products
- **Backend**: RESTful API with user authentication, product management, and cart functionality
- **Database**: MongoDB for storing products, users, and cart data

## Project Structure

```
Full_Stack_Ecommerce/
├── frontend/          # React frontend application
├── admin/            # React admin panel
├── backend/          # Node.js/Express backend API
└── README.md
```

## Prerequisites

- Node.js (v14 or higher)
- MongoDB Atlas account or local MongoDB installation
- npm or yarn package manager

## Installation & Setup

### 1. Clone the repository
```bash
git clone <repository-url>
cd Full_Stack_Ecommerce
```

### 2. Backend Setup
```bash
cd backend
npm install
```

Create a `.env` file in the backend directory:
```env
PORT=4000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_super_secret_jwt_key_here
NODE_ENV=development
```

Start the backend server:
```bash
npm start
```

### 3. Frontend Setup
```bash
cd frontend
npm install
npm start
```

### 4. Admin Panel Setup
```bash
cd admin
npm install
npm start
```

## Environment Variables

Make sure to set up the following environment variables in your `.env` file:

- `PORT`: Server port (default: 4000)
- `MONGODB_URI`: MongoDB connection string
- `JWT_SECRET`: Secret key for JWT token generation
- `NODE_ENV`: Environment (development/production)

## API Endpoints

### Authentication
- `POST /login` - User login
- `POST /signup` - User registration

### Products
- `GET /allproducts` - Get all products
- `GET /newcollections` - Get latest products
- `GET /popularinwomen` - Get popular women's products
- `POST /addproduct` - Add new product (Admin)
- `POST /removeproduct` - Remove product (Admin)

### Cart
- `POST /addtocart` - Add item to cart
- `POST /removefromcart` - Remove item from cart
- `POST /getcart` - Get user's cart

### File Upload
- `POST /upload` - Upload product images

## Security Features

- JWT-based authentication
- Environment variable configuration
- Input validation and error handling
- CORS enabled for cross-origin requests

## Recent Fixes Applied

1. **Database Connection**: Added proper MongoDB connection with error handling
2. **Environment Variables**: Moved sensitive data to environment variables
3. **Error Handling**: Added comprehensive error handling throughout the application
4. **Security**: Updated JWT secret to use environment variables
5. **Routing**: Fixed React Router configuration for proper navigation
6. **Schema Fix**: Corrected typo in Product schema (`avilable` → `available`)
7. **Input Validation**: Added validation for required fields in admin panel

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## License

This project is licensed under the MIT License.
