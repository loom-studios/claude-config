# Performance Skill

## Objective

Build websites that feel instant, responsive, and efficient.

Performance is a feature, not an optimization step. Every implementation should minimize rendering cost, network usage, JavaScript execution, and layout instability.

Performance decisions should be made during development—not after the UI is finished.

---

# Performance Priorities

Always optimize in this order:

1. Loading performance
2. Rendering performance
3. Interaction responsiveness
4. Animation smoothness
5. Bundle size

Never sacrifice usability or accessibility purely for benchmark scores.

---

# Performance Targets

Aim for excellent real-world performance.

## Lighthouse

- Performance ≥ 95
- Accessibility ≥ 95
- Best Practices ≥ 95
- SEO ≥ 95

## Core Web Vitals

- LCP < 2.5s
- INP < 200ms
- CLS < 0.1

---

# JavaScript

JavaScript is the most expensive resource.

Always:

- Ship the smallest amount of JavaScript possible.
- Remove unnecessary dependencies.
- Prefer native browser APIs over external libraries.
- Load JavaScript only when required.
- Split large bundles into smaller chunks.

Avoid:

- Large utility libraries for simple operations.
- Duplicate dependencies.
- Unused code.
- Blocking the main thread.

---

# React Performance

Build components that render efficiently.

Prefer:

- component composition
- local state
- lazy loading
- code splitting

Avoid:

- unnecessary re-renders
- deeply nested component trees
- excessive prop drilling
- expensive computations during rendering

Only optimize with memoization when profiling demonstrates a real benefit.

---

# Images

Images are often the largest assets.

Always:

- serve correctly sized images
- use modern image formats
- reserve layout space
- lazy load below-the-fold images
- prioritize above-the-fold content

Never download images significantly larger than their rendered size.

---

# Fonts

Typography should load quickly.

Prefer:

- self-hosted fonts
- variable fonts when appropriate
- minimal font weights
- font subsetting
- non-blocking font loading

Avoid loading unused font families or weights.

---

# CSS

Keep CSS predictable and lightweight.

Prefer:

- reusable utilities
- design tokens
- simple selectors

Avoid:

- duplicated styles
- deeply nested selectors
- unnecessary overrides

---

# Animations

Animations should never reduce performance.

Animate only GPU-friendly properties whenever possible.

Prefer:

- transform
- opacity

Avoid animating layout or paint-heavy properties.

Keep interactions smooth and responsive.

Target 60 FPS.

---

# Network

Reduce unnecessary network requests.

Prefer:

- code splitting
- lazy loading
- route-based loading
- resource preloading only for critical assets

Avoid downloading resources before they are actually needed.

---

# Dependencies

Every dependency has a maintenance and performance cost.

Before adding one, verify:

- Is a native browser API sufficient?
- Can existing project utilities solve the problem?
- Is the library actively maintained?
- Is the bundle cost justified?

Prefer removing dependencies over adding them.

---

# Build Quality

Production builds should be optimized by default.

Ensure:

- tree shaking
- code splitting
- asset hashing
- minification
- compressed assets

---

# Performance Checklist

Before completing a task, verify:

- No unnecessary JavaScript has been introduced.
- No unnecessary dependencies have been added.
- Images are optimized.
- Fonts are optimized.
- Layout shifts are prevented.
- Components render efficiently.
- Animations remain smooth.
- Bundle size has not increased unnecessarily.
- Lighthouse performance remains high.

---

# Anti-Patterns

Avoid:

- Premature optimization.
- Loading everything on the first render.
- Large third-party libraries for trivial features.
- Duplicate code.
- Duplicate dependencies.
- Blocking the main thread.
- Layout thrashing.
- Unnecessary DOM updates.
- Heavy animations.
- Unoptimized images.
- Excessive network requests.