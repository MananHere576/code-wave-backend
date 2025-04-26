# ⚡ CodeWave - Real-time Collaborative Code Editor

CodeWave is a web-based real-time code collaboration platform where multiple users can join a room and edit code together live, powered by **React**, **Express**, **Socket.IO**, and **Render** hosting.

---

### 🚀 Features

- Real-time collaborative editing using Socket.IO
- Unique Room ID generation and sharing
- Instant code synchronization between clients
- Join/Leave notifications
- Clean and responsive frontend built with React

---

### 📦 Project Structure

/ ├── public/ ├── src/ │ ├── components/ │ ├── pages/ │ ├── Actions.js <-- Socket action types │ └── App.js ├── server.js <-- Backend Express server ├── package.json └── README.md

yaml
Copy
Edit

---

### 🛠️ Local Setup (Frontend + Backend)

#### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/code-wave.git
cd code-wave
2. Install Dependencies
bash
Copy
Edit
npm install
3. Setup Environment Variables
Create a .env file in the root folder:

env
Copy
Edit
REACT_APP_BACKEND_URL = http://localhost:5000
4. Start the Backend Server
bash
Copy
Edit
npm run server:dev
5. Start the Frontend
bash
Copy
Edit
npm run start:front
🌍 Deployment
Backend Deployment (Render)
Create a new Web Service on Render.

Connect your backend repository.

Set:

Start Command: node server.js

Build Command: (leave empty)

Expose the correct port (process.env.PORT is auto handled).

After deployment, copy your Render backend URL.

Frontend Deployment (Vercel)
Create a project on Vercel.

Connect your frontend repository.

In Project Settings → Environment Variables, add:

env
Copy
Edit
REACT_APP_BACKEND_URL = https://your-backend-url.onrender.com
Redeploy the frontend.

🧩 Tech Stack
Frontend: React, React Router, CodeMirror

Backend: Node.js, Express.js, Socket.IO

Hosting: Vercel (Frontend) + Render (Backend)

🙌 Acknowledgements
Inspired by real-time editors like Replit, Google Docs, and others.

🔥 Made with passion by Manan Mishra
