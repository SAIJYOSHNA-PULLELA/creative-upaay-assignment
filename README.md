# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) for information on how to integrate TypeScript and [`typescript-eslint`](https://typescript-eslint.io) in your project.





# Creative Upaay — Dashboard (Full Stack Assignment Level 1)

## Overview
A React dashboard that implements a 3-stage task board (To Do, In Progress, Done) with:
- Add Task (dynamic title and description)
- Move Tasks between columns (drag-and-drop)
- Filtering by text and priority
- State management with Redux Toolkit and persistence via Local Storage
- UI built with Chakra UI

## Tech
- React (Vite or CRA)
- Redux Toolkit, react-redux
- Chakra UI
- react-beautiful-dnd

## How to run
1. Install dependencies:
   npm install

2. Start dev server:
   npm run dev   (or npm start for CRA)

3. Open http://localhost:5173 (Vite) or http://localhost:3000 (CRA)

## Project structure
- src/
  - features/tasks/tasksSlice.js
  - components/
    - Board.jsx
    - Column.jsx
    - TaskCard.jsx
    - AddTaskModal.jsx
    - FilterBar.jsx
  - store.js
  - App.jsx
  - main.jsx

## Notes & assumptions
- Tasks contain `title`, `description`, `priority`, and `category`. You can extend fields easily.
- Other metadata (createdAt, dueDate) can be added; omitted for brevity.
- Drag-and-drop uses react-beautiful-dnd which gives natural UX and keyboard support.
- Local Storage key: `creative_upaay_state`. Clear browser storage to reset.

## Demo
Record a short video (e.g., Loom) showing:
- Adding a task in To Do
- Dragging it to In Progress and Done
- Filtering by keyword and priority
- Refreshing the page to show persistence

## Deployment
Deploy on Vercel / Netlify:
- Push to GitHub
- Connect repo to Vercel/Netlify and build with `npm run build`.
