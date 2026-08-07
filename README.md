# 💬 Chat Application

A modern **real-time chat application** built using the MERN stack with secure authentication, instant messaging, online user status, image sharing, and a responsive user interface.

The application enables users to create accounts, connect with other users, send real-time messages, share images, and manage their profiles with a smooth chat experience.

---

## 🚀 Features

### 🔐 Authentication & User Management

* User registration and login
* Secure password hashing using bcrypt
* JWT-based authentication
* Protected routes and user sessions
* Profile management

### 💬 Real-Time Messaging

* Instant one-to-one messaging using Socket.IO
* Real-time message delivery
* Online/offline user status
* Persistent chat history stored in MongoDB

### 🖼️ Media Sharing

* Image upload support
* Cloud-based image storage using Cloudinary
* Display user profile images

### 🎨 Modern UI Experience

* Responsive design
* Multiple theme support
* Smooth loading skeletons
* Toast notifications
* Clean chat interface

---

# 🛠️ Tech Stack

## Frontend

* React.js
* Vite
* Tailwind CSS
* DaisyUI
* Zustand (State Management)
* Axios
* Socket.IO Client
* React Router
* Lucide React Icons

## Backend

* Node.js
* Express.js
* MongoDB
* Mongoose
* Socket.IO
* JWT Authentication
* bcrypt.js
* Cloudinary

---

# 📂 Project Structure

```
chat-application/

│
├── backend/
│   ├── src/
│   │   ├── controllers/
│   │   │   ├── auth.controller.js
│   │   │   └── message.controller.js
│   │   │
│   │   ├── models/
│   │   │   ├── user.model.js
│   │   │   └── message.model.js
│   │   │
│   │   ├── routes/
│   │   │   ├── auth.route.js
│   │   │   └── message.route.js
│   │   │
│   │   ├── middleware/
│   │   ├── lib/
│   │   └── index.js
│   │
│   └── package.json
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── store/
│   │   ├── lib/
│   │   └── App.jsx
│   │
│   └── package.json
│
└── package.json
```

---

# ⚙️ Installation & Setup

## 1. Clone the Repository

```bash
git clone <repository-url>

cd chat-application
```

---

# Backend Setup

Navigate to backend:

```bash
cd backend
```

Install dependencies:

```bash
npm install
```

Create a `.env` file inside the backend folder:

```
PORT=5000

MONGODB_URI=your_mongodb_connection_string

JWT_SECRET=your_secret_key

CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret

NODE_ENV=development
```

Start backend server:

```bash
npm run dev
```

Backend will run on:

```
http://localhost:5000
```

---

# Frontend Setup

Open another terminal:

```bash
cd frontend
```

Install dependencies:

```bash
npm install
```

Start frontend:

```bash
npm run dev
```

Frontend will run on:

```
http://localhost:5173
```

---

# 🔄 Application Flow

```
User
 |
 | Authentication
 |
JWT Verification
 |
Express Backend
 |
MongoDB Database
 |
Socket.IO Connection
 |
Real-Time Messaging
 |
React UI Update
```

---

# 🔌 API Modules

## Authentication Routes

| Method | Endpoint                   | Description        |
| ------ | -------------------------- | ------------------ |
| POST   | `/api/auth/signup`         | Create new account |
| POST   | `/api/auth/login`          | User login         |
| POST   | `/api/auth/logout`         | Logout user        |
| PUT    | `/api/auth/update-profile` | Update profile     |

---

## Message Routes

| Method | Endpoint                 | Description       |
| ------ | ------------------------ | ----------------- |
| GET    | `/api/messages/users`    | Get users         |
| GET    | `/api/messages/:id`      | Get chat messages |
| POST   | `/api/messages/send/:id` | Send message      |

---


# 🌟 Future Enhancements

* Group chat support
* Video and voice calling
* Message reactions
* Message search
* Push notifications
* End-to-end encryption
* AI chatbot integration

---

# 👨‍💻 Author

**Lathvika Maddi**

B.Tech Computer Science Engineering

---

# ⭐ Support

If you like this project, consider giving it a ⭐ on GitHub.
