# ✈️ Flight Booking & Management System

> A full-stack MERN application for booking flights, managing reservations, and administering flight operations.

![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat&logo=mongodb&logoColor=white)
![Express](https://img.shields.io/badge/Express.js-000000?style=flat&logo=express&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat&logo=react&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=nodedotjs&logoColor=white)

---

## 🎥 Demo

> 📽️ [Watch Demo Video](https://drive.google.com/file/d/1ebbjfQyS7f9kod-dEQ_rdz0-wZmH47k4/view?usp=sharing)

---

## 💡 About

A complete flight reservation platform with three role-based modules — **Customer**, **Admin**, and **Flight Operator** — built as a MERN stack course project.

---

## ✨ Features

### 👤 Customer
- Register, login, and manage profile
- Search flights (one-way & return) by date & destination
- Book tickets with passenger details
- View booking history & cancel bookings

### 🛠 Admin
- Dashboard with total users, bookings, flights & operators
- Approve or reject flight operator registrations
- Manage all users, bookings, and flights

### 🛫 Flight Operator
- Request admin approval to onboard
- Add, edit, and manage flights
- View bookings for their own flights

### 🔒 System
- JWT-based authentication
- Role-based route protection (Customer / Admin / Operator)
- Password hashing with bcrypt
- Responsive UI with React + Bootstrap

---

## 🛠 Tech Stack

| Layer | Technology |
|---|---|
| Frontend | React.js, Context API, React Router, Axios, Bootstrap |
| Backend | Node.js, Express.js |
| Database | MongoDB + Mongoose |
| Auth | JWT + bcrypt |

---

## 📁 Folder Structure

```
flight-booking/
├── client/                    # React Frontend
│   └── src/
│       ├── components/        # Navbar, Cards, Forms
│       ├── pages/             # Landing, Login, Dashboard pages
│       ├── context/
│       │   └── GeneralContext.jsx  # Auth, token, global state
│       ├── RouteProtectors/   # Protected routes
│       └── styles/
│
└── server/                    # Node.js Backend
    ├── controllers/           # Business logic
    ├── models/                # MongoDB schemas
    ├── routes/                # API routes
    ├── middleware/            # JWT auth middleware
    └── server.js
```

---

## 🚀 Quick Start

### Prerequisites
- Node.js v16+
- MongoDB (local or Atlas)

### 1. Clone the repo
```bash
git clone https://github.com/Ranjitha04-S/flight-booking.git
```

### 2. Backend Setup
```bash
cd server
npm install
```

Create `.env` in `server/`:
```env
PORT=6001
MONGO_URL=mongodb://localhost:27017/flightapp
JWT_SECRET=your_secret_key
```

```bash
npm start
```

### 3. Frontend Setup
```bash
cd client
npm install
npm start
```

- Frontend → `http://localhost:3000`
- Backend → `http://localhost:6001`

---

## 🔌 API Reference

### Auth
| Method | Endpoint | Description |
|---|---|---|
| POST | `/register` | Register new user |
| POST | `/login` | Login + return JWT |

### Flights
| Method | Endpoint | Description |
|---|---|---|
| GET | `/fetch-flights` | Get all flights |
| GET | `/fetch-flight/:id` | Get single flight |
| POST | `/add-flight` | Add new flight |
| PUT | `/update-flight` | Update flight |

### Bookings
| Method | Endpoint | Description |
|---|---|---|
| POST | `/book-ticket` | Book a flight |
| GET | `/fetch-bookings` | Get all bookings |
| PUT | `/cancel-ticket/:id` | Cancel booking |

### Admin
| Method | Endpoint | Description |
|---|---|---|
| GET | `/fetch-users` | Get all users |
| POST | `/approve-operator` | Approve operator |
| POST | `/reject-operator` | Reject operator |

---

## 🔮 Future Enhancements

- Real-time seat availability
- Payment gateway integration
- Email/SMS ticket confirmation
- Analytics dashboard for admin
- Mobile app using React Native

---

## 👩‍💻 Developer

**Ranjitha S** — Full Stack Developer
[@Ranjitha04-S](https://github.com/Ranjitha04-S)
