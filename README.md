

```md
# 🎬 MagicStream

> A fast, scalable backend for a modern movie streaming platform built with Go and MongoDB.

MagicStream is a backend service designed to power a smooth, high-performance media streaming experience. It manages movies and APIs with a clean, modular architecture built for scalability, maintainability, and real-world usage.

---

## ⚡ Features

- 🎥 Full Movie CRUD system (Create, Read, Update, Delete)
- 🔐 Auth-ready API structure (JWT-ready design)
- 🗄️ MongoDB integration for flexible data storage
- 🌐 RESTful APIs for web/mobile frontend integration
- 🧩 Clean, modular Go architecture (Gin framework)
- 🚀 Scalable and production-ready structure
- 🔒 CORS enabled for frontend communication

---

## 🏗️ Tech Stack

- **Language:** Go (Golang)
- **Framework:** Gin
- **Database:** MongoDB (Atlas / Local)
- **Architecture:** REST API (Modular design)
- **Tools:** dotenv, CORS middleware

---

## 📁 Project Structure

```

MagicStream/
│
├── Server/
│   └── MagicStreamServer/
│       ├── main.go
│       ├── database/
│       ├── routes/
│       ├── controllers/
│       ├── models/
│       ├── middleware/
│       └── config/
│
├── go.mod
├── go.sum
└── README.md

````

---

##  Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/hosama-adem/MagicStream.git
cd MagicStream
````

### 2. Install dependencies

```bash
go mod tidy
```

### 3. Setup environment variables

Create a `.env` file inside `Server/MagicStreamServer/`:

```env
PORT=8080
MONGO_URI=your_mongodb_connection_string
DB_NAME=magicstream
```

---

### 4. Run the server

```bash
go run Server/MagicStreamServer/main.go
```

---

## 📡 API Endpoints

### Health Check

```
GET /api/health
```

### Movies

```
GET    /api/movies
POST   /api/movies
GET    /api/movies/:id
PUT    /api/movies/:id
DELETE /api/movies/:id
```

### Authentication (if enabled)

```
POST /api/auth/register
POST /api/auth/login
```

---

## 🧠 Architecture Overview

Client (Web / Mobile)
↓
REST API (Gin Server)
↓
Controllers Layer
↓
Database Layer (MongoDB)

---

## 🔮 Future Improvements

* JWT Authentication system
* Video streaming (HLS/DASH support)
* Redis caching for performance optimization
* Admin dashboard APIs
* Microservices architecture upgrade
* CI/CD pipeline integration

---

## 🤝 Author

**Hosama Adem**

Backend-focused software engineer passionate about scalable systems, clean architecture, and real-world engineering solutions.

---

## ⭐ Support

If you like this project, consider giving it a ⭐ on GitHub.

```

