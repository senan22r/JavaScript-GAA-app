# GAA Training Tracker

A lightweight JavaScript web app for tracking GAA training sessions, gym work, matches, and recovery days across the week. The app is built as a single-page HTML/CSS/JS dashboard and stores data in the browser using `localStorage`, making it easy to use without a backend or database.

## Features

- Weekly calendar view for the current training block
- Session logging for:
  - Gym
  - GAA training
  - Match
  - Recovery
- Effort rating slider from 1 to 5
- Optional notes for each session
- Daily and weekly load tracking
- Warning system highlighting risky load combinations and scheduling issues
- Edit and delete existing session entries
- Responsive dark-themed interface for quick use on desktop or tablet

## Project overview

This project is a single-file web app (`gaa-training-tracker (3).html`) with inline CSS and JavaScript. It lets a player or coach log training intensity and receive alerts when:

- heavy gym sessions are scheduled near match days
- hard training is placed before or after a match
- consecutive high-load days are detected

## How to run

Since this app is a static front-end project, there is no installation step required.

1. Download or clone the repository.
2. Open `gaa-training-tracker (3).html` in a browser.
3. Start logging sessions by selecting a date, type, effort rating, and optional note.

You can also serve it locally using a simple static file server if you prefer.

Example:

```bash
python -m http.server 8000
```

Then open:

```text
http://localhost:8000/gaa-training-tracker%20(3).html
```

## App behaviour

- Each session is stored in browser local storage under `gaa_sessions`.
- The calendar shows the current week and allows navigation between weeks.
- Each day displays a coloured status for load level:
  - Green: low / manageable load
  - Amber: moderate load
  - Red: high load
- Warning banners appear when the schedule suggests excessive fatigue or poor recovery planning.


