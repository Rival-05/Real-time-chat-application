# 📡 Real-Time Chat Application

A full-stack real-time chat application built using modern web technologies. It allows users to communicate in real time, using WebSockets for instant message exchange and a clean, responsive UI powered by Tailwind CSS.

---

## 🛠️ Tech Stack

### 🔹 Frontend (`client/`)
- **Next.js (App Router)** – React framework for SSR/SSG and routing
- **Tailwind CSS v4** – Utility-first CSS framework for responsive styling
- **TypeScript** – Type-safe development
- **Prettier** – Code formatting
- **ESLint** – Linting and code quality
- **Socket.IO (Client)** – For connecting to WebSocket server

### 🔹 Backend (`server/`)
- **Node.js + Express** – Backend runtime and framework
- **Socket.IO** – Real-time bidirectional communication
- **MongoDB + Mongoose** – NoSQL database with ORM
- **TypeScript** – For scalable backend logic
- **dotenv** – Environment configuration
- **cors** – Middleware for handling cross-origin requests

---

## 🧱 Project Structure

real-time-chat-app/ <br>
├── client/ # Frontend (Next.js App Router + Tailwind v4)<br>
│ ├── src/<br>
│ │ ├── app/ # Pages and layouts (App Router)<br>
│ │ ├── components/ # Reusable UI elements (ChatBox, Message, Sidebar)<br>
│ │ ├── hooks/ # Custom React hooks (useSocket, useAuth)<br>
│ │ ├── lib/ # Utility functions/helpers<br>
│ │ ├── socket/ # Socket.IO client setup<br>
│ │ ├── styles/ # Tailwind CSS & global styles<br>
│ │ └── types/ # TypeScript types/interfaces<br>
│ ├── tailwind.config.ts # Tailwind CSS configuration<br>
│ ├── next.config.js # Next.js configuration<br>
│ └── .env.local # Frontend environment variables<br>
│<br>
├── server/ # Backend (Express + Socket.IO + MongoDB)<br>
│ ├── config/ # MongoDB connection setup<br>
│ ├── controllers/ # Route logic (message handling, user auth)<br>
│ ├── models/ # Mongoose schemas/models<br>
│ ├── routes/ # API routes (optional)<br>
│ ├── index.ts # Server entry point<br>
│ ├── tsconfig.json # TypeScript config for backend<br>
│ └── .env # Backend environment variables<br>
│<br>
├── .gitignore # Files to exclude from git<br>
├── README.md # Project overview<br>
└── package.json # Project metadata<br>

---

## 📦 Installation & Setup

1. **Clone the repository:**

git clone https://github.com/your-username/real-time-chat-app.git<br>
cd real-time-chat-app

2. **Install frontend and backend dependencies:** 

In both client and server<br>
npm install

3. **Setup environment variables:**

client/.env.local

Paste: <br>
NEXT_PUBLIC_SOCKET_URL=http://localhost:5000

server/.env

Paste: <br>
PORT=5000<br>
MONGO_URI=mongodb://localhost:27017/chatapp

4. **Run the servers:**

In both client and server<br>
npm run dev 

