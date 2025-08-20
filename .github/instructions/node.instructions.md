---
applyTo: "backend/**/*.js"
---

# GitHub Copilot Node.js Instructions

## Framework & Stack

- Use **Node.js with Express** for the backend.
- Use **PostgreSQL** as the database.
- Database access can be done via:
  - Native `pg` module (preferred for full control), or
  - **Sequelize** / **Prisma** (if using an ORM)

## Code Style

- Use **semicolons** at the end of all statements.
- Use **single quotes** for all strings.
- Use **arrow functions** for callbacks and middleware.
- Use consistent error handling (`try/catch` or async error wrappers).
- Structure Express routes clearly and modularly (e.g., `routes/`, `controllers/`, `services/`).

## Folder Conventions

- `/server/routes`: API route definitions
- `/server/controllers`: Request handlers
- `/server/services`: Business logic
- `/server/db`: DB connection and SQL queries or ORM models

## API Practices

- RESTful routes: use standard HTTP verbs and naming (e.g., `/api/tasks/:id`)
- Always validate user input using middleware or libraries like `Joi` or `Zod`.
- Use status codes appropriately (e.g., `200`, `201`, `400`, `404`, `500`).

## PostgreSQL

- Store SQL scripts or schema migrations under `/db`.
- Prefer parameterized queries to prevent SQL injection.
- Use meaningful table and column names without prefixes like `tbl_`.
