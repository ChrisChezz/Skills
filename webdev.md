---
name: senior-web-developer
description: Expert-level guide for full-stack web development, focusing on performance, accessibility, and modern standards.
---

# Web Development Rules & Standards

## 1. Frontend Philosophy
- **Semantic HTML:** Always use proper elements (`<header>`, `<main>`, `<section>`, `<article>`, `<footer>`) instead of just `<div>`.
- **Accessibility (A11y):** All interactive elements must be keyboard-accessible. Use `aria-labels` where visual text is missing.
- **Performance:** - Always suggest lazy-loading for images and heavy components.
    - Keep CSS bundles lean; prioritize utility-first or modular CSS.
- **Responsiveness:** Use mobile-first CSS media queries. 

## 2. JavaScript/TypeScript Best Practices
- **Modern ES6+:** Use `const` and `let` over `var`. Prefer arrow functions and destructuring.
- **Type Safety:** If using TypeScript, define strict interfaces for props and API responses.
- **Error Handling:** Every `fetch` or async operation must be wrapped in `try/catch` with meaningful user-facing error messages.
- **Component Design:** Keep components small (single responsibility). Logic should be separated from presentation.

## 3. Security Requirements
- **Input Sanitization:** Never trust user input. Sanitize all data before rendering or sending to a database.
- **Environment Variables:** Never hardcode API keys or database strings. Use `.env` files.
- **Dependencies:** Regularly check for and update deprecated packages.

## 4. Workflow Rules
- **Documentation:** Every major function must have a JSDoc block explaining parameters and return values.
- **Testing:** Propose unit tests (Jest/Vitest) for complex business logic.
- **Clean Code:** Follow the "DRY" (Don't Repeat Yourself) principle. If you see repeated logic, suggest a helper function or a custom hook.
