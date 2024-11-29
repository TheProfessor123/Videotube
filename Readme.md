
# Videotube (Backend Development In Progress)

This project is a video-sharing platform designed to enable users to upload, stream, and interact with videos seamlessly. It features robust user authentication using JWT and password encryption for security, RESTful APIs for efficient data handling, and scalable video storage powered by Cloudinary. The platform supports functionalities such as user management, video uploads, likes, comments, and playlists, making it ideal for developers looking for a backend implementation of a modern video-sharing application or learning backend development concepts.


## Environment Variables

To run this project, you will need to add the following environment variables to your .env file

`PORT`

`MONGODB_URI`

`CORS_ORIGIN`

`ACCESS_TOKEN_SECRET`

`ACCESS_TOKEN_EXPIRY`

`REFRESH_TOKEN_SECRET`

`REFRESH_TOKEN_EXPIRY`

`CLOUDINARY_CLOUD_NAME`

`CLOUDINARY_API_KEY`

`CLOUDINARY_API_SECRET`
## Run Locally

Clone the project

```bash
  git clone https://github.com/TheProfessor123/backend.git
```

Go to the project directory

```bash
  cd backend
```

Install dependencies

```bash
  npm install
```

Start the server

```bash
  npm run dev
```


## API Reference

#### Register User

```http
  POST http://localhost:PORT/api/v1/users/register
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `fullName` | `string` | **Required**. Your Full Name |
| `email` | `string` | **Required**. Your Email ID |
| `username` | `string` |**Required**. Your User Name |
| `password` | `string` |**Required**. Your Password |
| `avatar` | `string` | **Required**. Your Avatar Path |
| `coverImage` | `string` | Your Cover Image Path |

#### Login User

```http
  POST http://localhost:PORT/api/v1/users/login
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `username` | `string` |**Required**. Your User Name |
| `email` | `string` | **Required**. Your Email ID |
| `password` | `string` |**Required**. Your Password |

#### Logout User

```http
  POST http://localhost:PORT/api/v1/users/logout
```

Status Code: 200 

Message: "User Logged Out Successfully"

#### Referesh Access Token

```http
  POST http://localhost:PORT/api/v1/users/refresh-token
```

Status Code: 200

Message: "Access Token Refreshed Successfully"
## Features

- Create User, Login and Logout
- Refresh Access Token
- Change Password
- Update User Account Details (Full Name, Email ID, Avatar, Cover Image)


## 🚀 About Author
I'm a passionate Information Technology student at Kalinga Institute of Industrial Technology with a strong interest in software development, machine learning, and backend technologies. Currently pursuing my B.Tech with a CGPA of 8.34, I'm actively expanding my technical skills and building innovative projects.

[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/TheProfessor123)

