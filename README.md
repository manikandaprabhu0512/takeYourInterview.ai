# 🤖 takeYourInterview.ai — AI-Powered Interview Platform

An AI-driven interview preparation platform that generates personalized interview questions from user profiles/resumes, conducts interactive interviews, and provides structured feedback using LLM-based evaluation.

---

## 🚀 Features

- Resume-based interview generation using LLMs.
- Supports both Technical and HR interview modes.
- AI-generated questions tailored to user profile and skills.
- Credit-based interview system to manage usage.
- Voice interaction using browser-based speech APIs (STT/TTS).
- Timed responses with difficulty progression (easy → hard).
- Instant answer evaluation with feedback and improvement suggestions.
- Comprehensive post-interview report (correctness, communication, confidence).
- Secure authentication using Google OAuth 2.0.
- Deployed with scalable backend (AWS EC2) and frontend (Vercel) .

---

## 🧠 System Overview

The platform simulates a real interview experience by combining LLM-based question generation, real-time interaction, and automated evaluation.

### Flow

1. User logs in via Google OAuth.
2. User uploads resume or provides profile details.
3. Credits are checked before starting an interview.
4. LLM processes input and extracts relevant skills.
5. System generates interview questions based on role and difficulty.
6. User answers via voice or text within a time limit.
7. LLM evaluates responses and provides feedback.
8. Final report is generated with detailed insights.

---

## ⚙️ Tech Stack

### Frontend

- React
- Tailwind CSS
- Web Speech API (Speech-to-Text & Text-to-Speech)

### Backend

- Node.js
- Express.js

### AI / LLM

- LLM APIs (OpenRouter or similar)
- Prompt engineering
- Basic RAG pipeline

### Database

- MongoDB

### DevOps & Deployment

- AWS EC2 (backend hosting)
- Vercel (frontend hosting)
- GitHub Actions (CI/CD)

---

## 🔄 Key Components

- Resume Parser → Extracts user skills and context using LLM.
- Question Generator → Generates role-specific interview questions.
- Evaluation Engine → Analyzes answers and provides structured feedback.
- Voice Engine → Handles speech input/output using browser APIs.
- Report Generator → Summarizes performance across multiple dimensions.

---

## 🛠️ Setup (Local Development)

1. Clone the repository
2. Install dependencies

```bash
npm install
```

3. Create `.env` file
   cp .env.sample file

4. Add required keys

5. Run the app

```bash
npm run dev
```

---

## Environment Variables

Example `.env.example`:

PORT=8000  
MONGO_URI=your_mongodb_connection_string  
JWT_SECRET=your_jwt_secret  
OPENROUTER_API_KEY=your_openrouter_api_key  
RAZORPAY_KEY_ID=your_razorpay_key_id  
RAZORPAY_KEY_SECRET=your_razorpay_client_secret

---

## 🔗 Live Demo

- Frontend: https://take-your-interview-front-end.vercel.app
- Backend: http://takeyourinterview-ags-1-682670051.ap-south-1.elb.amazonaws.com

---

## 💡Key Learnings

- Built AI-powered user-facing applications using LLM APIs
- Designed prompt-based evaluation systems for open-ended responses
- Handled real-time user interaction with voice and timers
- Integrated authentication and cloud deployment in full-stack systems
- Balanced user experience with AI latency and cost considerations

---

## 🚀 Future Improvements

- Advanced RAG with vector databases
- Adaptive questioning based on performance
- Multi-round interview simulation
- Analytics dashboard for progress tracking

---

## 📌 Notes

This project focuses on combining AI capabilities with real-time interaction to simulate realistic interview environments.
