<div align="center">

# Study Planner

**Plan your coursework, connect it to your notes, and study smarter with AI.**

![Status](https://img.shields.io/badge/status-in%20development-orange)
![Backend](https://img.shields.io/badge/backend-FastAPI-009688?logo=fastapi&logoColor=white)
![Frontend](https://img.shields.io/badge/frontend-React%20%2B%20TypeScript-3178C6?logo=react&logoColor=white)
![Database](https://img.shields.io/badge/database-PostgreSQL-4169E1?logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/docker-ready-2496ED?logo=docker&logoColor=white)

</div>

---

## About

Study Planner is a web app for university students that combines assignment management with an AI-powered study assistant. Its core idea is that **tasks and study materials are connected**: every assignment or exam links to its own notes and flashcards.

This project is built in public over 14 weeks as a full-stack portfolio piece covering **UI/UX design, front end, and back end**.

> 🚧 **Work in progress.** Live demo and screenshots will be added with the v1.0 release.

##  Planned Features

### v1.0: Core
-  Registration and login (JWT)
-  Semester and course management
-  Task management with deadlines, types, priorities, and status
-  "Today", "This week", and "Overdue" dashboard
-  Notes per course
-  Flashcards with practice mode
-  Light and dark theme

### v2.0: Differentiators
-  Grade weights and estimated grade per course
-  Calendar view and `.ics` export for Google Calendar
-  Spaced repetition using the SM-2 algorithm
-  Pomodoro timer and study statistics dashboard
-  Exam mode with countdown and daily study plan

### v3.0: AI
-  Auto-generate flashcards and quizzes from notes
-  AI-generated study plans that turn into tasks
-  Material summaries

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Design | Figma |
| Front End | React, TypeScript, Vite, Tailwind CSS |
| Back End | Python, FastAPI |
| Database | PostgreSQL, SQLAlchemy, Alembic |
| Auth | JWT, bcrypt |
| Testing | pytest, Vitest |
| DevOps | Docker, docker-compose, GitHub Actions |
| Deployment | Vercel (front end), Render (back end + database) |

## Roadmap

- [x] **Phase 0:** Setup (repo, tools, project board)
- [ ] **Phase 1:** UI/UX research and design
- [ ] **Phase 2:** Database and back end
- [ ] **Phase 3:** Front end
- [ ] **Phase 4:** Release v1.0
- [ ] **Phase 5:** Release v2.0
- [ ] **Phase 6:** Release v3.0

Progress is tracked on the [project board](https://github.com/users/Rnascaa/projects/1).

## Project Structure

```text
study-planner/
├── backend/     # FastAPI application
├── frontend/    # React + TypeScript application
└── docs/        # Research, design, and contributing guide
```

## Contributing

Commit and branch conventions are documented in [docs/CONTRIBUTING.md](docs/CONTRIBUTING.md).

---

<div align="center">

Built by [@Rnascaa](https://github.com/Rnascaa)

</div>