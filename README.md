# 🎧 Spotify – Spotify-Inspired Music Application.

It is a full-featured, Spotify-inspired music streaming application built using a **microservice architecture**. It includes two backend services (`user-service` and `admin-service`) and a modern React frontend. The system uses **Redis** caching for high performance and faster response times.

---

## ✨ Features

### 🎧 User Functionality
- 🔊 Listen to music online
- 📁 Create and manage personal playlists
- ❤️ save favorite tracks
- 🧠 Fast loading via Redis caching

### 🛠️ Admin Functionality
- ➕ Add new songs (audio file, image, metadata)
- ✏️ Edit/update song information
- 🗑️ Delete songs from the library
- 🔐 Protected admin access (role-based)

---

## 🧰 Tech Stack

| Layer        | Tech                                 |
|--------------|--------------------------------------|
| Frontend     | React.js, TypeScript, Tailwind CSS   |
| Backend      | Node.js, Express.js (Microservices)  |
| API Gateway  | (Optional) Express Gateway/Nginx     |
| Database     | PostgreSQL, MongoDB.                 |
| Media        | Cloudinary                           |
| Caching      | Redis                                |
| ORM          | Prisma                               |
| Auth         | JWT                                  |

---

## 📦 Services Overview

### `user-service`
- Handles music streaming, playlist management, and user authentication.
- Caches frequently accessed data with Redis.

### `admin-service`
- Manages CRUD operations for songs.
- Only accessible to admin users.

### `client`
- Built using React + TailwindCSS.
- Communicates with both backend services via REST APIs.

---

Spotify/
├── user-service/         # Backend service for users/music/playlists
├── admin-service/        # Backend service for admin CRUD
├── client/               # React frontend
├── .gitignore          
├── README.md

complete code is pushed in this repo: https://github.com/souvikjs01/spotify

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/spotlite-microservices.git
cd spotlite-microservices


