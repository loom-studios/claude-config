
## Project Rules

- Always invoke the `frontend-design` skill before working on any UI, styling, layout, animation, or design-related task.
- Follow the existing architecture and conventions. Do not introduce new patterns unless clearly justified.
- Prefer modifying existing code over rewriting it.
- Reuse existing components before creating new ones.
- Keep solutions simple, maintainable, and consistent with the codebase.

---

## Skills

Use project skills whenever they are relevant to the current task.

Always consult the most appropriate skill before implementing features that involve architecture, UI, animations, performance, accessibility, SEO, or other specialized domains.

--- 

## Tech Stack

- React (functional components + Hooks)
- TypeScript (`strict: true`)
- Tailwind CSS
- CSS (only when Tailwind is insufficient)
- GSAP (complex animations)
- Lenis (smooth scrolling integrated with GSAP)

---

## Project Architecture

### Folder Structure

```
src/
├── app/
├── pages/
├── features/
├── components/
│   ├── ui/
│   ├── layout/
│   ├── feedback/
│   └── shared/
├── hooks/
├── providers/
├── contexts/
├── store/
├── lib/
├── assets/
├── styles/
├── constants/
├── config/
├── seo/
├── data/
├── types/
```

### Architectural Principles

- Co-locate code that changes together.
- `components/` contains reusable UI.
- `features/` contains domain-specific functionality.
- Keep `lib/` framework-agnostic.
- One component per file.
- Keep files small and focused.
- Prefer composition over inheritance.
- Avoid premature abstractions.

---

## Code Standards

- TypeScript `strict` is required.
- Avoid `any` unless absolutely unavoidable.
- Use meaningful names.
- One responsibility per component, hook, and function.
- Remove unused code instead of commenting it out.
- Explain **why**, not **what**, when writing comments.

---

## Local Development

- Always use the Vite development server.
- Never work from a `file:///` URL.
- Reuse an existing dev server when possible.
- Wait until the application is fully loaded before interacting with it.

---

## Browser Testing

Use Playwright to validate every frontend change.

Before completing a UI task, verify:

- layout
- responsive behavior
- interactions
- animations
- browser console
- visual regressions

Never assume a UI change is correct based only on reading the code.

---

## Brand Assets

Before creating or modifying any UI:

- Check the `brand_assets/` directory.
- Use existing logos, colors, typography, icons, and images.
- Never replace existing brand assets with placeholders.
- Follow the provided brand guidelines exactly.

---

## Reference Designs

If a design reference is provided:

- Match the layout, spacing, typography, colors, and proportions as closely as possible.
- Do not redesign or improve the reference unless explicitly requested.
- Use placeholder content only when real assets are unavailable.
- Validate the final result visually using Playwright.

---

## Decision Priorities

When multiple valid solutions exist, prioritize:

1. Correctness
2. Simplicity
3. Maintainability
4. Accessibility
5. Performance
6. Visual polish

---

## Definition of Done

A frontend task is complete only if:

- TypeScript reports no errors.
- ESLint passes.
- The UI has been verified in the browser.
- Responsive behavior has been tested.
- No console errors or warnings remain.
- Existing components and design tokens have been reused where appropriate.