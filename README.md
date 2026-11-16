# StudyMate AI

**An Adaptive Study Planner and Course Material Assistant for University Students**

CSE 4104 – Software Development III | Northern University of Business and Technology, Khulna

> **Status:** Week 3 – Software Requirement Specification and initial system diagrams completed. System design and development follow.

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

## Objectives

1. Generate personalised daily and weekly study schedules from subjects, exam dates, difficulty levels and available study hours.
2. Adapt the schedule automatically when tasks are missed or quiz results show weak topics, without overloading any single day.
3. Summarise uploaded course PDFs and extract key points with page references.
4. Generate quizzes from the student's own material and use the results to detect weak topics.
5. Improve study consistency with a dashboard showing progress, study streak and exam countdown.
6. Deliver a complete, tested, deployed and documented system.

---

## Features

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
│   └── .env.example
├── database/     # Schema and migration files
├── docs/         # Project documents and diagrams
│   ├── CSE4104-7G-T05_Proposal.pdf
│   ├── CSE4104-7G-T05_SRS.pdf
│   ├── CSE4104-7G-T05_UseCaseDiagram.pdf
│   ├── CSE4104-7G-T05_ERDiagram.pdf
│   └── CSE4104-7G-T05_ArchitectureDiagram.pdf
├── .gitignore
└── README.md
```

## Documentation

| Document | File |
|---|---|
| Project proposal (Week 2) | `docs/CSE4104-7G-T05_Proposal.pdf` |
| Software Requirement Specification (Week 3) | `docs/CSE4104-7G-T05_SRS.pdf` |
| Use case diagram | `docs/CSE4104-7G-T05_UseCaseDiagram.pdf` |
| ER diagram | `docs/CSE4104-7G-T05_ERDiagram.pdf` |
| System architecture diagram | `docs/CSE4104-7G-T05_ArchitectureDiagram.pdf` |

## Branches

`main` (stable) · `development` · `frontend` · `backend` · `ai-integration`

## Getting Started

Setup and installation instructions will be added when the first version of the backend and frontend is committed.

Copy `backend/.env.example` to `backend/.env` and fill in your own values. Never commit real keys.

---

*Developed as the semester project for CSE 4104 – Software Development III.*
