# 🌐 Smart Medicine Reminder System – Frontend

## 📌 Overview
This folder contains the **frontend (web application)** of the **Smart Medicine Reminder System**.  
The frontend provides a user-friendly interface for patients, caregivers, and doctors to manage medicine schedules, view reminders, and monitor adherence.

The application is built using **React + Vite**, which provides fast development, hot reloading, and a modern development experience.

---

## 🛠️ Tech Stack
- **React** – UI library for building components
- **Vite** – Fast development server and build tool
- **JavaScript (ES6+)**
- **HTML5 & CSS3**
- **ESLint** – Code quality and linting

(Styling libraries like Bootstrap or Tailwind can be added later.)

---

## 📁 Folder Structure
frontend/
│
├── public/ # Static assets
│
├── src/ # Application source code
│ ├── assets/ # Images, icons, media
│ ├── components/ # Reusable UI components
│ ├── pages/ # Page-level components
│ ├── services/ # API calls & backend communication
│ ├── hooks/ # Custom React hooks
│ ├── App.jsx # Root React component
│ └── main.jsx # Application entry point
│
├── index.html # Main HTML file
├── package.json # Project dependencies & scripts
├── package-lock.json # Dependency lock file
├── vite.config.js # Vite configuration
├── eslint.config.js # ESLint rules
└── README.md # Frontend documentation

## 🚀 Getting Started

### ✅ Prerequisites
Make sure you have the following installed:
- **Node.js (v18 or above recommended)**
- **npm** (comes with Node.js)
- **VS Code** (recommended editor)

# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Babel](https://babeljs.io/) (or [oxc](https://oxc.rs) when used in [rolldown-vite](https://vite.dev/guide/rolldown)) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## React Compiler

The React Compiler is enabled on this template. See [this documentation](https://react.dev/learn/react-compiler) for more information.

Note: This will impact Vite dev & build performances.

## Expanding the ESLint configuration

If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) for information on how to integrate TypeScript and [`typescript-eslint`](https://typescript-eslint.io) in your project.
