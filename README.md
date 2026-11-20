# Acquisitions API

A Node.js REST API built with Express 5 and PostgreSQL, demonstrating modern backend development and DevOps practices.

## Tech Stack

- **Runtime:** Node.js 18
- **Framework:** Express 5
- **Database:** PostgreSQL (Neon)
- **ORM:** Drizzle ORM
- **Validation:** Zod
- **Authentication:** JWT and bcrypt
- **Logging:** Winston and Morgan
- **Testing:** Jest and Supertest
- **Containerization:** Docker and Docker Compose
- **CI/CD:** GitHub Actions
- **Code Quality:** ESLint and Prettier

## Features

- Modular REST API architecture.
- JWT-based authentication and password hashing.
- PostgreSQL database integration with Drizzle ORM.
- Database migrations.
- Request validation and security middleware.
- Centralized logging and error handling.
- Automated API testing.
- Separate Docker development and production environments.
- Automated code quality and testing workflows.

## Getting Started

### Prerequisites

- Node.js 18+
- npm
- Docker and Docker Compose

### Installation

Clone the repository:

```bash
git clone https://github.com/Kibika/acquisitions.git
cd acquisitions
```

Install dependencies:

```bash
npm install
```

Configure the required environment variables in `.env.development` or `.env.production`, including your database connection string and authentication secrets.

### Run Locally

```bash
npm run dev
```

### Run with Docker

Development:

```bash
npm run dev:docker
```

Production:

```bash
npm run prod:docker
```

## Database Commands

```bash
npm run db:generate
npm run db:migrate
npm run db:studio
```

## Testing & Code Quality

```bash
npm test
npm run lint
npm run format
```

## API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| GET | `/` | Welcome endpoint |
| GET | `/health` | Health check |
| GET | `/api` | API status |
| `/api/auth` | Authentication routes |
| `/api/users` | User management routes |

## Project Structure

```text
src/
├── config/
├── controllers/
├── middleware/
├── models/
├── routes/
├── services/
├── utils/
├── validations/
├── app.js
├── index.js
└── server.js

drizzle/               # Database migrations
tests/                 # Automated tests
scripts/               # Docker scripts
.github/workflows/     # CI/CD workflows
```
## Acknowledgements

Inspired by the **[JavaScript Mastery – DevOps from Zero to Hero](https://www.youtube.com/watch?v=H5FAxTBuNM8)** course by Adrian Hajdin.