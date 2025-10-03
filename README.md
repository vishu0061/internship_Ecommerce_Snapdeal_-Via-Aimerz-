# 🛒 Orebi Shopping - Full Stack E-commerce Platform

A complete, production-ready e-commerce solution built with modern technologies including React.js, Node.js, Express, MongoDB, Redux Toolkit, Tailwind CSS, and Stripe payment integration.

![Orebi Shopping Platform](./public/thumbnail.png)

## 🌟 Features

### Customer Features

- **Product Catalog**: Browse products with advanced filtering and search
- **Shopping Cart**: Add/remove items with real-time updates
- **User Authentication**: Secure login/register system
- **Order Management**: Place orders, track order history
- **Payment Integration**: Secure Stripe payment processing
- **Responsive Design**: Works perfectly on all devices
- **FAQ Section**: Comprehensive help section
- **Blog Page**: Coming soon functionality

### Admin Features

- **Dashboard Analytics**: Sales metrics and business insights
- **Product Management**: Add, edit, delete products with image upload
- **Order Management**: View and manage customer orders
- **User Management**: Manage customer accounts
- **Brand & Category Management**: Organize products efficiently
- **Contact Management**: Handle customer inquiries
- **Inventory Tracking**: Real-time stock management
- **Refresh Functionality**: One-click data refresh across all pages

### Technical Features

- **Database Migration**: Complete export/import system for MongoDB
- **Environment Configuration**: Separate development/production configs
- **CORS Policy**: Production-ready cross-origin resource sharing
- **Order Count Badges**: Real-time order notifications
- **Custom Skeleton Loading**: Smooth loading experiences
- **React Icons**: Modern icon system
- **Redux State Management**: Centralized state management

## 🏗️ Architecture

This is a full-stack application with three main components:

```
📁 Project Structure
├── 📁 client/          # React.js Frontend (Customer)
├── 📁 admin/           # React.js Admin Panel
├── 📁 server/          # Node.js Backend API
└── 📄 README.md        # This file
```

## 🚀 Quick Start Guide

### 1. Project Setup

After purchasing and downloading the code:

```bash
# Extract the downloaded ZIP file
# Navigate to the project directory
cd orebishopping-vitejs

# Install dependencies for all components
# For Server
cd server
npm install

# For Client
cd ../client
npm install

# For Admin
cd ../admin
npm install
```

### 2. Environment Variables Setup

You'll need to create environment files for each component. **These are not included for security reasons.**


#### 🎨 Client Environment Variables

Create `client/.env` file:

```env
VITE_SERVER_URL=http://localhost:8000
VITE_STRIPE_PUBLISHABLE_KEY=pk_test_your_stripe_publishable_key
VITE_PAYPAL_CLIENT_ID=your_paypal_client_id
```

#### 👨‍💼 Admin Environment Variables

Create `admin/.env` file:

```env
VITE_SERVER_URL=http://localhost:8000
```

### 3. Getting Your Credentials

#### MongoDB Atlas Setup

1. Go to [MongoDB Atlas](https://www.mongodb.com/cloud/atlas)
2. Create a free account
3. Create a new cluster
4. Go to Database Access → Add Database User
5. Go to Network Access → Add IP Address (0.0.0.0/0 for development)
6. Go to Database → Connect → Connect your application
7. Copy the connection string and replace `<password>` with your database user password

#### Cloudinary Setup

1. Sign up at [Cloudinary](https://cloudinary.com/)
2. Go to Dashboard
3. Copy your Cloud Name, API Key, and API Secret

### 4. Database Setup

Initialize your database with sample data:

```bash
cd server

# Create admin user (optional)
npm run create-admin

# Seed database with sample data (optional)
npm run seed
```

### 5. Running the Application

Start all three components in different terminals:

```bash
# Terminal 1 - Start Backend Server
cd server
npm run dev
# Server runs on http://localhost:8000

# Terminal 2 - Start Client (Customer Frontend)
cd client
npm run dev
# Client runs on http://localhost:5173

# Terminal 3 - Start Admin Panel
cd admin
npm run dev
# Admin runs on http://localhost:5174
```















