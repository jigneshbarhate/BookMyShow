# 🎬 BookMyShow – Movie Ticket Booking Website (Full Stack)

A full-stack **Movie Ticket Booking Web Application** inspired by **BookMyShow**, where users can select a movie, choose a time slot, book seats, and view the **last booking details**.
This project is built as part of a **Full Stack assignment** using **React, Node.js, Express, and MongoDB**.

---

## 🚀 Live Demo

* **Frontend (Netlify):** [https://book-m-show.netlify.app](https://book-m-show.netlify.app)
* **Backend (Render):** [https://bookmyshow-ktcy.onrender.com](https://bookmyshow-ktcy.onrender.com)
* **API Endpoint:** `/api/booking`

---

## 🛠 Tech Stack

### Frontend

* React.js
* JavaScript (ES6)
* HTML5 & CSS3
* Webpack
* Axios / Fetch API
* Netlify (Deployment)

### Backend

* Node.js
* Express.js
* MongoDB Atlas
* Mongoose
* Render (Deployment)

---

## 📌 Features

* 🎥 Select movie from predefined list
* ⏰ Choose a time slot
* 💺 Select number of seats by type (A1, A2, A3, A4, D1, D2)
* 📦 Book tickets with a single API request
* 🕒 View **Last Booking Details**
* 💾 User selections persist using **localStorage**
* 🌐 Fully deployed frontend & backend
* 📱 Responsive UI

---

## 📂 Project Structure

```
BookMyShow/
├── client/                # Frontend
│   ├── src/
│   ├── webpack.config.js
│   └── package.json
│
├── server/                # Backend
│   ├── index.js
│   ├── connector.js
│   ├── schema.js
│   └── package.json
│
└── README.md
```

---

## 🔌 Backend API Endpoints

### ➤ Create Booking

**POST** `/api/booking`

**Request Body:**

```json
{
  "movie": "Tenet",
  "slot": "10:00 AM",
  "seats": {
    "A1": 2,
    "A2": 1,
    "A3": 0,
    "A4": 0,
    "D1": 0,
    "D2": 0
  }
}
```

**Success Response (200):**

```json
{
  "message": "Booking Successful",
  "data": { ... }
}
```

---

### ➤ Get Last Booking

**GET** `/api/booking`

**Response:**

```json
{
  "movie": "Tenet",
  "slot": "10:00 AM",
  "seats": {
    "A1": 2,
    "A2": 1
  }
}
```

If no booking exists:

```json
{
  "message": "No Previous Booking found!"
}
```

---

## 🗄 Database

* **MongoDB Atlas**
* Stores booking details using Mongoose schema
* Collection: `bookmovietickets`

---

## ⚙️ Environment Variables

### Backend (`server/.env`)

```env
MONGO_URI=your_mongodb_connection_string
PORT=8080
```

---

## 🧪 How to Run Locally

### Backend

```bash
cd server
npm install
node index.js
```

### Frontend

```bash
cd client
npm install
npm run start
```

---

## 🌍 Deployment

* **Backend:** Deployed on Render
* **Frontend:** Deployed on Netlify
* **Node Version Locked:** v16 (for Webpack compatibility)

---

## 🧠 Key Learnings

* Full-stack project structure
* REST API creation
* MongoDB integration using Mongoose
* Handling environment variables
* Netlify & Render deployment
* Fixing Node + Webpack OpenSSL compatibility issues

---

## 👤 Author

**Jignesh Barhate**
Computer Science Student
SRM Institute of Science and Technology, Chennai

---

## ⭐ Acknowledgements

* Inspired by **BookMyShow**
* Reference UI & behavior based on assignment guidelines

---

### ✅ If you like this project, feel free to ⭐ the repository!
