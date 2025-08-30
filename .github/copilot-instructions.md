# GitHub Copilot Repository Instructions

## Project Overview

This is a full-stack web application that allows users to manage their tasks and to-do lists. It is built with a **React frontend**, **Node.js backend (Express)**, and uses **PostgreSQL** as the relational database.

Always generate code that follows these conventions.

---

## General Rules
- Use **TypeScript** consistently across frontend and backend.
- Prefer **ES Modules** (`import/export`) instead of CommonJS (`require`).
- Write **clear JSDoc/TSDoc comments** for all exported functions, APIs, and components.
- Ensure **error handling** and **input validation** in backend code.
- Avoid unused imports, variables, or dead code.
- Follow **security best practices** (sanitize input, prevent SQL injection, protect secrets).

---

## Folder Structure

- `/src`: Contains React application source code.
- `/server`: Contains Node.js backend (Express) source code.
- `/docs`: Documentation including API specifications and guides.
- `/db`: SQL schema files or migration scripts for PostgreSQL.

---

## Libraries and Frameworks

- **Frontend**: React (with functional components), Tailwind CSS
- **Backend**: Node.js with Express
- **Database**: PostgreSQL (accessed via pg or Sequelize/Prisma — see backend instructions)

---

## Coding Standards

- Use **semicolons** at the end of each statement.
- Use **single quotes** for all strings.
- Use **arrow functions** for all callbacks and handlers.
- Prefer **function-based components** in React.
- Follow **consistent indentation** (2 spaces per level).

---

## UI Guidelines

- UI should follow a **clean, modern design** using Tailwind CSS.
- Include a toggle for **light and dark mode**.
- Ensure responsiveness across devices using Tailwind utilities.
