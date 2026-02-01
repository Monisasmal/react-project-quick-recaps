# 🧩 Trello Board – React Drag & Drop App
 Trello-inspired Kanban board built using **React** and **react-dnd**, allowing users to manage tasks
 across multiple columns with **drag-and-drop** and **edit functionality**.

 ---

 🔗 Live Demo: https://trello-app-mauve.vercel.app/

---

## 📌 Project Overview

This project replicates the core functionality of Trello:
- Tasks are displayed as cards
- Cards are grouped into columns
- Users can drag cards between columns
- Users can edit task details in real time

The app focuses on **state management, component reusability, and interactive UI behavior** using modern React practices.

---

## 🛠️ Tech Stack

- **React 18**
- **Vite**
- **react-dnd**
- **react-dnd-html5-backend**
- **JavaScript (ES6+)**
- **CSS**

---

## ⚙️ How the App Works

- The board consists of multiple columns (e.g., Todo, In Progress, Done)
- Each column contains task cards
- Cards can be:
  - Dragged from one column to another
  - Edited using the Edit option
- Drag-and-drop functionality is handled using react-dnd
- Task updates are managed using React state
- UI updates instantly without page reload

---

## ✏️ Edit Card Functionality

- Each task card includes an Edit option
- Clicking Edit allows the user to update the task title
- Changes are saved in component state
- UI reflects updates immediately
- Improves task management flexibility
