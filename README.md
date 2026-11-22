# Fiscal Fable CFO — Internal Workspace

A simple, no-AI, local-first internal app for the Fiscal Fable CFO team.

## Features
- Overview dashboard (clients, reports, pending/completed tasks)
- Client list with engagement model and notes
- Report creation, editing, saving, searching, and deletion
- Report templates aligned to the firm's corporate profile
- Print reports / Save as PDF via Android or desktop print dialog
- Basic task tracking with client assignment and deadlines
- Documents section links report history and describes file workflow
- Local storage only; no account system, cloud sync, AI, or external database

## Run
Open `index.html` in a modern browser. For more reliable browser storage, serve this folder locally (e.g. Python: `python -m http.server 8000`).

## Data
Data is saved in the browser's local storage. Clearing browser data may erase it. This build is a lightweight prototype and does not provide shared team sync or secure client file storage.

## Android APK
Android packaging and a GitHub Actions APK build workflow are included in this project. See `README-ANDROID.md`.
