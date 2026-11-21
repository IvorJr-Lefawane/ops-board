# Ops Board

A single-page task and study dashboard: one queue for school and cyber work, built as one self-contained `index.html` (no build step, no dependencies).

## Features

- **Exam week panel** pinned to the top, sorted by date with a countdown and a Start/Done button per exam
- **Kanban board** (To do / In progress / Done) with drag-and-drop on desktop and tabs on mobile
- **Grouped by module** so you finish one assignment before starting the next
- **Today panel**: classes, anything due or overdue, and what's in progress
- **Urgency colours** from overdue through to later, plus module colour chips
- **Weekly timetable** with open-task counts per module
- Dark mode, responsive layout, and a "first step" starter on each task

## Run it

Open `index.html` in a browser. That's it.

Tasks are saved in your browser's local storage, so each device keeps its own board.

## Deploy with GitHub Pages

1. Push this repo to GitHub.
2. Go to **Settings → Pages**.
3. Set the source to **Deploy from a branch**, then choose `main` and `/ (root)`.
4. Your site goes live at `https://<your-username>.github.io/<repo-name>/`.

## Task fields

`title`, `area` (school | cyber), `tag` (module code or cert), `due` (YYYY-MM-DD), `priority` (high | med | low), `status` (todo | doing | done), `notes`, `first` (5-minute starter).

## Notes

- Exams are detected by the word "Exam" in the task title.
- Module colours are set in the `MODCLS` and `MODORDER` constants in `index.html`.
