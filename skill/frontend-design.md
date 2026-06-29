# Frontend Design Skill

## Objective

Design interfaces that feel intentional, polished, and production-ready.

Every interface should prioritize clarity, usability, consistency, accessibility, and visual hierarchy. Avoid generic layouts and default framework aesthetics.

---

# Core Principles

- Design for users first, not for implementation convenience.
- Every visual decision should have a purpose.
- Simplicity is a feature. Remove unnecessary complexity.
- Consistency is more important than originality.
- Build interfaces as systems, not isolated pages.

---

# Visual Hierarchy

Guide the user's attention through deliberate use of:

- size
- spacing
- contrast
- alignment
- typography
- color
- motion

The most important content should always be immediately recognizable.

Avoid interfaces where every element has the same visual weight.

---

# Layout

Design layouts that feel balanced and predictable.

- Use consistent alignment.
- Respect a clear grid system.
- Maintain generous whitespace.
- Group related elements together.
- Separate unrelated content.

Never place elements randomly.

---

# Spacing

Use spacing to create rhythm.

- Follow a consistent spacing scale.
- Keep spacing consistent between similar components.
- Increase spacing to separate different content groups.
- Reduce spacing only for strongly related elements.

Whitespace is an active design element, not empty space.

---

# Typography

Typography should establish hierarchy before decoration.

- Use a consistent type scale.
- Differentiate headings, body text, captions and labels clearly.
- Prioritize readability over visual effects.
- Keep line lengths comfortable.
- Use font pairings only when they improve the overall design.

Never rely only on color to create hierarchy.

---

# Color

Colors should communicate meaning.

- Build a semantic color system.
- Primary colors represent actions.
- Neutral colors define structure.
- Accent colors draw attention intentionally.

Avoid decorative colors that do not reinforce the hierarchy.

---

# Components

Every component should belong to the same design language.

Ensure consistency across:

- spacing
- border radius
- shadows
- typography
- colors
- interaction patterns
- animation

Avoid creating one-off component styles.

---

# Depth

Create depth using hierarchy instead of decoration.

Prefer:

- spacing
- elevation
- shadows
- layering
- contrast

Avoid excessive visual effects.

---

# Images

Images should support the content.

- Use high-quality assets.
- Maintain consistent aspect ratios.
- Crop intentionally.
- Apply overlays only when they improve readability.
- Never stretch images.

---

# Motion

Motion should communicate, not entertain.

Animations should:

- reinforce hierarchy
- explain state changes
- improve perceived performance
- guide attention

Avoid decorative animations.

Whenever possible:

- animate only `transform` and `opacity`
- avoid layout-triggering animations
- use consistent durations and easing
- respect `prefers-reduced-motion`

---

# Interaction

Every interactive element should clearly communicate its state.

Support when appropriate:

- hover
- focus
- active
- disabled
- loading
- success
- error

Users should never wonder whether something is clickable.

---

# Responsive Design

Design mobile-first.

Layouts should adapt naturally across screen sizes.

Prioritize:

- flexible layouts
- CSS Grid
- Flexbox
- intrinsic sizing
- fluid spacing
- fluid typography

Avoid fixed-width layouts whenever possible.

---

# Forms

Forms should minimize user effort.

Always provide:

- visible labels
- helpful validation
- meaningful error messages
- loading feedback
- success feedback

Never rely only on placeholder text.

---

# Accessibility

Accessibility is part of the design process.

Ensure:

- sufficient color contrast
- visible focus indicators
- keyboard navigation
- semantic HTML
- accessible form controls
- reduced motion support

Accessibility is never optional.

---

# Performance

Visual quality should never reduce performance.

Prefer:

- lightweight components
- optimized images
- lazy loading
- efficient animations
- minimal dependencies

Design should remain smooth on low-end devices.

---

# Design System

Think in systems, not pages.

Before creating anything new:

- reuse existing components
- reuse design tokens
- reuse interaction patterns

If a pattern appears multiple times, promote it into the design system.

---

# Design Review Checklist

Before completing any UI task, verify:

- Clear visual hierarchy
- Consistent spacing
- Balanced layout
- Readable typography
- Cohesive color palette
- Consistent component styles
- Meaningful interactions
- Responsive behavior
- Accessibility
- Smooth performance
- No unnecessary visual noise

---

# Anti-Patterns

Avoid:

- Generic framework-looking interfaces.
- Inconsistent spacing.
- Arbitrary colors.
- Random border radii.
- Inconsistent shadows.
- Multiple competing focal points.
- Decorative animations.
- Fixed pixel layouts.
- Duplicate components.
- Poor accessibility.
- Visual clutter.
- One-off design decisions.