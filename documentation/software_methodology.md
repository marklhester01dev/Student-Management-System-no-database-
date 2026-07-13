## Iterative/Incremental Methodology

This project follows an **Iterative/Incremental** approach: each roadmap phase is a working increment that builds on the one before it, is tested before moving on, and adds a complete piece of functionality rather than a partial slice of many features at once.

### Why This Fits the Project

- **Requirements were fixed up front.** The features, data fields, and system requirements were fully documented (`features.md`, `data.md`, `system_requirements.md`) before development started, so there's no need for a methodology built around shifting priorities.
- **Phases have real build-order dependencies.** Search, sorting, and filtering all depend on CRUD and the UI existing first. Web Components refactor the UI after it's functional. Dashboard statistics depend on records already being creatable and storable. Form validation hardens a form that already works. Each phase is only possible because the previous one is done — this is dependency-ordered delivery, not a pull-based backlog.
- **Solo build, single stream of work.** There's one person working on one increment at a time, so there's no need for WIP limits or a board to manage contention between parallel work streams.
- **Each increment is independently testable.** Per `testing.md`, QA happens per module/feature — this maps directly onto "finish an increment, verify it works, move to the next," rather than a continuously flowing, always-in-motion board.

### Workflow Summary

- **Planning/backlog approach:** Fixed backlog, defined in `roadmap.md`, ordered by technical dependency rather than shifting priority.
- **Iteration length:** One roadmap phase = one increment. No fixed time-box; a phase is complete when its feature works and is tested.
- **How progress is tracked:** Roadmap phase checklist (`roadmap.md`), 6 increments.
- **Testing approach:** Manual QA per increment before moving to the next phase (see `testing.md`), plus a final full pass across all features during UX polish.