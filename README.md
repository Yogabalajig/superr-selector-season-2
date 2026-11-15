# SupeRR Selector — Pressure Performance Lab

Interactive dashboard for the SupeRR Selector Season 2 pressure-performance analysis.

## What is included
- Batter and bowler pressure-performance leaderboards
- Player-level evidence and comparison views
- Methodology, fairness, sensitivity and RR venue context
- A reproducible GitHub Pages deployment workflow

## Important methodology note
The rankings displayed are provisional prototype results for IPL and T20I from 2022 onward. They should be treated as a working analytical foundation pending final validation against the source ball-by-ball data and the challenge's final player-eligibility list. Availability, injury status and Rajasthan Royals role fitment are separate decision layers.

## Deployment
The dashboard source is stored as a compressed Base64-encoded gzip file at `dashboard.html.gz.b64`. The GitHub Actions workflow decompresses it into `index.html` and deploys that artifact to GitHub Pages whenever changes are pushed to `main`.

After the first successful workflow run, the dashboard should be available at:

https://yogabalajig.github.io/superr-selector-season-2/

## Update process
Replace `dashboard.html.gz.b64` with a newly gzip-compressed, Base64-encoded version of the dashboard HTML and push to `main`. The Pages workflow will rebuild and redeploy the site.
