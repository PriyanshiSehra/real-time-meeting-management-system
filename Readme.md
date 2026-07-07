# MCMS – Meeting & Communication Management System

A modern meeting and collaboration platform that combines real-time video conferencing, intelligent scheduling, agenda management, and productivity analytics into a single application.

> 🚀 This repository is under active development. New features, UI improvements, and performance optimizations are being added continuously.

---

## ✨ Features

### 🎥 Real-Time Video Conferencing
- WebRTC powered peer-to-peer video and audio calls
- Screen sharing support
- Camera & microphone controls
- Audio-only fallback mode
- STUN/TURN server support

### 📅 Smart Meeting Management
- Create, edit and schedule meetings
- Online, Offline & Hybrid meeting modes
- Automatic meeting lifecycle management
- Auto-generated meeting links
- Natural language scheduling using **chrono-node**

### 📝 Agenda & Notes
- Create meeting agendas
- Allocate time for each agenda item
- Real-time agenda synchronization
- Track progress during meetings

### 📊 Productivity Dashboard
- Meeting attendance statistics
- Weekly activity heatmap
- Speaking time analytics
- Task completion tracking
- Meeting streaks & achievements
- AI-inspired productivity insights

### 🔐 Secure Authentication
- JWT Authentication
- Protected API routes
- Secure password hashing using bcrypt
- Persistent login sessions

### ⚡ Productivity Shortcuts
Built-in keyboard shortcuts for faster navigation and meeting controls.

---

# 🛠 Tech Stack

| Layer | Technologies |
|--------|--------------|
| Frontend | React 19, Vite, TypeScript |
| Backend | Node.js, Express 5 |
| Database | MongoDB (Mongoose) |
| Real-Time | Socket.io |
| Video | WebRTC |
| Authentication | JWT, bcryptjs |
| Scheduling | chrono-node |
| Utilities | Nodemailer |

---

# 📁 Project Structure

```
client/
│── src/
│   ├── components/
│   ├── context/
│   ├── hooks/
│   ├── pages/
│   └── App.tsx

server/
│── middleware/
│── models/
│── routes/
│── services/
│── index.ts

ai-service/

README.md
```

---

# 🚀 Getting Started

## Clone Repository

```bash
git clone https://github.com/PriyanshiSehra/SWE_meeting_and_communication_platform.git
cd SWE_meeting_and_communication_platform
```

---

## Backend Setup

```bash
cd server
npm install
npm run dev
```

---

## Frontend Setup

```bash
cd client
npm install
npm run dev
```

---

## Environment Variables

### Server

```env
PORT=5000
MONGO_URI=mongodb://127.0.0.1:27017/mcms_db
JWT_SECRET=your_secret_key
```

### Client

```env
VITE_API_URL=http://localhost:5000/api
```

---

# 📡 REST API

### Authentication

- POST `/api/auth/signup`
- POST `/api/auth/login`
- GET `/api/auth/me`
- GET `/api/auth/verify`

### Meetings

- GET `/api/meetings`
- POST `/api/meetings`
- PUT `/api/meetings/:id`
- DELETE `/api/meetings/:id`

### Agenda

- GET `/api/agenda/:meetingId`
- POST `/api/agenda/:meetingId`
- PUT `/api/agenda/:meetingId/item/:itemId`

---

# 🔌 Socket Events

### Client → Server

- join_room
- leave_room
- signal
- start_transcription
- stop_transcription

### Server → Client

- room_peers
- peer_joined
- peer_left
- signal
- transcription_started
- transcription_stopped

---

# 📌 Future Enhancements

- AI meeting summaries
- Live speech transcription
- Calendar integrations
- Meeting recordings
- File sharing
- Whiteboard collaboration
- Performance optimizations
- Mobile responsiveness improvements

---

# 🤝 Contributing

Contributions, suggestions and feature requests are welcome.

If you'd like to contribute:

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Open a Pull Request

---

## 📄 License

This project is intended for educational and development purposes.

---
