# Accessibility Skill

## Objective

Build interfaces that are accessible, inclusive, and usable by everyone.

Accessibility is a core quality requirement—not an optional enhancement. Every feature should be fully usable regardless of a user's abilities, input method, or assistive technology.

---

# Accessibility Priorities

Always prioritize:

1. Semantic HTML
2. Keyboard accessibility
3. Screen reader support
4. Visual accessibility
5. Motion accessibility

Never sacrifice accessibility for visual design.

---

# Semantic HTML

Use native HTML elements whenever possible.

Prefer:

- `<header>`
- `<nav>`
- `<main>`
- `<section>`
- `<article>`
- `<aside>`
- `<footer>`
- `<button>`
- `<a>`
- `<form>`
- `<label>`

Avoid replacing semantic elements with generic `<div>` or `<span>` elements.

Native HTML is almost always more accessible than custom implementations.

---

# Keyboard Navigation

Every interactive element must be fully usable with a keyboard.

Ensure users can:

- Tab through interactive elements
- Activate controls using Enter or Space
- Close dialogs with Escape
- Navigate menus using arrow keys where appropriate

Never create keyboard traps.

Keyboard navigation should follow a logical order.

---

# Focus Management

Focus should always be visible and predictable.

Ensure:

- visible focus indicators
- logical tab order
- focus moves appropriately after user actions
- focus returns to the triggering element when closing dialogs

Never remove the browser's focus outline without providing an accessible replacement.

---

# Screen Readers

Content should make sense without visual context.

Ensure:

- meaningful page structure
- descriptive headings
- accessible labels
- meaningful link text
- appropriate announcements for dynamic content

Avoid redundant or misleading announcements.

---

# ARIA

Use ARIA only when native HTML cannot provide the required accessibility.

Prefer native semantics over ARIA whenever possible.

Ensure:

- accurate ARIA roles
- correct aria-label usage
- aria-labelledby where appropriate
- aria-describedby for supporting information
- aria-live for dynamic updates when needed

Avoid incorrect or unnecessary ARIA attributes.

No ARIA is better than bad ARIA.

---

# Forms

Forms should be easy to complete and understand.

Ensure:

- every field has a visible label
- labels are correctly associated with inputs
- required fields are clearly identified
- validation messages are descriptive
- errors are announced to assistive technologies
- users understand how to fix validation issues

Never rely solely on placeholder text.

Never communicate errors using color alone.

---

# Color and Contrast

Content should remain readable under all conditions.

Ensure sufficient contrast between:

- text and background
- interactive elements
- icons
- focus indicators

Never rely on color alone to communicate meaning.

Always provide additional visual cues.

---

# Images

Every image should have an appropriate purpose.

Use:

- descriptive alt text for informative images
- empty alt attributes (`alt=""`) for decorative images

Avoid repeating nearby text inside alt attributes.

---

# Interactive Components

Every interactive component should expose its current state.

Support when appropriate:

- hover
- focus
- active
- disabled
- expanded
- collapsed
- selected
- loading
- error

State changes should be perceivable by all users.

---

# Motion

Respect user motion preferences.

When `prefers-reduced-motion` is enabled:

- reduce animations
- disable parallax
- disable smooth scrolling
- avoid excessive movement

Motion should never interfere with usability.

---

# Responsive Accessibility

Accessibility applies across all devices.

Ensure:

- touch targets are sufficiently large
- text remains readable
- zoom up to 200% does not break layouts
- content remains usable on small screens

---

# Error Prevention

Help users avoid mistakes.

Provide:

- clear instructions
- meaningful defaults
- confirmation for destructive actions
- recoverable workflows

Never leave users without feedback.

---

# Accessibility Checklist

Before completing a feature, verify:

- Semantic HTML is used.
- Keyboard navigation works.
- Focus is visible and correctly managed.
- Screen readers receive meaningful information.
- Forms are fully accessible.
- Images have appropriate alt text.
- Color contrast is sufficient.
- Motion preferences are respected.
- Interactive states are communicated.
- No accessibility regressions have been introduced.

---

# Anti-Patterns

Avoid:

- Clickable `<div>` elements.
- Missing labels.
- Keyboard traps.
- Hidden focus indicators.
- Placeholder-only forms.
- Color-only feedback.
- Missing alt text.
- Incorrect ARIA attributes.
- Excessive animations.
- Poor contrast.
- Tiny touch targets.
- Inaccessible custom components.