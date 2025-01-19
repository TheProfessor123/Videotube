# Videotube Backend

A robust backend implementation for a video-sharing platform built with Node.js, Express, and MongoDB. The platform provides comprehensive user management, secure authentication, and video handling capabilities.

## 🚀 Features

- **User Management**
  - Registration with avatar and cover image upload
  - Login with username/email
  - Password encryption using bcrypt
  - Profile management and updates
  - Watch history tracking

- **Authentication & Security**
  - JWT-based authentication
  - Access and refresh token mechanism
  - Secure cookie handling
  - Protected routes with middleware

- **File Handling**
  - Image upload support (avatar, cover image)
  - Cloudinary integration for media storage
  - Multer middleware for file uploads
  - Temporary file cleanup

- **API Features**
  - RESTful architecture
  - Error handling with custom ApiError class
  - Standardized responses with ApiResponse
  - Async operation handling
  - MongoDB aggregation pipelines

## 🛠️ Tech Stack

- Node.js
- Express.js
- MongoDB with Mongoose
- JWT for authentication
- Cloudinary for media storage
- Multer for file uploads
- CORS enabled
- Cookie Parser

## 📊 API Endpoints

### User Management
```http
POST /api/v1/users/register
POST /api/v1/users/login
POST /api/v1/users/logout
POST /api/v1/users/refresh-token
```

### Profile Management
```http
POST /api/v1/users/change-password
GET /api/v1/users/current-user
PATCH /api/v1/users/update-account
PATCH /api/v1/users/avatar
PATCH /api/v1/users/cover-image
```

### Channel & History
```http
GET /api/v1/users/c/:username
GET /api/v1/users/history
```

## 🚀 Getting Started

1. Clone the repository:
```bash
git clone https://github.com/TheProfessor123/Videotube.git
```

2. Install dependencies:
```bash
cd Videotube
npm install
```

3. Set up environment variables in `.env`:
```env
PORT=8000
MONGODB_URI=your_mongodb_uri
CORS_ORIGIN=your_frontend_origin
ACCESS_TOKEN_SECRET=your_access_token_secret
ACCESS_TOKEN_EXPIRY=1d
REFRESH_TOKEN_SECRET=your_refresh_token_secret
REFRESH_TOKEN_EXPIRY=10d
CLOUDINARY_CLOUD_NAME=your_cloudinary_name
CLOUDINARY_API_KEY=your_cloudinary_key
CLOUDINARY_API_SECRET=your_cloudinary_secret
```

4. Start the development server:
```bash
npm run dev
```

## 📝 Project Structure

```
src/
├── app.js          # Express app setup
├── constants.js    # Global constants
├── controllers/    # Request handlers
├── db/            # Database connection
├── middlewares/   # Custom middlewares
├── models/        # Mongoose models
├── routes/        # API routes
└── utils/         # Helper functions
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 👤 Author

**Chhagan Ram Choudhary**
- Student at Kalinga Institute of Industrial Technology
- CGPA: 8.38
- Passionate about software development and backend technologies

[![GitHub](https://img.shields.io/badge/GitHub-TheProfessor123-black?style=for-the-badge&logo=github)](https://github.com/TheProfessor123)
