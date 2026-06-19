# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository nature

A collection of standalone HTML pages — no build system, no package manager, no tests. Each `.html` file is a self-contained mini-project with inline CSS and JS.

- `index.html` — landing page that links to the other pages; update this when adding a new page.
- `sports.html` — sports drink + gel calculator (single-file vanilla JS app).
- `feed-investigation.html` — slide-deck style presentation for EMGuidance content delivery.

## Working with the code

- View a page: open the file directly in a browser (`open sports.html` on macOS). There is no dev server.
- Edit-and-reload is the entire workflow — there is no transpilation step, so changes are visible on browser refresh.
- Keep each page self-contained: do not extract shared CSS/JS into separate files unless the user asks. The existing convention is one HTML file per project with everything inlined.
- When adding a new page, add a corresponding `<li><a>` entry to the `<ul>` in `index.html`.
