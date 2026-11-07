# StudyMate AI

**An Adaptive Study Planner and Course Material Assistant for University Students**

CSE 4104 – Software Development III | Northern University of Business and Technology, Khulna

> **Status:** Week 2 – project proposal and initial structure. Development starts in the following weeks.

---

## Team Information

| Field | Details |
|---|---|
| Team Name | CSE4104-7G-T05 |
| Section | 7G |
| Team Leader | Md. Samir Ishrak Nafi |
| Course Teacher | Md. Riaz Mahmud, Assistant Professor, Dept. of CSE |

| Student ID | Name | Role |
|---|---|---|
| 11230321442 | Md. Samir Ishrak Nafi | Team Leader and AI Integration Lead |
| 11230321502 | Marshia Hafsa | Database Manager |
| 11230321487 | Zakia Jesmine Jerin | Frontend Developer |
| 11230321493 | Biplobi Akter Sheme | Backend Developer |

---

## Project Description

University students study several courses at once, each with its own chapters, deadlines and exam date. Most plan by hand, and the plan breaks as soon as they miss a few sessions. Turning long course PDFs into something that can be revised also takes a lot of time.

**StudyMate AI** is a web application that:

- builds a personalised daily and weekly study plan from the student's subjects, exam dates, difficulty levels and available hours;
- re-plans automatically when tasks are missed or quiz results show weak topics;
- uses AI to summarise the student's own course PDFs and generate practice quizzes from them.

Every AI feature works only on the student's own stored data and document text, asks the model for structured JSON, and validates the result in the backend before saving it.

---

## Proposed Features

**Core features**

1. Authentication and profile (JWT, password hashing, study preferences)
2. Subject, chapter/topic and exam management with difficulty, priority and exam countdown
3. AI study schedule generator (daily and weekly plan, editable by the student)
4. Adaptive re-scheduling for missed tasks and weak topics
5. PDF upload with AI summary and key points (with page references where possible)
6. AI quiz generator, automatic scoring and weak topic detection
7. Dashboard with progress charts, study streak and exam countdown

**Optional stretch goals** (only if the core features are stable)

- Ask-Your-PDF chatbot with page references
- Flashcards generated from uploaded material
- Bangla language support for AI summaries and explanations
- Admin panel with usage statistics

---

## Technology Stack

| Layer | Technology |
|---|---|
| Frontend | React.js, Tailwind CSS, Recharts |
| Backend | Node.js, Express.js (REST APIs, JWT, bcrypt, pdf-parse) |
| Database | PostgreSQL (Supabase) |
| AI Integration | Gemini API (OpenAI API as an alternative) |
| Deployment | Vercel (frontend), Render (backend), Supabase (database) |
| Tools | GitHub, Figma, Postman, draw.io, dbdiagram.io |

---

## Repository Structure

```
cse4104-7g-t05-studymate-ai/
├── frontend/     # React application
├── backend/      # Express API, authentication, AI integration
├── database/     # Schema and migration files
├── docs/         # Proposal, SRS, design diagrams, reports
├── .gitignore
└── README.md
```

## Branches

`main` (stable) · `development` · `frontend` · `backend` · `ai-integration`

## Getting Started

Setup and installation instructions will be added when the first version of the backend and frontend is committed.

Copy `backend/.env.example` to `backend/.env` and fill in your own values. Never commit real keys.

---

*Developed as the semester project for CSE 4104 – Software Development III.*
