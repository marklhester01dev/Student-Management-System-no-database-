## Functional Requirements

### Adding a Student

Fill in the student form using the data's from `data.md` and click **Add Student**. The form validates required fields, email format, contact number format, and checks for duplicate Student IDs before saving.

### Editing a Student

Select a student from the table to populate the form with their existing data, make changes, and click **Update Student** to save.

### Deleting a Student

Select a student and confirm the deletion prompt. The record is removed from the table and from `localStorage`.

### Searching, Sorting, and Filtering

- Use the search bar to find students by ID, first name, last name, or course.
- Use the sort controls to order the table by ID, name, course, or year level.
- Use the filter dropdowns to narrow the table by course, year level, or gender.

Clearing search/filters restores the full student list.

### Dashboard

The dashboard displays live counts: total students, total courses, and per-category breakdowns (year level, gender), recent student records. These update automatically whenever records are added, edited, or deleted.

## Data Storage

All student records are stored in the browser's `localStorage` under a dedicated key, as a JSON array of student objects. There is no server component — data is local to the browser/device it was entered on and will not sync across devices or browsers.

## Report Generation

Generate a downloadable CSV/JSON File specific for the requested data download from the user.

## Non-Functional Requirements

### Performance
Demonstrates fast update and retrieval of student informations, and capable to handle large chunks of informations necessary for the operations of the system.

### Browser Support
Supports modern browsers only

### Accessibility 
Covers parts that are essential for the users to know (eg. numbers of students, students informations, actions, and modals) that is readable by screen readers, particularly the NVDA Screen Reader, and be able to accommodate the mobile version of the system for the target users.

### Security
NFR4 (Security): The application enforces a Content-Security-Policy via a meta tag in `index.html` restricting scripts, styles, and objects to same-origin sources, to mitigate XSS from injected or malicious content (e.g. student names/fields containing script payloads).
