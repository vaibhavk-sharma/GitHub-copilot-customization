---
applyTo: "src/**/*.{js,jsx,ts,tsx}"
---

# GitHub Copilot React Instructions

## Framework & Styling

- Use **React functional components**.
- Styling should be done using **Tailwind CSS** utility classes.
- Avoid using class components or inline styles.

## Code Style

- Use **arrow functions** for all event handlers, mapping functions, and callbacks.
- Use **single quotes** for all JSX and JavaScript strings.
- Use **semicolons** at the end of each statement.
- Prefer **Hooks** (useState, useEffect, useContext) for logic reuse and state management.

## Best Practices

- Break components into smaller reusable pieces.
- Place reusable components under `/src/components`.
- Use prop types or TypeScript (if configured).
- Always handle loading and error states explicitly.
- Write clean, readable JSX with proper indentation (2 spaces).
