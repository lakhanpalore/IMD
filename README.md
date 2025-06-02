# 📦 Inventory Management System (Full-Stack MERN + Prisma + Next.js)

A production-ready inventory management system built using the **MERN stack** with **Next.js**, **TypeScript**, and **Prisma ORM**. This system allows admins to manage inventory, view dashboards, track purchases, and monitor expenses with a clean and modern UI.

> 🚀 Split into two parts:  
> 🖥️ `inventory-management/` → Frontend (Next.js)  
> 🔧 `server/` → Backend API (Express + Prisma + PostgreSQL)


![Screenshot 2025-06-02 134509](https://github.com/user-attachments/assets/f6cb99a5-9110-45b9-9130-afd1461e93e0)


## 📁 Project Structure
```
├── inventory-management/ # Frontend (Next.js + TS)
│ ├── pages/
│ ├── app/components/
│ ├── dashboard/
│ ├── inventory/
│ ├── state/ # Redux or global state
│ └── .env.local
│
├── server/ # Backend (Node.js + Prisma)
│ ├── src/
│ │ ├── controllers/
│ │ ├── routes/
│ │ ├── prisma/ # Prisma client and schema
│ │ └── server.ts
│ └── .env
```

---

## 🧰 Tech Stack

| Layer     | Tech                                      |
|-----------|-------------------------------------------|
| Frontend  | Next.js, React, TypeScript, Tailwind CSS  |
| Backend   | Node.js, Express.js, Prisma ORM           |
| Database  | PostgreSQL (or your DB of choice)         |
| State     | Redux (or useContext)                     |
| Auth      | (Optional) NextAuth / JWT                 |

---

## ⚙️ Backend Setup (`server/`)

1. **Navigate:**

```bash
cd server
npm install
```

```.env
> NEXT_PUBLIC_API_BASE_URL=http://localhost:8000
> PORT=8000
> DATABASE_URL=postgresql://user:password@localhost:5432/yourdb
```
```
npx prisma migrate dev
npx prisma generate
npm run dev
```

2. Frontend
```bash
cd inventory-management
npm install
npm run dev
```

