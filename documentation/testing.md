## Approach

Manual QA and per-module testing, performed at the end of each roadmap phase (see `software_methodology.md`), plus a final full pass across all features during UX polish.

## What Gets Tested

- All CRUD functions (add, edit, delete, view) work correctly and persist to `localStorage`
- Search, sort, and filter behave correctly individually and in combination, and can be cleared to restore the full list
- Dashboard counts update correctly after every add, edit, and delete
- Form validation catches required-field, email-format, contact-number-format, and duplicate-Student-ID errors before save
- All user actions (buttons, modals, confirmations) are understandable and behave as expected
- Accessibility: key content (student counts, student information, actions, and modals) is readable by screen readers, particularly NVDA, and the layout works on mobile
- When a later increment touches logic shared with an earlier one (e.g. Increment 4 adding Local Storage persistence and Dashboard Statistics on top of the CRUD and Search/Sort/Filter logic from Increments 2–3), earlier features are re-verified rather than assumed still correct
- CSP is present and correctly blocks inline scripts/styles; verify via browser DevTools console (CSP violations log there) and by attempting to inject a script tag through a student field (e.g. Name = `<script>alert(1)</script>`) to confirm it renders as inert text, not executable code

## Tools

- Chrome DevTools
- NVDA Screen Reader
