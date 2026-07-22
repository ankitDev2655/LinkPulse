# 🚀 LinkPulse

> A production-ready URL Shortener built with the MERN ecosystem, featuring JWT authentication, Docker support, analytics-ready architecture, and a scalable backend.

---

## 📌 Project Status

> 🚧 **This project is under active development.**

The core application is functional, and additional production-grade features are being added continuously.

---

## ✨ Features

- 🔗 URL Shortening
- 👤 JWT Authentication
- 📊 Dashboard
- 📈 Click Tracking
- 🐳 Docker Support
- ⚛️ React + Vite Frontend
- 🚀 Express.js Backend
- 🍃 MongoDB Atlas
- ⚡ TanStack Router
- 🔄 TanStack Query
- 🎨 Tailwind CSS

---

## 🛣️ Roadmap

### ✅ Completed

- [x] User Authentication (JWT)
- [x] URL Shortening
- [x] Dashboard
- [x] Click Tracking
- [x] Docker Development Setup
- [x] MongoDB Atlas Integration

### 🚧 Upcoming

- [ ] QR Code Generation
- [ ] URL Expiration
- [ ] Redis Caching
- [ ] Rate Limiting
- [ ] AWS Deployment
- [ ] CI/CD Pipeline
- [ ] Analytics Dashboard
- [ ] Custom URL Alias
- [ ] Search & Pagination

---

## 🛠 Tech Stack

### Frontend

- React 19
- Vite
- TanStack Router
- TanStack Query
- Redux Toolkit
- Tailwind CSS
- Axios

### Backend

- Node.js
- Express.js
- MongoDB Atlas
- Mongoose
- JWT
- bcryptjs
- NanoID

### DevOps

- Docker
- Docker Compose

---

## 📁 Project Structure

```text
Link-Pulse/
│
├── Backend/
├── Frontend/
├── docker/
│   ├── backend/
│   ├── frontend/
│   ├── compose/
│   ├── nginx/
│   └── scripts/
│
├── README.md
└── .gitignore
```

---

## 🚀 Getting Started

Clone the repository

```bash
git clone <repository-url>
cd Link-Pulse
```

---

### Backend Setup

```bash
cd Backend
npm install
```

Create a `.env` file.

```env
MONGO_URI=
APP_URL=
JWT_SECRET=
```

Start the backend

```bash
npm run dev
```

---

### Frontend Setup

```bash
cd Frontend
npm install
npm run dev
```

---

## 🐳 Run with Docker

From the project root

```bash
docker compose -f docker/compose/docker-compose.dev.yml up --build
```

Stop containers

```bash
docker compose -f docker/compose/docker-compose.dev.yml down
```

---

## 📚 API Documentation

### Authentication

| Method | Endpoint | Description |
|---------|----------|-------------|
| POST | `/api/auth/register` | Register User |
| POST | `/api/auth/login` | Login User |
| POST | `/api/auth/logout` | Logout User |

### URL

| Method | Endpoint | Description |
|---------|----------|-------------|
| POST | `/api/create` | Create Short URL |
| GET | `/:shortCode` | Redirect to Original URL |
| GET | `/api/url` | Get User URLs |
| DELETE | `/api/url/:id` | Delete URL |

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome.

Feel free to fork the repository and submit a pull request.

---

## 📄 License

This project is licensed under the MIT License.