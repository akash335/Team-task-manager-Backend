# ⚙️ Team Task Manager — Backend (Express + PostgreSQL)

A secure and scalable **REST API backend** for Team Task Manager, built with **Node.js, Express, and PostgreSQL**, deployed on **Render**.  
Handles authentication, task CRUD operations, and integrates with the React frontend hosted on **Vercel**.

---

## 🧩 Tech Stack
- **Runtime:** Node.js (v22+)
- **Framework:** Express.js  
- **Database:** PostgreSQL (Render / Supabase)  
- **Auth:** JWT (jsonwebtoken) + bcryptjs  
- **Hosting:** Render  
- **ORM:** Native SQL via `pg`  

---

## 🚀 Features
- 🔐 User Authentication (Register / Login via JWT)
- 🗂️ Create, read, update, and delete tasks
- ✅ Mark tasks as **completed** or **pending**
- 👥 Tasks linked to individual user accounts
- 🌐 CORS support for secure frontend integration
- 🪶 PostgreSQL schema auto-initialization
- 🧩 API routes for health, auth, and tasks

---

## 🧪 Local Setup

1. **Clone this repo**
   ```bash
   git clone https://github.com/akash335/Team-task-manager-Backend.git
   cd team-task-manager-backend

2. **Install dependencies**

   npm install


3. Create .env file

PORT=3000
JWT_SECRET=your-secret-key
DATABASE_URL=postgresql://user:password@host:port/dbname
CORS_ORIGIN=http://localhost:5173,https://your-frontend.vercel.app


4. Run locally

npm run dev


5. Visit API health check

http://localhost:3000/health

## Environment Variables
Variable	     Description
--------       -----------
PORT	         Port for local development
JWT_SECRET	   Secret key for JWT signing
DATABASE_URL	 PostgreSQL connection string
CORS_ORIGIN	   Allowed frontend origins (comma-separated)
HOST	         Host address (default: 0.0.0.0)

## Folder Structure
team-task-manager-backend/
├── server.js
├── package.json
├── .env.example
├── .gitignore
├── README.md
└── team.db (if using SQLite locally)

## Deployment on Render

1. Push your code to GitHub:

git add .
git commit -m "Deploy ready"
git push origin main

2. Go to Render
 → Create New Web Service

3. connect your GitHub repo

4. Set these environment variables in Render dashboard:
   PORT=10000
   JWT_SECRET=your-production-secret
   DATABASE_URL=your-render-postgres-url
   CORS_ORIGIN=https://team-task-manager-frontend.vercel.app

5. Build Command:

npm install


6. Start Command:

npm run start


7. Deploy 🎉

🔗 Frontend Repo

Frontend source: https://team-task-manager-frontend.vercel.app/

🪶 Author

Porumamilla_Akash — Full Stack Developer
🔗 https://github.com/akash335/Team-task-manager-Backend
