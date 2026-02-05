# 📝 To-Do List Manager (Pro)

A sleek, high-performance task management web application. This tool is designed for productivity, featuring a "Local First" architecture where all your data stays privately in your browser's local storage.

---

## ✨ Key Features

* **Advanced Task Metadata:** Support for titles, detailed notes, priority levels (Low, Medium, High), due dates, and custom tags.
* **Dynamic Filtering:** Filter tasks by completion status, priority, due date windows (Today, This Week, Overdue), or specific tags.
* **Powerful Search & Sort:** Real-time search across titles/notes and multiple sorting options.
* **Bulk Actions:** Select multiple tasks to complete or delete them simultaneously.
* **Data Portability:** Integrated **Export/Import JSON** functionality to backup your data.
* **Responsive Design:** Optimized for both desktop and mobile with a modern dark theme.

---

## 🚀 Quick Start

1.  **Save the code** as an `index.html` file.
2.  **Open the file** in any modern web browser.
3.  **Start Adding Tasks:** Use the top bar to quickly add a task, or use the "Edit" button to add notes and tags.

---

## ⌨️ Keyboard Shortcuts

| Key | Action |
| :--- | :--- |
| `/` | Focus the Search bar |
| `Enter` | Submit a new task (from title input) |
| `C` | Mark selected tasks as **Complete** |
| `E` | **Edit** the selected task |
| `Delete` | **Remove** selected tasks |

---

## 🛠️ Technical Overview

The application follows a standard **Model-View-Controller (MVC)** pattern implemented in vanilla JavaScript:



* **Storage:** Uses the `localStorage` API for persistence.
* **Styling:** Custom CSS variables (`:root`) for easy theme tweaking.
* **No Dependencies:** No React, Vue, or Tailwind required—just pure web standards.

### Data Schema
The app handles data in the following JSON structure:

```json
{
  "tasks": [
    {
      "id": "t_k9z2x...",
      "title": "Example Task",
      "notes": "Task details",
      "due": "2026-02-05",
      "priority": "High",
      "tags": ["work"],
      "done": false
    }
  ]
}
