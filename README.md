# NMD Football Booking

Web app for booking football fields in Oradea, like Mero but for sports venues. Team project for Inginerie Software II (team NMD: Denis Todoran, Daniel Niculcea, Alexia Molnar).

## Tech stack

- Backend: ASP.NET Core Web API (C#), Entity Framework Core
- Database: PostgreSQL
- Frontend: React (Vite)
- CI: GitHub Actions

## Repository structure

- `backend/` - ASP.NET Core Web API and tests
- `frontend/` - React app

## Run locally

Requirements: .NET SDK 8+, Node.js 20+, Docker (for PostgreSQL).

1. Start PostgreSQL:
   ```
   docker run --name nmd-db -e POSTGRES_PASSWORD=postgres -p 5432:5432 -d postgres:16
   ```
2. Backend: `cd backend`, then `dotnet run`
3. Frontend: `cd frontend`, then `npm install` and `npm run dev`

These steps will be updated once the backend and frontend projects are generated.

## Workflow

- Tickets live in Jira (project "Inginerie Software II - Proiect", label NMD)
- One branch per ticket, e.g. `feature/SCRUM-195-free-slots`
- Pull request into `main` with at least one review from a teammate
