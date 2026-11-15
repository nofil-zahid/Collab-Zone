# Collab-Zone

A **Kanban‑based project management** web application with **fine‑grained permission controls**. Users can create boards, define columns, move tasks, and set role‑based access (admin, manager, contributor, viewer) per project.

---

## ✨ Features
- **Kanban Boards**: Drag‑and‑drop tasks across customizable columns.
- **Permission System**: Role‑based access control at the project and board level.
- **Real‑time Collaboration**: Powered by WebSockets (or similar) for live updates.
- **RESTful API**: Backend services expose CRUD endpoints for projects, boards, tasks, and permissions.
- **Modular Architecture**: Separate `frontend`, `backend`, and `database` folders for clean development.

---

## 📂 Folder Structure
```
Collab-Zone/
├─ backend/          # Node/Express API server
├─ database/         # DB schema & migration scripts
├─ frontend/         # React (or Vue) UI
├─ README.md         # ↗️ You are reading it right now!
└─ .git/             # Git repository metadata
```

---

## 🚀 Getting Started
1. **Clone the repo**
   ```bash
   git clone <repo-url>
   cd Collab-Zone
   ```
2. **Install dependencies**
   ```bash
   # backend
   cd backend && npm install && cd ..
   # frontend
   cd frontend && npm install && cd ..
   ```
3. **Configure the database**
   - Copy `database/.env.example` to `.env` and set your DB credentials.
   - Run migrations:
     ```bash
     cd database && npm run migrate
     ```
4. **Run the development servers**
   ```bash
   # Terminal 1: backend
   cd backend && npm run dev
   # Terminal 2: frontend
   cd frontend && npm start
   ```
5. Open `http://localhost:3000` (or the port configured in the frontend) in your browser.
