# TaskFlow — React To-Do List Application with Authentication & Streaks

A modern, responsive, and minimalist To-Do List web application with user authentication and habit streaks built using **React 18** and **Vite**.

## ✨ Features

- **🔥 Habit Streaks**:
  - **Dynamic Consecutive Day Tracking**: Automatically detects consecutive daily task completions.
  - **Header Streak Pill**: Quick glance at your current streak count with glowing flame animation.
  - **Interactive Streak Dashboard**:
    - **Current & Best Streaks**: Displays current streak alongside your all-time personal record (🏆).
    - **7-Day Activity Grid**: Shows visual checkmarks for days you completed tasks and a pulsing indicator for today.
    - **Expandable Details**: Click anywhere on the streak card to toggle full week view.
  - **Celebration Feedback**: Motivational toasts celebrate new streak milestones when checking off tasks.
  - **Smart Break Detection**: Automatically detects missed days if tasks weren't completed.
- **🔐 User Authentication**:
  - **Sign In** and **Create Account** tabs with input validation.
  - **Instant Demo Login**: Jump right in with one click as `Alex Rivera` (with preloaded streak history).
  - **Show/Hide Password** toggle.
  - **Persistent Session**: Remembers the logged-in user in `localStorage`.
  - **Multi-Account Support**: Each user gets their own isolated to-do list and streak records.
  - **Header User Profile & Logout**: Shows user initials/name with one-click logout.
- **✅ Task Management**: Add, complete, inline-edit, and delete tasks.
- **⚡ Priority Levels**: Tag tasks with `High ⚡`, `Normal`, or `Low` priority.
- **🔍 Live Search & Status Filtering**: Real-time search by task name + filter tabs (**All**, **Active**, **Completed**).
- **✏️ Inline Editing**: Double-click any task title or click the pencil icon to edit in-place.
- **📊 Dynamic Progress Bar**: Visual tracker showing overall percentage of completed tasks.
- **🌓 Dark & Light Mode**: Seamless theme switching with automatic system theme detection and persistence (available on both the login screen and the main app).

---

## 🚀 Getting Started

### 1. Run Development Server
To launch the app with instant Hot Module Replacement (HMR):
```bash
npm run dev
```
Open the local URL displayed in your terminal (usually `http://localhost:5173`) in your browser.

### 2. Demo Credentials
You can log in instantly by clicking **"Continue with Demo Account"**, or use:
* **Email**: `alex@example.com`
* **Password**: `password123`

You can also switch to the **"Create Account"** tab to register any new account.

### 3. Build for Production
```bash
npm run build
```

---

## 📁 Project Structure

```text
├── index.html                  # Vite HTML entry point
├── package.json                # Project dependencies & scripts
├── vite.config.js              # Vite configuration
├── dist/                       # Optimized production build
└── src/
    ├── main.jsx                # React DOM root entry
    ├── App.jsx                 # App root with auth & streak state
    ├── App.css                 # Main app styles & header badges
    ├── index.css               # Global theme variables and resets
    └── components/
        ├── Login.jsx           # Sign in, Sign up, and Demo login component
        ├── Login.css           # Auth card styling and animations
        ├── StreakTracker.jsx   # Streak tracker & 7-day activity view
        └── StreakTracker.css   # Flame animations & streak styles
```
