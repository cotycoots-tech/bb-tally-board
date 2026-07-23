# B&B Tally Board — Field Ops

Mobile-first web app for field crews to log human interventions on automated railway tie-plate systems.

## Features

- **Daily tally entry** for three categories: Robotic System, Tie Plate Setter, Truck Malfunction
- **Reason picker** (bottom sheet) with icons + persistent custom reasons
- **Unit selector**: Raiv-T1 / T-53, Raiv-T2 / T-57, Raiv-T3 / T-51
- **History log** with search and delete
- **Analytics dashboard** with date ranges, KPIs, trends, top reasons
- **Export to Excel** (Daily Summary + Reasons Log sheets)
- **Print report** for paper records
- Works offline after first load (data stored in browser localStorage)

## Live demo

After deploy, your Render / GitHub Pages URL will go here.

## Local use

Open `index.html` in any modern browser, or serve with:

```bash
npx serve .
# or
python3 -m http.server 8080
```

## Deploy to Render (Static Site)

1. Push this repo to GitHub
2. In [Render](https://dashboard.render.com) → **New → Static Site**
3. Connect the repo
4. Settings:
   - **Build Command**: leave empty
   - **Publish Directory**: `.` (root)
5. Deploy

Or use the included `render.yaml` with **Blueprint**.

## Deploy to GitHub Pages

1. Repo Settings → Pages
2. Source: Deploy from a branch → `main` / root
3. Save — site will be at `https://cotycoots-tech.github.io/bb-tally-board/`

## Data

All data stays in the browser (`localStorage`). Export to Excel or JSON for backup / sharing across devices.

## Tech

- Single-page HTML/JS/CSS
- Tailwind CSS (CDN)
- Chart.js, SheetJS, Font Awesome (CDN)

## License

Internal use — B&B Railway Solutions / Field Ops.
