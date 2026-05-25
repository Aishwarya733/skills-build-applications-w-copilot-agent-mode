# 🐙 OctoFit Tracker

A modern multi-tier fitness tracking application built with GitHub Copilot Agent Mode.

## Architecture

```
OctoFit Tracker
├── Frontend (React 19 + Vite)
│   └── Port: 5173
├── Backend (Express + TypeScript)
│   └── Port: 8000
└── Database (MongoDB)
    └── Port: 27017
```

## Prerequisites

- Node.js 18+
- MongoDB running locally or connection string
- npm or yarn

## Getting Started

### Frontend Setup

```bash
cd octofit-tracker/frontend
npm install
npm run dev
```

The frontend will be available at `http://localhost:5173`

### Backend Setup

```bash
cd octofit-tracker/backend
npm install
npm run dev
```

The backend API will be available at `http://localhost:8000`

### MongoDB

Ensure MongoDB is running on `mongodb://localhost:27017`

Or update the `MONGODB_URI` in `backend/.env` with your connection string.

## Available Scripts

### Frontend
- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint

### Backend
- `npm run dev` - Start development server with ts-node
- `npm run build` - Compile TypeScript to JavaScript
- `npm start` - Run compiled JavaScript
- `npm run lint` - Run ESLint

## API Endpoints

- `GET /api/health` - Health check
- `GET /api/ping` - Ping endpoint

## Project Structure

```
octofit-tracker/
├── frontend/
│   ├── src/
│   │   ├── App.jsx
│   │   ├── main.jsx
│   │   └── index.css
│   ├── vite.config.js
│   ├── index.html
│   └── package.json
├── backend/
│   ├── src/
│   │   └── server.ts
│   ├── tsconfig.json
│   ├── .env
│   └── package.json
└── README.md
```

## Technologies

- **Frontend**: React 19, Vite, JavaScript/JSX
- **Backend**: Express, TypeScript, Node.js
- **Database**: MongoDB, Mongoose
- **Tools**: CORS, dotenv

## Next Steps

1. ✅ Project structure initialized
2. ⏭️ Create data models (User, Workout, Progress)
3. ⏭️ Build API endpoints
4. ⏭️ Connect frontend to backend
5. ⏭️ Add authentication

---

Built with 💪 and 🐙
