# RBAC
VRV Security’s Backend Developer Intern Assignment
# Role-Based Access Control (RBAC) System

This is a Node.js and Express.js project that implements Role-Based Access Control (RBAC). It includes user authentication, role management, and secure API endpoints for managing user roles and permissions.

---

## Features

- **User Authentication**: 
  - Register and login functionality with hashed passwords.
- **Protected Routes**: 
  - Only authenticated users can access specific routes.
- **Role-Based Access Control**:
  - Users have roles like Admin, Moderator, or User.
  - Access is controlled based on roles.
- **Role Management**: 
  - Admin can update user roles.

---

## Technologies Used

- Node.js
- Express.js
- MongoDB (Mongoose)
- JWT (JSON Web Tokens) for authentication
- bcrypt for password hashing
- dotenv for environment variable management

---

## Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-folder>

2. Install dependencies:
   
    npm install
   
4. Create a .env file in the root directory and add the following variables:

    PORT=5000
    MONGO_URI=<Your MongoDB Connection String>
    JWT_SECRET=<Your JWT Secret>
    
4.Start the server:

    npm start
API Endpoints
Authentication
Register
POST /api/users/register
Body:

{
  "username": "testuser",
  "email": "test@example.com",
  "password": "password123",
  "role": "User"
}



