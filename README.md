# CCR Gala Planner

Project management web app for planning the **CEMS Club Rotterdam (CCR) Gala** — a black-tie student event on **Thursday 3 December 2026**. Planning runs for 11 weeks, from Monday 28 September to Sunday 13 December 2026 (post-event wrap-up included).

The whole app is one file, [`index.html`](index.html): HTML, CSS and vanilla JavaScript. There's no build step and nothing to install.

## Features

- **Dashboard**: overall progress, a live countdown to the gala, overdue tasks, the next milestone, progress per phase, workload per person and what's due in the next 14 days.
- **Timeline**: a Gantt chart by week with milestones (◆), a red "today" line and a gold line for gala night. You can filter it by person or phase and hide completed tasks.
- **Tasks**: tasks grouped into seven phases (Planning & Budget, Venue & Logistics, Partners & Sponsors, Marketing & Tickets, Programme & Guests, Event Week, Post-Event), with search and filters.
- **Status tracking**: click a status to cycle it through Not Started → In Progress → Complete.
- **Team**: board members (President, Treasurer, Head of Social, Head of Corporate, Head of Marketing, Head of Alumni, Head of CSR) with each person's workload. You can add, edit and delete people.
- **Add / edit / delete tasks**. Deleting a task or person can be undone from the toast message.
- **Saved automatically** in the browser (localStorage). From the Team tab you can export and import a JSON backup, or reset to the sample plan.
- Navy and gold design that also works on phones.

## Hosting on GitHub Pages

1. Push this repository to GitHub.
2. Go to **Settings → Pages**, set **Source** to *Deploy from a branch*, then pick the branch and the `/ (root)` folder.
3. The planner will be live at `https://<user>.github.io/<repo>/`.

To run it locally, just open `index.html` in a browser.

## Notes

- Data lives in each visitor's own browser, so board members don't see each other's changes automatically. To share the latest plan, use **Export backup** and **Import backup** on the Team tab.
- To preview the planner as if it were another date, add `?today=YYYY-MM-DD` to the URL, e.g. `index.html?today=2026-11-10`.
