## Why This Exists

A browser-based CRUD application for managing student records — built with plain HTML, CSS, and JavaScript, using `localStorage` in place of a backend database.

This project is a practical exercise in building a complete, interactive CRUD app without relying on a server or database. It covers the full loop of creating, reading, updating, and deleting records, plus the supporting features (search, sort, filter, stats) that turn a basic form-and-table page into something that feels like a real admin tool — all persisted client-side.

## Objectives

*Concrete, checkable definitions of "done" for this project.*

- [ ] Full CRUD (Create, Read, Update, Delete) for student records, usable entirely through the UI
- [ ] All student data persists in `localStorage` and survives a page refresh with no data loss
- [ ] Search works across Student ID, first name, last name, and course
- [ ] Sort works on ID, name, course, and year level, in both ascending and descending order
- [ ] Filter works by course, year level, and gender, and can be cleared to restore the full list
- [ ] Dashboard shows live, accurate counts (total students, total courses, breakdowns by year level and gender) that update on every add/edit/delete
- [ ] Report Generation using CSV/JSON based on the requested files by the user.
- [ ] Form validation prevents invalid email/contact formats and duplicate Student IDs before a record is saved
- [ ] UI is built using JS Web Components (custom elements) rather than plain markup, per `tech_stack.md`
- [ ] No backend, build tools, or external dependencies are required to run the app

## What This Project Demonstrates

- CRUD operations in vanilla JavaScript
- Working with arrays and objects as an in-memory data layer
- DOM manipulation and event handling
- Form validation
- Persisting state with `localStorage`
- Implementing search, sort, and filter logic client-side
- Building a complete interactive web app without a backend