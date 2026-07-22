# ⚛️ LinkPulse Frontend

Frontend application for LinkPulse.

Built using **React**, **Vite**, **TanStack Router**, **TanStack Query**, **Redux Toolkit**, and **Tailwind CSS**.

---

# Tech Stack

- React
- Vite
- TanStack Router
- TanStack Query
- Redux Toolkit
- Tailwind CSS
- Axios

---

# Installation

Install dependencies

```bash
npm install
```

---

# Run the Application

Development

```bash
npm run dev
```

Build

```bash
npm run build
```

Preview

```bash
npm run preview
```

---

# Docker

Build

```bash
docker build -f ../docker/frontend/Dockerfile -t linkpulse-frontend .
```

Run

```bash
docker run -p 5173:5173 linkpulse-frontend
```

---

# Features

- User Authentication
- Dashboard
- URL Shortener
- Click Tracking
- Responsive UI
- Protected Routes
- TanStack Router
- TanStack Query

---

# Folder Structure

```text
Frontend/
│
├── src/
├── components/
├── pages/
├── routing/
├── hooks/
├── api/
├── store/
├── utils/
├── package.json
└── vite.config.js
```

---

# Upcoming Features

- QR Code Generation
- URL Expiration
- Better Analytics Dashboard
- Search
- Pagination
- Dark Mode
- Redis-powered Optimizations
- CI/CD Integration
- AWS Deployment

---

# Notes

Currently, the frontend does not require any environment variables. If backend URLs or third-party integrations are introduced later, a `.env` file will be added using Vite's `VITE_*` convention.