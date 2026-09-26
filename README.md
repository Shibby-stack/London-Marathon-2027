# London Marathon 2027

Shihab's training project for the London Marathon on Sunday 25 April 2027, with Claude as running coach.

## What is in this repository

| Folder | What it holds |
|---|---|
| `site/road-to-the-mall.html` | The source of the private coaching site "Road to The Mall" (showreel, 30 week plan, run log, Ask Coach, lessons). |
| `data/strava-runs.csv` | A cleaned table of every run from the Strava export of 26 September 2026: date, name, distance, moving time, pace and cadence. |
| `data/run-log-seed.json` | The same runs in the format the site's run log uses. |
| `docs/coach-brief.md` | The coaching brief: athlete profile, baseline fitness, goals and plan outline. |
| `task/todo.md` | Plan checklist and review notes for this project. |
| `task/lessons.md` | Lessons learned, so the same mistakes are not repeated. |

## How the site works (plain English)

The site is one HTML file. HTML describes the page's content, the `<style>` block sets the look, and the `<script>` block is the program that runs in your browser. The code is commented section by section:

1. **Helpers**: small tools for dates and formatting times and paces.
2. **Plan data**: the 30 week plan written as a compact table, which the code expands into day by day sessions.
3. **Runs store**: where your logged runs are saved. On the live site they go into the site's own private database, so Claude can read them when coaching you.
4. **Views**: the code that draws the Today, Plan, Run log, Ask Coach and Learn tabs.
5. **Showreel**: the motion graphics intro, drawn frame by frame on a canvas and timed to a 120 BPM beat, plus a soundtrack generated live in the browser.
6. **Boot**: starts everything when the page opens.

The live site is published as a private Claude artifact. This file is the source kept under version control. The file on its own is a page body; Claude wraps it in the standard page skeleton when publishing.

## Updating

Ask Claude in the "London Marathon April 2027" project to change the site. Claude edits `site/road-to-the-mall.html`, republishes the artifact, and commits the change here.

## Privacy

The raw Strava export is deliberately **not** in this repository. It includes your email, contacts, followers and other personal data. Only the cleaned run table is kept. This repository also contains health information (injury history), so keep it **private** on GitHub.
