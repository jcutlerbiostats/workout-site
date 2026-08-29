---
title: Workout Log System
---

A 5-day training split kept as plain-markdown notes in [Obsidian](https://obsidian.md), with structured inline fields so the numbers can be queried and charted.

## The split

Runs Tuesday → Monday: **Day 1** quads & calves · **Day 2** push · **Day 3** sprints · **Day 4** glutes · **Day 5** pull · two rest days.

## Templates

Static templates, one per day type. `{{DATE}}` is filled in by a script that generates a whole week at a time.

- [Day 1 — Quads & Calves](templates/workout_day_1)
- [Day 2 — Push](templates/workout_day_2)
- [Day 3 — Sprints](templates/workout_day_3)
- [Day 4 — Glutes](templates/workout_day_4)
- [Day 5 — Pull](templates/workout_day_5)
- [Rest Day 1](templates/rest_day_1) · [Rest Day 2](templates/rest_day_2)

## An example week

- [Tue — Day 1](example-week/2026-08-18-workout-day-1)
- [Wed — Day 2](example-week/2026-08-19-workout-day-2)
- [Thu — Day 3](example-week/2026-08-20-workout-day-3)
- [Fri — Day 4](example-week/2026-08-21-workout-day-4)
- [Sat — Day 5](example-week/2026-08-22-workout-day-5)
- [Sun — Rest](example-week/2026-08-23-rest-day-1) · [Mon — Rest](example-week/2026-08-24-rest-day-2)

## How the tracking works

Each exercise records two sets, followed by inline fields:

```
### Calf raises
- Set 1: 135 x 12
- Set 2: 135 x 10

calf_raises_wt:: 135
calf_raises_reps:: 12
```

The blank line before the inline fields matters — without it they attach to the list item instead of the page, and cross-page queries won't see them.
