# TaskFlow

A collaborative project management application inspired by Kanban tools, built for the CodeAlpha Full Stack Development internship.

## Features
- Register and log in securely
- Create and manage collaborative projects
- Create tasks, set priority and assign members
- Update task status across workflow columns
- Add comments to tasks
- Project activity and SQLite persistence
- JWT-protected REST API and responsive UI

## Stack
Node.js, Express, SQLite (better-sqlite3), HTML, CSS and vanilla JavaScript.

## Run locally
```bash
npm install
cp .env.example .env
# Set a long random JWT_SECRET in .env
npm run dev
```
Open http://localhost:3000.

## API
- POST /api/auth/register
- POST /api/auth/login
- GET/POST /api/projects
- GET/POST /api/projects/:id/tasks
- PATCH /api/tasks/:id
- GET/POST /api/tasks/:id/comments
- GET /api/health

The SQLite database is created automatically in data/app.db. This is an educational internship project; review and test before production use.
