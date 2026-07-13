## Scope

- Implementation of CRUD in students management
- Storing data's using the Local Storage
- Export and backup of student records (CSV/JSON) to mitigate data loss
- Uses only HTML, CSS, and JS
- Focuses on creation of enrolled students
- Local Host only
- XSS Injection Prevention Using CSP Headers

## Limitations

- No databases used
- Data is stored only in the browser's localStorage. Clearing browser data/cache, using a different browser, or using a different device will still lose all records unless the user has exported a backup file beforehand
- Export/backup is manual — there is no automatic or scheduled backup; the user must actively trigger an export
- Restoring from a backup (import) is not guaranteed to merge cleanly with existing records; duplicate Student IDs between an imported file and existing data must be resolved manually
- Advanced Features (eg. enrollment projection chart, attendance checker, grade monitoring, student documents inventory) are not covered by this project.
- No server hosting
- No frameworks