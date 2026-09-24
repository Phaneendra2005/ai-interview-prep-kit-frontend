# 🚀 AI Interview Prep Kit — Frontend

### Full-Stack AI-Powered Interview Preparation Platform

The **AI Interview Prep Kit** is a production-ready full-stack application that transforms a job description and company URL into a personalized interview preparation workspace.

The frontend is built with **Next.js, React, TypeScript, and Tailwind CSS** and communicates with a separate Express/TypeScript backend.

## 🌐 Live Application

https://ai-interview-prep-kit-frontend-zeta.vercel.app/

## 💻 Frontend Repository

https://github.com/Phaneendra2005/ai-interview-prep-kit-frontend

## ⚙️ Backend Repository

https://github.com/Phaneendra2005/ai-interview-prep-kit-backend

## ✨ Features

- 🔐 User registration and login
- 🎯 Create personalized interview preparation kits
- 📝 Job description and company URL input
- 📊 Real-time generation progress
- 🏢 Company brief and role breakdown
- 🧠 Requirement-linked interview questions
- 📚 Technical flashcards
- 🔍 Requirement coverage validation
- 🔄 Regenerate missing questions
- ✏️ Edit questions and expected answers
- ➕ Add custom questions
- 🗑️ Delete questions
- 📌 Pin questions
- ↕️ Reorder questions
- 🎴 Interactive flashcard practice mode
- 📈 Confidence tracking
- 📅 Personalized multi-day preparation schedule
- 💾 Persistent user edits
- 📱 Responsive UI for desktop and mobile
- ⚠️ Clear loading, empty, success, and error states

## 🏗️ Frontend Architecture

```text
Next.js Frontend
       │
       │ HTTPS REST API
       ↓
Express + TypeScript Backend
       │
       ├── MongoDB
       └── Google Gemini
```

The frontend uses a centralized API client for backend communication and HTTP-only authentication cookies for user sessions.

## 🛠️ Tech Stack

- **Next.js**
- **React**
- **TypeScript**
- **Tailwind CSS**
- **REST APIs**
- **React Context**
- **Vercel**

## 📁 Project Structure

```text
frontend/
├── app/
│   ├── dashboard/
│   ├── login/
│   ├── register/
│   └── ...
├── components/
├── lib/
│   ├── api.ts
│   └── ...
├── public/
├── package.json
├── next.config.ts
├── tsconfig.json
└── README.md
```

## ⚙️ Environment Setup

Create a `.env.local` file:

```env
NEXT_PUBLIC_API_URL=http://localhost:8080/api
```

For production:

```env
NEXT_PUBLIC_API_URL=https://ai-interview-prep-backend-8qt3.onrender.com/api
```

> No Gemini API keys, MongoDB credentials, session secrets, or other backend secrets are stored in the frontend.

## 💻 Local Development

### 1. Clone

```bash
git clone https://github.com/Phaneendra2005/ai-interview-prep-kit-frontend.git
cd ai-interview-prep-kit-frontend
```

### 2. Install dependencies

```bash
npm install
```

### 3. Configure environment

Create `.env.local`:

```env
NEXT_PUBLIC_API_URL=http://localhost:8080/api
```

### 4. Start the development server

```bash
npm run dev
```

Open:

```text
http://localhost:3000
```

The backend must be running separately.

## 🏭 Production Build

```bash
npm run build
```

Run the production build locally:

```bash
npm start
```

## ☁️ Deployment

The frontend is deployed on **Vercel**.

Production URL:

https://ai-interview-prep-kit-frontend-zeta.vercel.app/

The production frontend communicates with the backend deployed on Render:

https://ai-interview-prep-backend-8qt3.onrender.com

## 🔄 User Workflow

```text
Register / Login
       ↓
Create New Kit
       ↓
Enter Job Description
       ↓
Enter Company URL
       ↓
Select Preparation Days
       ↓
AI Generation
       ↓
Company Brief + Role + Questions + Flashcards
       ↓
Coverage Validation
       ↓
Interview Kit
       ↓
Edit / Add / Delete / Pin / Reorder
       ↓
Regenerate Missing Content
       ↓
Practice Flashcards
       ↓
Follow Preparation Schedule
```

## 🧠 Key Engineering Decisions

### Stable Content Identity

Questions and flashcards use stable unique identifiers to support reliable editing, reordering, pinning, deletion, regeneration, and persistence.

### User Edit Preservation

Regeneration is designed to preserve user-controlled content instead of unnecessarily replacing edits made in the Builder.

### Centralized API Communication

Backend requests are handled through a centralized API client to keep API configuration, authentication, and request handling consistent.

### Responsive User Experience

The interface provides responsive layouts together with clear loading, empty, error, and success states across desktop and mobile devices.

## 🔐 Security

- Authentication handled through HTTP-only cookies
- Backend secrets never exposed to the frontend
- Production API communication over HTTPS
- User-specific protected application data
- Public frontend environment variables contain only the backend API URL

## 🔗 Production Links

| Resource | Link |
|---|---|
| 🌐 Live Application | https://ai-interview-prep-kit-frontend-zeta.vercel.app/ |
| 💻 Frontend Repository | https://github.com/Phaneendra2005/ai-interview-prep-kit-frontend |
| ⚙️ Backend Repository | https://github.com/Phaneendra2005/ai-interview-prep-kit-backend |
| 🚀 Backend API | https://ai-interview-prep-backend-8qt3.onrender.com |

## 👨‍💻 Author

**Phaneendra Kanduri**

Full-Stack Developer | AI/ML Engineer

Built as a full-stack engineering assessment project focused on AI-powered interview preparation, structured generation workflows, deterministic validation, persistence, and user-controlled editing.
