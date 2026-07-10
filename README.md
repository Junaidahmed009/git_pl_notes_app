# Notes App Frontend

This is the **Notes App** built with **React**, **Vite**, and **Tailwind CSS**.  
It connects to a **Node.js + Express** backend that handles saving, fetching, updating, and deleting personal notes.

i updated the code of both frontend and backend now this app can run locallly easily and fixed some bugs.
because the frontend is running on
axios.get("https://notes-app-ftxv.onrender.com/api/notes")
and backend is running on 
https://notes-app-chi-khaki.vercel.app
---

## 📦 Installation Guide

Follow the steps below to set up and run both the backend and frontend locally.

---

## 🖥️ 1. Clone the Repository

```bash
git clone 

cd notes_app
```

## 🧩 2. Install and Run Backend of notes app

📁 Navigate to the backend folder and start the server:

```bash
cd notes-app/backend
npm install
node index.js
```

- The backend will start on `http://localhost:3001/api/notes`
-if you see [] your backend is working fine.

- Make sure it's running before starting the frontend

## 🌐 3. Install and Run Frontend of notes app

📁 In a new terminal, navigate to the frontend folder:

```bash
cd notes-app/frontend
npm install
npm run dev
```

- The frontend will run on `http://localhost:5173`

- It communicates with the backend for full CRUD functionality

## ✅ That’s it!

Your Notes App is now running locally 🎉

- Frontend: `http://localhost:5173`

- Backend: `http://localhost:3001`

--- 

Make sure both servers are running in separate terminals. Enjoy coding!

# GitHub Actions CI Pipeline
#
# This pipeline activates whenever code is pushed to the main
# branch or a pull request is opened on notes-app.
#
# The pipeline performs the following tasks:
<!-- creates ubuntu server -->

# 1. Checks out the latest source code from the repository.
# 2. Sets up the mentioned Node.js environment.
# 3. Installs backend project dependencies.
# 4. Installs frontend project dependencies.
# 5. Runs code quality checks (ESLint).
# 6. Builds the React (Vite) frontend to verify that it compiles successfully.
# 7. Starts the backend server to ensure it launches without runtime errors.
#
# If any step fails, the workflow stops immediately and reports the failure,
# preventing broken code from being merged or deployed.
# -----------------------------------------------------------------------------