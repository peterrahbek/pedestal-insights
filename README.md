# Pedestal · Insights

Private hub for Pedestal dashboards & data drops — served at **insights.pedestal.com**.

Each item lives in its own folder and is reachable **only by its direct link**:
nothing is listed on the landing page, and the whole site is `noindex` +
robots-disallowed.

## Contents
- `/us-demand/` — US market opportunity (24-month session demand; shared with the US partner)

## Add a new drop
1. Create a new folder at the repo root, e.g. `/my-topic/`, with an `index.html`.
2. Keep `<meta name="robots" content="noindex">` in the page `<head>`.
3. `git commit` + `git push` — live at `insights.pedestal.com/my-topic/` in ~30s.

## Hosting
GitHub Pages, custom domain `insights.pedestal.com` (CNAME at Abion → `peterrahbek.github.io`).
The standalone US page also still lives at its original GitHub Pages URL — this hub is the
canonical home going forward.
