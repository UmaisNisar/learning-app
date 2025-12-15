# Learning App

A full-stack learning project built to practice modern, industry-standard application development using React, .NET, and PostgreSQL.

---

## Tech Stack

### Backend
- .NET 10 (ASP.NET Core Web API)
- Entity Framework Core
- PostgreSQL
- Swagger (OpenAPI)

### Frontend
- React (Vite + TypeScript) — setup in progress

---

## Repository Structure



/client React frontend (to be implemented)
/server .NET Web API backend
/docs Documentation and notes


---

## Prerequisites

- .NET SDK 10
- Node.js (LTS)
- PostgreSQL
- Git

Optional:
- DBeaver or pgAdmin

---

## Backend Setup

### Create Database

```sql
CREATE DATABASE learningapp_dev;

Configure Connection String

Update server/appsettings.Development.json:

{
  "ConnectionStrings": {
    "DefaultConnection": "Host=localhost;Port=5432;Database=learningapp_dev;Username=postgres;Password=YOUR_PASSWORD"
  }
}

Apply Migrations

From the server directory:

dotnet ef database update

Run the API

From the server directory:

dotnet run

Verify API
Health Check
https://localhost:<port>/health


Expected response:

{
  "status": "Healthy",
  "timestamp": "..."
}

Swagger UI
https://localhost:<port>/swagger

Frontend

The frontend will be implemented in the client directory.
Instructions will be added after the frontend skeleton is created.

Notes

This project is for learning purposes

Authentication and frontend integration will be added incrementally

Production deployment is out of scope


---

When pasted and committed, reply with:



README task complete


Then we officially close **Sprint 1** and move into **Frontend Skeleton Setup** 🚀
