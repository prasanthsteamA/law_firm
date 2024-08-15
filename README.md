Full Stack Authentication Application
Overview
This project is a full-stack authentication application built with React (frontend) and Node.js (backend). It features user registration, login, password reset, and token-based authentication, along with an admin kickout function.

Features
User registration with email or phone number.
User login with token-based authentication.
Password reset via a one-time link.
Dashboard with welcome message.
Admin kickout functionality.
Rate limiting and account locking.
Folder Structure



```
backend/
│
├── config/
│   ├── db.js               # Database configuration and connection
│   └── rateLimiter.js      # Rate limiting middleware
│
├── controllers/
│   ├── authController.js   # Authentication-related logic
│
├── models/
│   ├── User.js             # User model schema
│
├── routes/
│   └── authRoutes.js       # API routes for authentication
│
├── services/
│   └── authService.js      # Authentication service logic
│
├── middleware/
│   ├── authMiddleware.js   # Authentication and authorization middleware
│
├── .env                    # Environment variables
├── server.js               # Main server entry point
├── package.json            # Node.js dependencies and scripts
└── README.md               # Instructions and documentation
```
Frontend
```
frontend/
│
├── public/
│   ├── index.html          # Main HTML file
│
├── src/
│   ├── components/
│   │   ├── Login.js        # Login component
│   │   ├── Register.js     # Register component
│   │   ├── ResetPassword.js# Reset Password component
│   │   ├── Dashboard.js    # Dashboard component
│   │
│   ├── services/
│   │   └── authService.js  # API calls to the backend
│   │
│   ├── App.js              # Main React app entry
│   ├── index.js            # ReactDOM entry point
│   ├── styles.css          # Basic styling for the application
│
├── package.json            # React dependencies and scripts
└── README.md               # Instructions and documentation
```
