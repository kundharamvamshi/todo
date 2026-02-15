# Todo App

A simple browser-based Todo application built with HTML, CSS, and vanilla JavaScript.

## Features

- Add new tasks
- Mark tasks as completed/incomplete
- Delete tasks
- Persist tasks in `localStorage`
- Restore saved tasks on page reload

## Tech Stack

- HTML5
- CSS3
- JavaScript (ES6)
- Bootstrap 4.5 (layout/utilities)
- Material Symbols (delete icon)

## How It Works

- Tasks are stored in an in-memory array called `todoList`.
- Clicking `Save` stores the current list in `localStorage` under the key `todoList`.
- On load, the app reads from `localStorage` and re-renders all tasks.
- Each task object contains:
  - `text`: task content
  - `uniqueNo`: numeric id used to build element ids
  - `isChecked`: completion status

## Run Locally

1. Clone or download this repository.
2. Open `index.html` in your browser.
3. Start adding your tasks.

## Project Structure

- `index.html` - App markup and CDN imports
- `styles.css` - App styles
- `script.js` - Todo logic, rendering, and persistence

## Notes

- This app does not auto-save after each action; click `Save` to persist changes.
- Data is stored per-browser using `localStorage`.
