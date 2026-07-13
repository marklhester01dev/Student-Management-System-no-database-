## Main User Flow

1. User opens `index.html` in a browser — the app loads any existing students from `localStorage` and displays them in the table, with dashboard stats reflecting the current count/breakdown.
2. User fills in the student form (Student ID, First Name, Middle Name, Last Name, Age, Sex, Section, Program, Year Level, Email Address, Contact Number).
3. User clicks **Add Student**. The form validates required fields, email format, contact number format, and checks for a duplicate Student ID.
   - If validation fails, an inline error is shown and the record is not saved.
   - If validation passes, the record is saved to `localStorage`, appears in the table, and the dashboard stats update.
4. User can select a row in the table to edit it — the form populates with that student's existing data.
5. User makes changes and clicks **Update Student** — the same validation rules apply, then the record and dashboard update.
6. User can select a row and delete it — a confirmation prompt appears before the record is removed from the table and from `localStorage`, and the dashboard updates.
7. At any point, the user can:
   - Type in the search bar to filter the table by Student ID, first name, last name, or course.
   - Use the sort controls to reorder the table by ID, name, course, or year level (ascending/descending).
   - Use the filter dropdowns to narrow the table by course, year level, or gender.
   - Clear search/filters to restore the full student list.
8. User refreshes the page — all data persists, loaded again from `localStorage`.

## Wireframes / Mockups

Not yet created. Recommend a low-fidelity sketch (paper, Figma, or Excalidraw) covering: the form, the table, the dashboard stat cards, and the delete-confirmation modal, before starting phase 3 of the roadmap (User Interface).