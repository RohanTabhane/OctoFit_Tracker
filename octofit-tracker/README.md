# OctoFit Tracker

A social fitness app designed to help students stay active and compete with their peers.

## Project Structure

```
octofit-tracker/
├── frontend/          # React 19 + Vite application (Port 5173)
└── backend/           # Node.js + Express + TypeScript API (Port 8000)
```

## Prerequisites

- Node.js (v18+ recommended)
- npm or yarn
- MongoDB (v6+ recommended, running on port 27017)

## Getting Started

### Backend Setup

1. Navigate to the backend directory:
   ```bash
   cd octofit-tracker/backend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create a `.env` file based on `.env.example`:
   ```bash
   cp .env.example .env
   ```

4. Start the backend server:
   ```bash
   npm run dev
   ```

   The backend will run on `http://localhost:8000`

### Frontend Setup

1. Navigate to the frontend directory:
   ```bash
   cd octofit-tracker/frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm run dev
   ```

   The frontend will run on `http://localhost:5173`

## Configuration

### Ports
- **Frontend**: 5173
- **Backend**: 8000
- **MongoDB**: 27017

### Environment Variables

Create a `.env` file in the backend directory with the following:

```
PORT=8000
MONGODB_URI=mongodb://localhost:27017/octofit_tracker
FRONTEND_URL=http://localhost:5173
```

## Available Scripts

### Backend
- `npm run dev` - Start development server with hot reload
- `npm run build` - Build TypeScript to JavaScript
- `npm start` - Run production build

### Frontend
- `npm run dev` - Start Vite development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build

## Technology Stack

### Frontend
- React 19
- Vite
- TypeScript

### Backend
- Node.js
- Express.js
- TypeScript
- Mongoose (MongoDB ODM)
- CORS

## API Endpoints

- `GET /api/health` - Health check endpoint

## Development

To work on both frontend and backend simultaneously, open two terminal windows:

**Terminal 1 (Backend):**
```bash
cd octofit-tracker/backend
npm run dev
```

**Terminal 2 (Frontend):**
```bash
cd octofit-tracker/frontend
npm run dev
```

Then open your browser and navigate to `http://localhost:5173`
