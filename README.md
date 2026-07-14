# 📋 Momentum Kanban Board

A modern, responsive, offline-first Kanban-style To-Do application built with pure HTML, CSS, and JavaScript. Designed for personal daily productivity with drag-and-drop task management, subtasks, progress tracking, dark mode, and local data persistence.

![Version](https://img.shields.io/badge/version-2.0.0-brightgreen
)
![License](https://img.shields.io/badge/License-MIT-green)
![HTML](https://img.shields.io/badge/HTML-5-orange)
![CSS](https://img.shields.io/badge/CSS-3-blue)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6-yellow)
---

## ✨ Features

### 🚀 What's New in Version 2.0
- **Multi-Selection & Playing-Card Fan Drag**: Hold `Ctrl` (`Cmd` on Mac) to select multiple tasks and drag them effortlessly without releasing the key. Dragged items display as a realistic hand of playing cards fanned out clockwise from the bottom-left corner with a `+N` stack indicator badge!
- **Custom Color-Coded Labels & Tag Filtering**: Create or select custom tags on the fly when adding/editing tasks. Filter your Kanban board instantly by tag using the new toolbar dropdown.
- **Board Insights & Analytics Dashboard**: Open the interactive analytics modal to view real-time productivity statistics, completion rates, and visual breakdowns by status, priority, and tags.
- **Card Cover Accents & Custom Color Highlights**: Choose vibrant cover color accents for individual task headers to organize and beautify your board.
- **Unified Custom UI Component Engine**: All native `<select>` dropdowns across the toolbar and task modal have been upgraded to sleek, animated custom overlay components with `MutationObserver` auto-sync.

---

### 📌 Task Management
- Create, edit and delete tasks
- Yet To Start, In Progress and Completed columns
- Drag & Drop between columns (Single and Multi-Card Fan Drag)
- Automatic task timestamps
- Due date support
- Priority levels (Low, Medium, High)
- Search tasks instantly
- Filter by Priority
- Filter by Status
- Filter by Custom Tags
- Sort by:
  - Created Date
  - Due Date
  - Priority
  - Manual Order

---

### ✅ Subtasks

Each task supports unlimited subtasks.

Features include:

- Add subtasks
- Remove subtasks
- Mark subtasks complete
- Live checklist
- Progress indicator
- Progress percentage

Example:

```
Website Redesign

☑ Create Homepage
☑ Design Dashboard
☐ Mobile Responsive
☐ Testing

Progress: 50%
```

---

### 📊 Progress Tracking

The application includes multiple progress indicators.

### Task Progress

Each task displays:

- Completed subtasks
- Remaining subtasks
- Progress bar
- Percentage completed

Example

```
3 / 5 Completed

██████████░░░░░

60%
```

### Overall Dashboard Progress

Displays:

- Total Tasks
- Yet To Start Tasks
- In Progress Tasks
- Completed Tasks
- Completion Percentage

Example

```
Total Tasks : 20

Completed : 15

Overall Progress

██████████████████░░

75%
```

---

### 📦 Completed Information

Whenever a task is moved into **Completed**, the application records:

- Completed By
- Completed Date
- Completed Time

These values remain permanently attached to the task.

---

### 📂 Archive

- Archive completed tasks
- Restore archived tasks
- Permanent storage

---

### 💾 Offline Storage

Everything works locally.

No:

- Database
- Backend
- Login
- Internet

Data is stored using:

- LocalStorage

All changes are automatically saved.

---
<style>
  .alert-info {
    color: #0c5460;
    background-color: #d1ecf1;
    border-color: #bee5eb;
}
.alert {
    position: relative;
    padding: .75rem 1.25rem;
    margin-bottom: 1rem;
    border: 1px solid transparent;
    border-radius: .25rem;
}
</style>

### 🔄️ Github Sync (Optional)

You can configure Github Sync if you wanna sync your board across multiple systems.

Provide following details in the sync settings
1. Repo owner - Your Github account name - e.g. **shandeepc**
2. Repository - The name of the repository where you wish to store your board e.g. **Momentum-Storage**

    <div class="alert alert-info" style="width:880px">
    <svg height="20px" class="svg-inline--fa fa-info-circle fa-w-16" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="info-circle" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" data-fa-i2svg=""><path fill="currentColor" d="M256 8C119.043 8 8 119.083 8 256c0 136.997 111.043 248 248 248s248-111.003 248-248C504 119.083 392.957 8 256 8zm0 110c23.196 0 42 18.804 42 42s-18.804 42-42 42-42-18.804-42-42 18.804-42 42-42zm56 254c0 6.627-5.373 12-12 12h-88c-6.627 0-12-5.373-12-12v-24c0-6.627 5.373-12 12-12h12v-64h-12c-6.627 0-12-5.373-12-12v-24c0-6.627 5.373-12 12-12h64c6.627 0 12 5.373 12 12v100h12c6.627 0 12 5.373 12 12v24z"></path></svg>
    <strong>Note:</strong>Make sure this repository is<strong>private</strong>, if not any one can view your borad if they vist this repository in Github
  </div>

3. Branch - Name of git branch, you can leave it as default which is **main**
4. File path - Json file path of the board in your repo, you can leave it as default which is **data/momentum-board.json**
5. Personal access token - **Create one at github.com** → **Settings** → **Developer settings** → **Personal access tokens** → **Fine-grained tokens**.

    <div class="alert alert-info" style="width:880px">
    <svg height="20px" class="svg-inline--fa fa-info-circle fa-w-16" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="info-circle" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" data-fa-i2svg=""><path fill="currentColor" d="M256 8C119.043 8 8 119.083 8 256c0 136.997 111.043 248 248 248s248-111.003 248-248C504 119.083 392.957 8 256 8zm0 110c23.196 0 42 18.804 42 42s-18.804 42-42 42-42-18.804-42-42 18.804-42 42-42zm56 254c0 6.627-5.373 12-12 12h-88c-6.627 0-12-5.373-12-12v-24c0-6.627 5.373-12 12-12h12v-64h-12c-6.627 0-12-5.373-12-12v-24c0-6.627 5.373-12 12-12h64c6.627 0 12 5.373 12 12v100h12c6.627 0 12 5.373 12 12v24z"></path></svg>
    <strong>Note:</strong><bold>Use a fine-grained personal access token</strong> scoped to only this one repo, with only "Contents" read/write permission. It's stored solely in this browser - never written into the synced file itself. If this repo is public, anyone can read the synced file once it's pushed, even though only token-holders can write to it.
  </div>

Click **Save & Sync now**

All changes are automatically saved and synced to your github repo.

---

### 📤 Import / Export

Export all tasks as JSON.

Import tasks back at any time.

Perfect for backups.

---

### 🎨 Themes

Supports

- ☀ Light Mode
- 🌙 Dark Mode

Theme preference is remembered.

---

### 📱 Responsive Design

Works on

- Desktop
- Laptop
- Tablet
- Mobile

---

### ⌨ Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| N | New Task |
| / | Search |
| Ctrl + E | Export Tasks |
| Ctrl + Left Click | Select Multiple |
| T | Toggle Theme |
| Esc | Close Dialog |
| ? | Help |

---

## 🚀 Getting Started

### Visit https://momentum.shandeep.dev

---

## 🛠 Technologies Used

- HTML5
- CSS3
- Vanilla JavaScript (ES6)
- LocalStorage API

---

## 📸 Features Overview

✔ Multi-Selection & Playing-Card Fan Drag

✔ Custom Tags & Color-Coded Labels

✔ Board Insights & Analytics Dashboard

✔ Card Cover Accents & Highlights

✔ Custom UI Dropdown Engine

✔ Drag & Drop

✔ Kanban Board

✔ Subtasks

✔ Progress Bars

✔ Overall Progress Percentage

✔ Search

✔ Filters

✔ Sorting

✔ Archive

✔ JSON Export

✔ JSON Import

✔ Dark Theme

✔ Responsive Layout

✔ Offline Ready

✔ Github Sync

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 👨‍💻 Author

**Shandeep Srinivas**

IAM Consultant | SailPoint IdentityIQ Developer | Saviynt Engineer

GitHub:
https://github.com/shandeepc

LinkedIn:
https://www.linkedin.com/in/shandeepc

---

⭐ If you found this project useful, consider giving it a Star on GitHub!
