# 🎁 SecretGift – Anonymous Gift Exchange

## 🚀 SWYNEX Task 4 – Complete Deployed Application

**SecretGift** is a complete full-stack web application developed as part of the **SWYNEX Full-Stack Development Internship**.

It makes gift exchanges fun, private, and organized. Users can create private gift exchange groups, invite friends using a unique invite code, manage wishlists, and receive secret gift assignments.

---

## 📌 Project Overview

Users can create a private gift exchange group, set a gift budget and reveal date, and invite other participants using a unique invite code.

The system randomly assigns each participant a secret gift recipient while ensuring that **no user is assigned to themselves**.

Each participant can only view their own assigned recipient, keeping the gift exchange private until the reveal date.

---

## ✨ Features

### 🔐 User Authentication

- User registration
- User login and logout
- JWT-based authentication
- Password security using bcrypt
- Protected application routes

### 🎁 Gift Group Management

- Create private gift exchange groups
- Set a group name
- Set a gift budget
- Set a reveal date
- Generate a unique invite code
- View and manage groups

### 👥 Join Groups

- Join groups using an invite code
- View group members
- Manage active gift exchange groups

### 🎲 Secret Gift Assignment

- Randomly assign participants
- Prevent users from being assigned to themselves
- Keep assignments private
- Allow each participant to view only their own recipient

### 📝 Wishlist Management

Users can:

- Add gift wishes
- Edit gift wishes
- Delete gift wishes

The assigned gift giver can view their recipient's wishlist.

### 📊 Dashboard

The dashboard displays information such as:

- Active gift groups
- Gift budget
- Reveal date
- Group members
- Secret recipient
- Countdown to the reveal date

### 🎉 Final Reveal

After the reveal date, secret gift assignments can be revealed to group members.

---

## 🛠️ Technology Stack

### Frontend

- React
- TypeScript
- Vite
- Tailwind CSS

### Backend

- Node.js
- Express.js
- TypeScript

### Database

- MongoDB
- Mongoose

### Authentication

- JWT
- bcrypt

---

## 📁 Project Structure

```text
SWYNEX-Complete-Deployed-Application/
│
├── client/                     # React + Vite Frontend
│   ├── public/
│   ├── src/
│   │   ├── api/                # API integration
│   │   ├── assets/             # Images and assets
│   │   ├── components/         # Reusable UI components
│   │   ├── context/            # Authentication and state management
│   │   ├── types/              # TypeScript interfaces
│   │   ├── App.tsx
│   │   ├── index.css
│   │   └── main.tsx
│   ├── index.html
│   ├── package.json
│   └── vite.config.ts
│
├── server/                     # Node.js + Express Backend
│   ├── middleware/             # JWT authentication middleware
│   ├── models/                 # Database models
│   ├── routes/                 # API routes
│   ├── utils/                  # Secret assignment logic
│   ├── store.ts                # Database/persistence logic
│   ├── app.ts
│   ├── server.ts
│   ├── .env.example
│   └── package.json
│
├── screenshots/                # Application screenshots
│
├── README.md
└── .gitignore
```

---

## ⚙️ Installation and Setup

### 1. Clone the Repository

```bash
git clone <your-repository-url>
cd SWYNEX-Complete-Deployed-Application
```

### 2. Install Backend Dependencies

```bash
cd server
npm install
```

### 3. Create Environment Variables

Create a `.env` file inside the `server` folder:

```env
PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
```

### 4. Start the Backend

```bash
npm start
```

The backend will run on:

```text
http://localhost:5000
```

### 5. Install Frontend Dependencies

Open another terminal and run:

```bash
cd client
npm install
```

### 6. Start the Frontend

```bash
npm run dev
```

The frontend will usually run on:

```text
http://localhost:5173
```

---

## 🔄 How SecretGift Works

### 1️⃣ Create an Account

Users register and log in to the application.

### 2️⃣ Create a Gift Group

The user creates a private gift exchange group and sets details such as:

```text
Group Name: Christmas Surprise 🎄
Budget: ₹1000
Reveal Date: December 25
```

### 3️⃣ Share the Invite Code

The system generates a unique invite code.

Other users can join the group using this code.

### 4️⃣ Add Wishlists

Each participant adds gift ideas to their personal wishlist.

### 5️⃣ Generate Secret Assignments

The system randomly assigns each participant another person.

```text
User A → User B
User B → User C
User C → User D
User D → User A
```

No participant can be assigned to themselves.

### 6️⃣ Keep It Secret 🤫

Each user can only see their own assigned recipient.

### 7️⃣ Final Reveal 🎉

After the reveal date, the secret assignments can be revealed.

---

## 🗄️ Database Models

### 👤 User

```text
User
├── name
├── email
├── password
└── createdAt
```

### 🎁 Gift Group

```text
GiftGroup
├── groupName
├── createdBy
├── members
├── budget
├── inviteCode
├── revealDate
└── createdAt
```

### 📝 Wishlist

```text
Wishlist
├── userId
├── groupId
├── itemName
└── description
```

---


## 🔒 Security

- Passwords are protected using bcrypt.
- JWT is used for authentication.
- Protected routes require authorized access.
- Secret assignments remain private before the reveal date.

---

## 🎯 What I Learned

This project helped me gain practical experience in:

- Full-stack web development
- React and TypeScript
- REST API development
- Node.js and Express.js
- MongoDB database integration
- JWT authentication
- CRUD operations
- Frontend and backend integration
- Application deployment

---

## 👩‍💻 Author

**Pooja G**

---

## 📄 Internship

**SWYNEX Full-Stack Development Internship**

**Task 4 – Complete Deployed Application**

---

### 🎁 Made with React, Node.js, Express.js, TypeScript and MongoDB
