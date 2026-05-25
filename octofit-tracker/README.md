# 🐙 OctoFit Tracker

A modern multi-tier fitness tracking application built with **React 19**, **Express**, **TypeScript**, and **MongoDB**.

## 🏗️ Architecture

### Frontend
- **Framework**: React 19
- **Build Tool**: Vite
- **Port**: 5173
- **Location**: `octofit-tracker/frontend/`

### Backend
- **Runtime**: Node.js
- **Framework**: Express
- **Language**: TypeScript
- **Port**: 8000
- **Location**: `octofit-tracker/backend/`
- **Database**: MongoDB (Mongoose ODM)

### Database
- **System**: MongoDB
- **Port**: 27017
- **Database Name**: `octofit-tracker`

## 📋 Project Structure

```
octofit-tracker/
├── frontend/
│   ├── src/
│   │   ├── App.jsx           (Main React component)
│   │   ├── App.css           (Component styling)
│   │   ├── main.jsx          (React entry point)
│   │   └── index.css         (Global styles)
│   ├── index.html            (HTML entry)
│   ├── package.json          (Dependencies)
│   ├── vite.config.js        (Vite configuration)
│   └── .gitignore
├── backend/
│   ├── src/
│   │   └── index.ts          (Express server)
│   ├── package.json          (Dependencies)
│   ├── tsconfig.json         (TypeScript configuration)
│   ├── .env.example          (Environment template)
│   └── .gitignore
└── README.md
```

## 🚀 Quick Start

### Prerequisites
- Node.js 18+ installed
- MongoDB 5.0+ installed or Docker
- npm or yarn package manager

### Step 1: Start MongoDB

```bash
# Using Docker (recommended)
docker run -d -p 27017:27017 --name octofit-mongodb mongo:latest

# Or locally if installed
mongod
```

### Step 2: Setup Backend

```bash
cd octofit-tracker/backend

# Copy environment file
cp .env.example .env

# Install dependencies
npm install

# Start backend server
npm run dev
```

Backend will be available at: **http://localhost:8000**

### Step 3: Setup Frontend

```bash
cd octofit-tracker/frontend

# Install dependencies
npm install

# Start frontend dev server
npm run dev
```

Frontend will be available at: **http://localhost:5173**

## ✅ Verify Setup

### Test Backend Health Check

```bash
curl http://localhost:8000/api/health
```

Expected response:
```json
{
  "status": "OK",
  "message": "OctoFit Tracker Backend is running",
  "timestamp": "2025-05-25T12:00:00.000Z"
}
```

### Check Backend Root Endpoint

```bash
curl http://localhost:8000
```

Expected response:
```json
{
  "message": "Welcome to OctoFit Tracker API",
  "version": "1.0.0",
  "endpoints": {
    "health": "/api/health"
  }
}
```

## 📦 Available Scripts

### Frontend Scripts
```bash
npm run dev       # Start Vite dev server (port 5173)
npm run build     # Build for production
npm run preview   # Preview production build
```

### Backend Scripts
```bash
npm run dev       # Start backend with ts-node (port 8000)
npm run build     # Compile TypeScript to JavaScript
npm start         # Run compiled backend
npm run watch     # Watch for TypeScript changes
```

## 🔧 Environment Variables

### Backend (.env)
```
MONGODB_URI=mongodb://localhost:27017/octofit-tracker
PORT=8000
NODE_ENV=development
```

## 📚 Technology Stack

| Layer | Technology |
|-------|-----------|
| Frontend | React 19, Vite, CSS3 |
| Backend | Express, TypeScript, Node.js |
| Database | MongoDB, Mongoose |
| Port Allocation | Frontend: 5173, Backend: 8000, MongoDB: 27017 |

## 🎯 Next Steps

- [ ] Create Mongoose schemas and models
- [ ] Build REST API endpoints
- [ ] Setup frontend API client
- [ ] Implement authentication
- [ ] Add unit tests
- [ ] Setup CI/CD pipeline
- [ ] Deploy to production

## 📝 Notes

- Hot module reloading enabled in both frontend and backend
- TypeScript strict mode enabled for type safety
- CORS configured for frontend-backend communication
- Environment variables required for backend configuration

## 🤝 Contributing

Feel free to submit issues and enhancement requests.

## 📄 License

MIT

---

**Branch**: `octofit-tracker/setup`  
**Created**: 2025-05-25  
**Status**: ✅ Initialized and Ready for Development
