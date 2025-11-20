# 🌐 BKIT — Slack Clone (Chat + Video Calling Platform)

<p align="center">
A modern, scalable Slack-style communication platform offering real-time chat, file sharing, direct messaging, channels, video calling, and powerful collaboration tools — built for teams, organizations, and communities.
</p>

<p align="center">
<img src="https://cdn-icons-png.flaticon.com/512/906/906349.png" width="120"/>
</p>

---

## 🚀 Overview

The **BKIT Slack Clone** is a full-scale communication system designed to mirror (and enhance) the core capabilities of platforms like Slack or Microsoft Teams. It supports both **real-time messaging** and **video conferencing**, backed by robust authentication, file sharing, and async background job processing.

Designed with modern engineering principles, it provides a smooth, secure and scalable experience suitable for:

- Tech teams  
- Educational institutions  
- Remote offices  
- Community groups  
- Enterprise internal communication networks  

---

## ✨ Platform Highlights

### 💬 Real-Time Messaging  
- Websocket-powered updates  
- Threads, replies, reactions  
- Read receipts  
- Typing indicators  
- Fully persistent chat history  

### 📂 File Sharing  
Upload & preview:  
- Images, PDFs, ZIPs  
- Videos  
- Documents  

Built-in security validation ensures only safe uploads.

### 📊 Polling System  
- Multiple selection  
- Anonymous voting  
- Real-time result updates  
- Comments inside polls  

### 👤 User Authentication (Clerk)  
- OAuth login  
- Multi-device sessions  
- Secure token validation  
- Profile & avatar sync  

### 🚪 Direct Messaging + Channels  
- Private DMs  
- Public & private channels  
- Role-based access  
- Team grouping  

### 🎥 Video Calling (Stream)  
- Group & 1:1 calls  
- Screen sharing  
- Emoji reactions  
- Grid/tiled view  
- Call logs  

### ⚙ Background Jobs (Inngest)  
Handles:  
- Event triggers  
- Notifications  
- Audit logs  
- Async cleanup  

### 🛡 Error Monitoring (Sentry)  
- API failure logging  
- Frontend error capture  
- Real-time crash alerts  

### 🤖 AI-Assisted Code Reviews (CodeRabbit)  
Ensures consistent high-quality pull requests.

---

## 🏗 Tech Stack

### Frontend  
- React + Vite  
- TailwindCSS  
- Stream Video SDK  
- Clerk Auth  
- Sentry SDK  

### Backend  
- Node.js  
- Express  
- MongoDB  
- Stream Chat/Video server SDK  
- Inngest  

### Deployment  
- Fully environment-based  
- Supports cloud hosting  
- Secure API key injection  

---

# 🔧 Environment Configuration

Below structure is based directly on your `.env` requirement references.

---

## 🌐 Backend (`/backend`)

Create `.env`:

```
PORT=5001
MONGO_URI=your_mongo_uri_here

NODE_ENV=development

CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key_here
CLERK_SECRET_KEY=your_clerk_secret_key_here

STREAM_API_KEY=your_stream_api_key_here
STREAM_API_SECRET=your_stream_api_secret_here

SENTRY_DSN=your_sentry_dsn_here

INNGEST_EVENT_KEY=your_inngest_event_key_here
INNGEST_SIGNING_KEY=your_inngest_signing_key_here

CLIENT_URL=http://localhost:5173
```

---

## 💻 Frontend (`/frontend`)

Create `.env`:

```
VITE_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key_here
VITE_STREAM_API_KEY=your_stream_api_key_here
VITE_SENTRY_DSN=your_sentry_dsn_here
VITE_API_BASE_URL=http://localhost:5001/api
```

---

# ▶️ Running the Application

### Start Backend
```bash
cd backend
npm install
npm run dev
```

### Start Frontend
```bash
cd frontend
npm install
npm run dev
```

Access the app at:
```
Frontend: http://localhost:5173
Backend API: http://localhost:5001
```

---

# 👥 Team — BKIT

<p align="center">
<b>BKIT</b> — Delivering modern, reliable and scalable software ecosystems for the next generation of digital collaboration.
</p>
