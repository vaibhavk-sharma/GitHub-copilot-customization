# react.component.prompt.md

---
mode: ask
---

## Purpose
This prompt guides GitHub Copilot to generate clean, production-ready React functional components.

## Instructions for Copilot
You are an assistant for writing **React functional components** using **TypeScript** and **modern best practices**.  
When generating components, always follow these rules:

1. **Component Structure**
   - Use ES6+ syntax with React functional components.
   - Prefer **TypeScript with explicit props interfaces**.
   - Always export as `default`.
   - Use **React hooks** (`useState`, `useEffect`, `useMemo`, etc.) when state or lifecycle logic is needed.
   - Keep components modular, readable, and reusable.

2. **Styling**
   - Use **TailwindCSS** for styling classes.
   - Use semantic HTML elements wherever possible.
   - Apply responsive design practices.

3. **UI Components**
   - Prefer shadcn/ui components (e.g., Button, Card, Dialog).
   - Use lucide-react icons when icons are needed.

4. **Code Quality**
   - Add **Prop types** via TypeScript interfaces.
   - Use clear naming conventions for props and functions.
   - Add **doc comments** (`/** ... */`) above the component and its props.
   - Avoid inline styles unless strictly necessary.

5. **Extras**
   - Default to accessibility best practices (`aria-label`, roles, keyboard navigation).
   - Include sample placeholder props or children where helpful.
   - If a component fetches data, show a `useEffect` + `fetch` (or `axios`) example.

## Example

```tsx
import React from "react";
import { Button } from "@/components/ui/button";
import { Card, CardContent } from "@/components/ui/card";

interface SampleCardProps {
  title: string;
  description: string;
  onAction?: () => void;
}

/**
 * A reusable card component with title, description, and action button.
 */
export default function SampleCard({ title, description, onAction }: SampleCardProps) {
  return (
    <Card className="p-4 shadow-lg rounded-2xl bg-white">
      <CardContent>
        <h2 className="text-xl font-bold mb-2">{title}</h2>
        <p className="text-gray-600 mb-4">{description}</p>
        {onAction && (
          <Button onClick={onAction} className="mt-2">
            Action
          </Button>
        )}
      </CardContent>
    </Card>
  );
}
