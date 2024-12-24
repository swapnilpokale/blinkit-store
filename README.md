# Blinkit Store

## Overview
A feature-rich, fully responsive e-commerce web application inspired by Blinkit. The project includes mobile and admin panel interfaces, offering seamless user and admin experiences. It is built using the MERN stack and focuses on secure authentication, efficient database management, and a smooth user experience.

---

## Features

### User Features
- **Responsive Design:** Works on desktop, mobile, and admin interfaces.
- **Secure Authentication:** JWT-based authentication with refresh and access tokens.
- **Profile Management:** Includes login, registration, profile editing, and password reset options.

### Product and Category Management
- **Product Display:** Features multiple products with banners and categorized sections.
- **Subcategories:** Dedicated pages for subcategories with product image slides.

### Admin Features
- **Admin Dashboard:** Manage products, users, and roles.
- **Role Management:** Define user roles and statuses (active/inactive/suspended).
- **Detailed User Management:** Manage additional fields like address, city, and state.

---

## Technical Implementation

### Backend Setup
- **Environment Management:** Utilized `.env` files for secure environment variable handling.
- **Database:** Connected to MongoDB with schemas for users, products, and subcategories.
- **API Endpoints:** Built with Node.js and Express for modularity and scalability.
- **Controllers:** Modularized controllers for handling routes like user registration, login, and email verification.

### Database Configuration
- **Schemas:** Included fields like email, last login, address, and discount.
- **Indexes:** Implemented compound indexes for faster query performance.
- **Relationships:** Connected schemas using `ref` and `populate` for relational data management.

### Authentication and Validation
- **Email Verification:** Templates for account verification with email uniqueness checks.
- **Validation:** Server-side validation for duplicate emails, password confirmation, and proper error handling.
- **Secure Passwords:** Encrypted storage for passwords and secure verification processes.

### Error Handling
- **Try-Catch Blocks:** Ensured error handling with clear success/error responses.
- **API Responses:** Comprehensive feedback for user actions like login and registration.

---

## Installation

### Prerequisites
- Node.js
- MongoDB
- VS Code (or any IDE)

### Steps to Run Locally
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/blinkit-clone.git
   ```

2. Navigate to the project directory:
   ```bash
   cd blinkit-clone
   ```

3. Install dependencies:
   ```bash
   npm install
   ```

4. Set up environment variables:
   - Create a `.env` file in the root directory.
   - Add the following:
     ```env
     PORT=5000
     MONGO_URI=your_mongodb_connection_string
     JWT_SECRET=your_jwt_secret
     ```

5. Start the development server:
   ```bash
   npm run dev
   ```

6. Open the application in your browser at `http://localhost:5000`.

---

## Folder Structure
- **/controllers**: Modular controllers for users, products, etc.
- **/models**: MongoDB schemas for database entities.
- **/routes**: API route definitions.
- **/middleware**: Authentication and error-handling middleware.
- **/config**: Configuration files, including database connection.

---

## Technologies Used
- **Frontend:** React.js
- **Backend:** Node.js, Express.js
- **Database:** MongoDB
- **Authentication:** JWT (JSON Web Tokens)
- **Environment Management:** dotenv

