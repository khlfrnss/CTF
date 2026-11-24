# Nexus CTF Platform

Nexus is a real-time capture-the-flag platform for hosting collaborative cybersecurity and puzzle challenges. It brings live games, team progress, scoring, and event controls together in one web application.

## What the system does

Depending on how a game is configured, Nexus can:

- Let players create an account, join a game with a code, and compete solo or as a team.
- Present staged challenges with custom content, instructions, hints, and flag submissions.
- Track challenge progress, submissions, scores, hints, and game events.
- Update player and gamemaster views in real time.
- Give gamemasters tools to create game rooms, configure timing and scoring, manage challenges, monitor participants, and send announcements.
- Show leaderboards, game results, and spectator views for active events.

## Run locally

### Requirements

- Node.js and npm
- MySQL

The backend defaults to MySQL on `localhost`, using user `root`, an empty password, and database `ctf_platform`. Update `server/db/connection.js` if your local MySQL credentials differ.

### Install dependencies

From the repository root:

```powershell
cd server
npm ci
cd ..\client
npm ci
```

### Start the system
Open two terminals in the repository folder.

In the first terminal, start the backend:
cd server
npm run dev

In the second terminal, start the frontend:
cd client
npm run dev
