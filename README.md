# Backend Developer Assignment – Node.js + Express REST API

This project is a RESTful API built with Node.js and Express. It supports user registration and login (without authentication), and full CRUD operations for a Product model using MongoDB.

---

## Table of Contents

- [Features](#features)
- [Tech Stack](#tech-stack)
- [Folder Structure](#folder-structure)
- [Getting Started](#getting-started)
- [API Endpoints](#api-endpoints)
- [Environment Variables](#environment-variables)


---

## Features

- User registration and login routes (no authentication required)
- CRUD operations for Product (name, price, quantity)
- MongoDB integration via Mongoose

---

## Tech Stack

- Node.js
- Express.js
- MongoDB (Mongoose)
- dotenv

---

## Folder Structure


---

## Getting Started

1. **Clone the repository or unzip the folder**

2. **Install dependencies**
npm install

3. **Set up environment variables**
- Create a `.env` file in the root directory.
- Add your MongoDB connection string:
  ```
  MONGODB_URI=your_mongodb_connection_string
  PORT=5000
  ```

4. **Start the server**
npm start

The server will run on `http://localhost:5000` by default.

---

## API Endpoints

### User Routes

- **POST /api/auth/register**
- Register a new user  
 **Body:**  
 ```
 {
   "username": "string",
   "password": "string"
 }
 ```

- **POST /api/auth/login**
- Login user (no authentication required)  
 **Body:**  
 ```
 {
   "username": "string",
   "password": "string"
 }
 ```

### Product Routes

- **GET /api/products**
- Get all products

- **GET /api/products/:id**
- Get product by ID

- **POST /api/products**
- Create a new product  
 **Body:**  
 ```
 {
   "name": "string",
   "price": number,
   "quantity": number
 }
 ```

- **PUT /api/products/:id**
- Update a product by ID  
 **Body:**  
 ```
 {
   "name": "string",
   "price": number,
   "quantity": number
 }
 ```

- **DELETE /api/products/:id**
- Delete a product by ID

---

## Environment Variables

- `MONGODB_URI` – MongoDB connection string
- `PORT` – (optional) Port number (default: 5000)

---
