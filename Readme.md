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

real-time-chat-app/
├── client/ # Frontend (Next.js App Router + Tailwind v4)
│ ├── src/
│ │ ├── app/ # Pages and layouts (App Router)
│ │ ├── components/ # Reusable UI elements (ChatBox, Message, Sidebar)
│ │ ├── hooks/ # Custom React hooks (useSocket, useAuth)
│ │ ├── lib/ # Utility functions/helpers
│ │ ├── socket/ # Socket.IO client setup
│ │ ├── styles/ # Tailwind CSS & global styles
│ │ └── types/ # TypeScript types/interfaces
│ ├── tailwind.config.ts # Tailwind CSS configuration
│ ├── next.config.js # Next.js configuration
│ └── .env.local # Frontend environment variables
│
├── server/ # Backend (Express + Socket.IO + MongoDB)
│ ├── config/ # MongoDB connection setup
│ ├── controllers/ # Route logic (message handling, user auth)
│ ├── models/ # Mongoose schemas/models
│ ├── routes/ # API routes (optional)
│ ├── index.ts # Server entry point
│ ├── tsconfig.json # TypeScript config for backend
│ └── .env # Backend environment variables
│
├── .gitignore # Files to exclude from git
├── README.md # Project overview
└── package.json # Project metadata

---

## 📦 Installation & Setup

1. **Clone the repository:**

git clone https://github.com/your-username/real-time-chat-app.git
cd real-time-chat-app

2. **Install frontend and backend dependencies:**

In both client and server
npm install

3. **Setup environment variables:**

client/.env.local

Paste: 
NEXT_PUBLIC_SOCKET_URL=http://localhost:5000

server/.env

Paste: 
PORT=5000
MONGO_URI=mongodb://localhost:27017/chatapp

4. **Run the servers:**

In both client and server
npm run dev 

