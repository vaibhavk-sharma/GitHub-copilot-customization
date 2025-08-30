---
applyTo: "backend/**/*.{js,ts}"
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
- Structure Express routes clearly and modularly (e.g., `routes/`, `controllers/`, `services/`).
- Keep functions **small and single-responsibility**.
- Use **dependency injection** patterns for better testability.
- Use **TypeScript** whenever possible, with explicit type definitions.
- Prefer `import` / `export` ES Modules syntax instead of `require`.
- Use **async/await** for asynchronous code, never raw `.then()` chains.
- Always handle async operations with **try/catch** for error safety.

## Folder Conventions

- `/server/routes`: API route definitions
- `/server/controllers`: Request handlers
- `/server/services`: Business logic
- `/server/db`: DB connection and SQL queries or ORM models

## API Practices

- RESTful routes: use standard HTTP verbs and naming (e.g., `/api/tasks/:id`)
- Always validate user input using middleware or libraries like `Joi` or `Zod`.
- Use status codes appropriately (e.g., `200`, `201`, `400`, `404`, `500`).

## Environment & Config
- Use **dotenv** or equivalent for environment variables.
- Never hardcode secrets, API keys, or DB credentials.
- Default configs should be safe for production.

## PostgreSQL

- Store SQL scripts or schema migrations under `/db`.
- Prefer parameterized queries to prevent SQL injection.
- Use meaningful table and column names without prefixes like `tbl_`.

## Code Quality
- Write **JSDoc/TSDoc comments** for functions and APIs.
- Avoid unused imports, variables, or dead code.
- Follow **consistent naming** conventions (`camelCase` for variables, `PascalCase` for classes).

