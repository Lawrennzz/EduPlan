## EduPlan

### Scenario
In the fast-paced academic environment, university students juggle multiple responsibilities, including assignments, discussions, club activities, and examinations. To effectively manage their time and prioritize their tasks, a well-structured To-Do List web application is required as an assistant to the students. This assignment requires you to develop a web application that is tailored to university students with the maximum number of web pages between 10–15 pages. Note that a pop-up dialog box is not considered a web page.

### Features
- **Task Recording**: Users can add tasks such as assignments, discussions, club activities, and examinations. Each task includes title, description, due date, and category.
- **Task Monitoring**: Users can view all tasks in a structured way with filtering options that allow sorting by category, priority, or due date.
- **Task Status Management**: Tasks can be marked as "On-going," "Pending," or "Completed."
- **Task Archiving**: Completed tasks are moved to an archive instead of being permanently deleted, and users can revisit archived tasks if necessary.
- **Task Prioritization**: Tasks can be assigned priority levels such as "High," "Medium," or "Low" to help students focus on urgent tasks first.
- **Reminder System**: Notifies students of approaching deadlines; users can set custom notifications based on their preferences.

---

## Current Project Contents (IndividualAssignment)

This repository contains the `IndividualAssignment` web app (PHP + JS + CSS). Below is the current folder structure to help you navigate the codebase:

``` 
IndividualAssignment/
  add_task.php
  ajax_handlers/
    bulk_task_action.php
    get_task_details.php
    task_action.php
  archive.php
  calendar.php
  dashboard.php
  database.sql
  edit_task.php
  forgot_password.php
  images/
    education.png
    student.jpg
  includes/
    archive_task.php
    captcha_svg.php
    check_tasks_structure.php
    db_connect.php
    delete_task.php
    export.php
    fonts/
      arial.ttf
    get_task.php
    login_process.php
    register_process.php
    reminder.php
    restore_task.php
    security_functions.php
    send_reminders.php
  index.php
  js/
    add_task.js
    archive.js
    auth.js
    calendar.js
    dashboard.js
    edit_task.js
    forgot_password.js
    landing.js
    libraries/
    profile.js
    reminders.js
    reports.js
    script.js
    sort.js
    tasks.js
  learn_more.php
  login.php
  logout.php
  profile.php
  register.php
  reminders.php
  reports.php
  styles/
    add_task.css
    archive.css
    auth.css
    calendar.css
    dashboard.css
    edit_task.css
    forgot_password.css
    landing.css
    notifications.css
    profile-styles.css
    reminders.css
    reports.css
    tasks.css
  tasks.php
```

### Key Pages and Scripts
- **Authentication**: `login.php`, `logout.php`, `register.php`, `includes/login_process.php`, `includes/register_process.php`, `js/auth.js`
- **Tasks**: `index.php`, `tasks.php`, `add_task.php`, `edit_task.php`, `archive.php`, `includes/archive_task.php`, `includes/restore_task.php`, `includes/delete_task.php`, `ajax_handlers/*`, `js/tasks.js`, `js/add_task.js`, `js/sort.js`, `js/archive.js`
- **Calendar**: `calendar.php`, `js/calendar.js`
- **Reminders**: `reminders.php`, `includes/reminder.php`, `includes/send_reminders.php`, `js/reminders.js`
- **Reports**: `reports.php`, `includes/export.php`, `js/reports.js`
- **Profile**: `profile.php`, `js/profile.js`
- **Dashboard**: `dashboard.php`, `js/dashboard.js`
- **Security/Utilities**: `includes/security_functions.php`, `includes/check_tasks_structure.php`, `includes/captcha_svg.php`

### Database
- SQL schema and sample data: `IndividualAssignment/database.sql`
- Connection settings: `IndividualAssignment/includes/db_connect.php`

### Local Setup
1. Import `IndividualAssignment/database.sql` into your MySQL/MariaDB server.
2. Update `IndividualAssignment/includes/db_connect.php` with your DB host, user, password, and database name.
3. Serve the folder via your PHP server (e.g., XAMPP `htdocs/IndividualAssignment`).

### Notes
- Server-side is plain PHP, client-side is vanilla JS/CSS, no external frameworks.
- All pages are interlinked; footer should state the business is fictitious for coursework.
- Media from external sources must include references.

---

## Detailed Specification (EduPlan - Student Task Management Platform)

### Project Overview
EduPlan is a PHP-based task management web application tailored for university students. It helps students record tasks, organize by categories and priority, monitor progress, archive completed items, and receive reminders for upcoming deadlines.

### Project Features (Detailed)
1. **User Authentication & Security**
   - Login/logout pages for users.
   - Basic auth handling and CAPTCHA support.
   - Files: `login.php`, `logout.php`, `register.php`, `includes/login_process.php`, `includes/register_process.php`, `includes/captcha_svg.php`, `js/auth.js`.

2. **Task Recording & Specification**
   - Add tasks with title, description, due date, category, and priority.
   - Files: `add_task.php`, `js/add_task.js`, `includes/get_task.php`.

3. **Task Monitoring & Filtering**
   - View tasks with filters (category, priority, due date) and sorting.
   - Files: `index.php`, `tasks.php`, `js/tasks.js`, `js/sort.js`, `js/script.js`.

4. **Task Status Management**
   - Mark tasks as On-going / Pending / Completed.
   - Files: `ajax_handlers/task_action.php`, `js/tasks.js`.

5. **Task Archiving & Restore**
   - Archive completed tasks; restore when needed.
   - Files: `archive.php`, `includes/archive_task.php`, `includes/restore_task.php`, `js/archive.js`.

6. **Reminders & Notifications**
   - Reminder scheduling and sending.
   - Files: `reminders.php`, `includes/reminder.php`, `includes/send_reminders.php`, `js/reminders.js`.

7. **Calendar View**
   - Calendar visualization of upcoming tasks/due dates.
   - Files: `calendar.php`, `js/calendar.js`.

8. **Reports & Export**
   - Basic reports and data export.
   - Files: `reports.php`, `includes/export.php`, `js/reports.js`.

9. **Dashboard & Profile**
   - High-level overview and profile management pages.
   - Files: `dashboard.php`, `profile.php`, `js/dashboard.js`, `js/profile.js`.

10. **Security & Utilities**
   - Security helpers, structure checks, and auxiliary endpoints.
   - Files: `includes/security_functions.php`, `includes/check_tasks_structure.php`, `includes/captcha_svg.php`, `ajax_handlers/*`.

### Development Requirements
- Technologies: HTML, CSS, JavaScript, PHP (XHTML/HTML5 permitted).
- Programming elements: variables, constants, conditionals, loops, functions, arrays (1D and multidimensional), string handling, files, directories, and object-oriented concepts where suitable.
- Database: MySQL/MariaDB via SQL scripts in `IndividualAssignment/database.sql`.
- Server-side: PHP only; no external frameworks or code generators.
- Media Attribution: Include references for any external media used.
- Footer Requirement: Each page should include a footer indicating the business is fictitious and part of a university course.
- Navigation: All pages should be linked together.

### How the repository maps to the features
- Authentication: `login.php`, `logout.php`, `register.php`, `includes/login_process.php`, `includes/register_process.php`, `js/auth.js`.
- Tasks: `index.php`, `tasks.php`, `add_task.php`, `edit_task.php`, `ajax_handlers/*`, `js/tasks.js`, `js/add_task.js`, `js/sort.js`.
- Archive/Restore: `archive.php`, `includes/archive_task.php`, `includes/restore_task.php`, `js/archive.js`.
- Calendar: `calendar.php`, `js/calendar.js`.
- Reminders: `reminders.php`, `includes/reminder.php`, `includes/send_reminders.php`, `js/reminders.js`.
- Reports/Export: `reports.php`, `includes/export.php`, `js/reports.js`.
- Dashboard/Profile: `dashboard.php`, `profile.php`, `js/dashboard.js`, `js/profile.js`.
- Security/Utilities: `includes/security_functions.php`, `includes/check_tasks_structure.php`, `includes/captcha_svg.php`.

### Prerequisites
- XAMPP (Apache + PHP + MySQL/MariaDB) or similar stack
- PHP 8.x recommended

### Setup
1. Clone the repository and place `IndividualAssignment/` under your web root, e.g., `htdocs/IndividualAssignment`.
2. Create database and import SQL:
   - Import: `IndividualAssignment/database.sql`.
3. Configure database connection:
   - Edit `IndividualAssignment/includes/db_connect.php` with your host, username, password, and database name.
4. Launch the app:
   - Visit `http://localhost/IndividualAssignment/`.

### Development Guidelines
- Use plain PHP for server logic; vanilla JS/CSS on the client.
- Prefer clear variable/function names; keep code modular (e.g., helpers in `includes/`).
- Keep large binary assets out of version control when possible; include small representative samples instead.
- Ensure all pages include the required academic footer note.

### Reporting and Analytics
- Task data can be exported via `includes/export.php` and viewed via `reports.php`.
- Extend reporting by adding SQL queries/procedures and corresponding UI in `reports.php` and `js/reports.js`.

### Credits & Attribution
- Provide references for any external media (images/icons/etc.).

### License / Usage
- For academic purposes and coursework demonstrations; review your institution’s policies before reuse.

