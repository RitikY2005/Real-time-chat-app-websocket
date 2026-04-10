# Pinge - Real time chat app 

[![Live Site](https://img.shields.io/badge/Live-Demo-brightgreen?style=for-the-badge)](https://real-time-chat-app-websocket.onrender.com)

A modern, real-time messaging platform built to provide seamless instant communication with a responsive user interface.

---

## Overview

[Pinge](https://real-time-chat-app-websocket.onrender.com) is a full-stack chat application using WebSockets for instantaneous data transfer. Unlike traditional apps that require page refreshes, Pinge enables users to communicate in real-time, see online/offline statuses, and manage conversations effortlessly within a secure MERN environment.

---

---

## Screenshots

![Screenshot 3](https://lh3.googleusercontent.com/u/0/d/1SONhhpOKINQqCHUkNqJmIz3QzB203jEt)

![Screenshot 2](https://lh3.googleusercontent.com/u/0/d/1HuyCu278NM9f1uMp_CUJsbEygUmHjcQV)




---



## Features

### Authentication & Authorization
* **JWT-Based Auth:** Secure user sessions using JSON Web Tokens.
* **Route Protection:** Middleware-protected routes only visible to authenticated users 
* **Data Privacy:** Encrypted password hashing using bcrypt.

### Real-Time Messaging
* **WebSockets:** Powered by Socket.io for instant message delivery and receipt.
* **Presence Indicators:** Real-time online/offline status tracking for all users.
* **Typing Indicators:** Visual cues when a contact is actively typing.

### UI/UX & Design
* **Responsive Design:** Fully optimized for mobile, tablet, and desktop using Tailwind CSS.
* **Dynamic Sidebar:** Easily search for users and navigate between different conversations.
* **Smooth Transitions:** Loading states and skeleton screens for a premium feel.


---

## Tech Stack

| Component | Technology |
| :--- | :--- |
| **Frontend** | React.js, Tailwind CSS, Shadcn ui |
| **Backend** | Node.js, Express.js, Socket.io |
| **Database** | MongoDB, Mongoose |
| **State Management** | Zustand  |
| **Security** | JWT, Bcrypt |

---

## Project Structure

```text
Pinge/
├── frontend/   # React.js frontend
└── backend/   # Node.js backend

```

---

---

## Installation and Setup
> [!NOTE]
> KEEP the .env file in the root folder

Frontend Setup

```
cd frontend
npm install
npm run dev
```
Frontend env variables -
```
VITE_BACKEND_URL=
VITE_NODE_ENV="production" | "development"

```
Backend Setup

```
cd backend
npm install
npm run dev
```

Backend env variables -
```
FRONTEND_URL=
PORT=
CLOUDINARY_CLOUD_NAME=
CLOUDINARY_API_KEY=
CLOUDINARY_API_SECRET=
MONGODB_URI=
NODE_ENV="production" | "development"
JWT_SECRET=
JWT_EXPIRY=in milliseconds

```
---
## API Endpoints

### Authentication & user
* `POST /api/v1/users/register` - Register a new user
* `POST   /api/v1/users/login` - User login
* `GET /api/v1/users/logout` - logout user
* `POST /api/v1/users/upload-avatar` - Upload user avatar
* `POST /api/v1/users/update-profile` - update user profile

### Discover
* `GET /api/v1/contacts/:searchTerm` - Fetch all users on platform
* `GET /api/v1/contacts/my-contacts` - fetch all my contacts
* `GET /api/v1/contacts/all-users` - fetch all users to add in a channel

### Messages
* `POST /api/v1/messages/upload-file` - upload the file to be shared in chat
* `POST /api/v1/messages/dm-chat-history` - fetch chat history of an authenticated user

### Channel
* `POST /api/v1/channels/create-channel` - Create a channel \(group chat\)
* `GET /api/v1/channels/my-channels` - fetch current users channels 
* `POST /api/v1/channels/channel-chat-history` - getch chat history of a channel 



---



