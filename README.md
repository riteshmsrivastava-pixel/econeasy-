# Econeasy

An interactive microeconomics tutor — eleven chapters of animated, draggable graphs
with live worked examples and practice questions. Built for the MIT 15.024 sequence.

**Live site:** _enable GitHub Pages (see below) → `https://<your-username>.github.io/econeasy/`_

## Chapters

Markets & Demand → Supply & Demand · Elasticity · Consumer Choice
The Firm → Costs · Profit Max
Market Structure → Monopoly · Game Theory
Policy & Trade → Tax Incidence · Price Ceilings & Floors · Externalities · Trade

Every chapter has:

- **▶ Play** — auto-walks the scenarios so you can watch the graph move.
- **Drag** — grab a curve or point with the mouse and it moves live.
- **A worked example** — preset scenarios + editable numbers that recompute and drive the graph.
- **Practice questions** — real problems from the course, with step-by-step solutions you can reveal.

## Run it

It's a single self-contained page — no build step.

```bash
# any static server works, e.g.
python3 -m http.server 8099
# then open http://localhost:8099/
```

Just opening `index.html` from disk also works in most browsers (it loads React from a CDN at runtime).

## Files

- `index.html` — the whole app (a Claude Design Component; the runtime in `support.js` self-loads React and boots it).
- `support.js` — the Design Component runtime.

## Publish on GitHub Pages

1. Create a new repo on GitHub (e.g. `econeasy`) and push this folder to it.
2. In the repo: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, pick `main` / `/ (root)`, save.
3. Wait ~1 minute; your site is at `https://<your-username>.github.io/econeasy/`.
