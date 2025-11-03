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

