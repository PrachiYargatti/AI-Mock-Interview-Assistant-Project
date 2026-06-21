
# 🎤 AI Mock Interview Assistant

An AI-powered mock interview platform that helps users practice technical interviews with personalized questions, resume-based interview generation, voice interaction, code editor support, and detailed AI feedback.

## 🚀 Live Demo

* **Frontend:** https://ai-mock-interview-assistant-project.vercel.app
* **Backend API:** https://ai-mock-interview-assistant-project.onrender.com

---

## 📌 Features

* 🔐 User Authentication (Register/Login using JWT)
* 📄 Resume Upload and Analysis
* 🤖 AI-generated interview questions
* 🎙️ Voice-based interview responses
* 💻 Built-in code editor for coding questions
* 📝 Text-based answer submission
* 📊 AI-generated interview feedback and scoring
* 📚 Interview history tracking
* 🔒 Protected routes using JWT authentication
* 🌐 Fully responsive user interface

---

## 🛠️ Tech Stack

### Frontend

* React.js
* Vite
* Axios
* React Router DOM
* CSS

### Backend

* Node.js
* Express.js
* MongoDB Atlas
* Mongoose
* JWT Authentication
* Multer

### AI & APIs

* Google Gemini API
* AssemblyAI API
* Murf AI API

### Deployment

* Frontend: Vercel
* Backend: Render
* Database: MongoDB Atlas

---

## 📂 Project Structure

```
AI-Mock-Interview-Assistant-Project/
│
├── client/                 # React (Vite) Frontend
│   ├── src/
│   ├── public/
│   └── package.json
│
├── server/                 # Node.js Backend
│   ├── src/
│   ├── server.js
│   └── package.json
│
└── README.md
```

---

## ⚙️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/PrachiYargatti/AI-Mock-Interview-Assistant-Project.git
cd AI-Mock-Interview-Assistant-Project
```

---

### 2. Backend Setup

```bash
cd server
npm install
```

Create a `.env` file inside the `server` folder.

Required environment variables:

```env
PORT=5000
NODE_ENV=development
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
JWT_EXPIRES_IN=7d
GEMINI_API_KEY=your_gemini_api_key
ASSEMBLYAI_API_KEY=your_assemblyai_api_key
MURF_API_KEY=your_murf_api_key
CLIENT_URL=http://localhost:5173
```

Start the backend:

```bash
npm run dev
```

---

### 3. Frontend Setup

```bash
cd client
npm install
```

Create a `.env` file inside the `client` folder.

```env
VITE_API_URL=http://localhost:5000/api
```

Start the frontend:

```bash
npm run dev
```

---

## 📡 API Routes

### Authentication

| Method | Endpoint             |
| ------ | -------------------- |
| POST   | `/api/auth/register` |
| POST   | `/api/auth/login`    |
| GET    | `/api/auth/me`       |
| POST   | `/api/auth/logout`   |

### Resume

| Method | Endpoint             |
| ------ | -------------------- |
| POST   | `/api/resume/upload` |
| GET    | `/api/resume`        |

### Interview

| Method | Endpoint                          |
| ------ | --------------------------------- |
| POST   | `/api/interview/start`            |
| POST   | `/api/interview/:id/answer`       |
| POST   | `/api/interview/:id/answer-audio` |
| POST   | `/api/interview/:id/code`         |
| POST   | `/api/interview/:id/end`          |
| GET    | `/api/interview/:id`              |

### History

| Method | Endpoint             |
| ------ | -------------------- |
| GET    | `/api/history`       |
| GET    | `/api/history/:id`   |
| DELETE | `/api/history/:id`   |
| DELETE | `/api/history/clear` |

---

## 🌍 Deployment

### Frontend

* Vercel

### Backend

* Render

### Database

* MongoDB Atlas

---

## 🔮 Future Enhancements

* Video interview support
* Real-time AI interviewer
* Company-specific interview preparation
* Leaderboard and performance analytics
* Multi-language interview support
* Email interview reports

---

## 👩‍💻 Author

**Prachi Yargatti**

GitHub: https://github.com/PrachiYargatti
