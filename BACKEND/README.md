# 🚀 LinkPulse Backend

Backend service for the LinkPulse URL Shortener.

Built with **Node.js**, **Express.js**, **MongoDB Atlas**, and **JWT Authentication**.

---

# Tech Stack

- Node.js
- Express.js
- MongoDB Atlas
- Mongoose
- JWT
- bcryptjs
- NanoID
- Docker

---

# Installation

Install dependencies

```bash
npm install
```

---

# Environment Variables

Create a `.env` file in the project root.

```env
MONGO_URI=mongodb+srv://<username>:<password>@cluster.mongodb.net/url-shortner

APP_URL=http://localhost:3000/

JWT_SECRET=your-secret-key
```

---

# Run the Server

Development

```bash
npm run dev
```

Production

```bash
npm start
```

---

# Docker

Build

```bash
docker build -f ../docker/backend/Dockerfile -t linkpulse-backend .
```

Run

```bash
docker run -p 3000:3000 --env-file .env linkpulse-backend
```

---

# API Documentation

## Authentication

### Register

```http
POST /api/auth/register
```

### Login

```http
POST /api/auth/login
```

### Logout

```http
POST /api/auth/logout
```

---

## URL

### Create Short URL

```http
POST /api/create
```

### Redirect

```http
GET /:shortCode
```

### Get User URLs

```http
GET /api/url
```

### Delete URL

```http
DELETE /api/url/:id
```

---

# Folder Structure

```text
Backend/
│
├── src/
├── package.json
├── app.js
└── .env
```

---

# Upcoming Features

- QR Code Generation
- URL Expiration
- Redis Caching
- Rate Limiting
- AWS Deployment
- CI/CD Pipeline
- Analytics
- Unit Testing