# Vibe Check Roulette — Standup Check-in Widget

A lightweight, embeddable HTML widget that generates random high/low check-in prompts for team standups. Spin the wheel and answer honestly — no coward answers allowed.

## What it does

- **Spin the wheel** — randomly picks a "high" (positive) or "low" (real talk) prompt
- **Just highs / Just lows** — filter by mood if you're feeling directional
- **Spin animation** — shuffles through emojis before landing on a prompt
- **History** — tracks your last 5 spins so you don't lose a good one

## Prompts

| Category | Count | Vibe |
|----------|-------|------|
| Highs | 12 | Wins, energy, hot takes, spirit animals |
| Lows | 12 | Frustrations, stress levels, battery drains |

## Usage

### Embed in Notion

1. Add an **Embed** block in your Notion page
2. Host the HTML file (e.g. via GitHub Pages, or paste into a service like [htmlbin](https://htmlbin.com))
3. Paste the URL into the embed block

### Standalone

Open `standup_high_low_checkin.html` directly in a browser. Note: the widget uses CSS custom properties (`var(--color-*)`) for theming, so colors will fall back to browser defaults outside a host app.

### GitHub Pages

1. Enable GitHub Pages on this repo (Settings > Pages > Source: `dev` branch)
2. Access at `https://<username>.github.io/standup-widget/standup_high_low_checkin.html`

## Design

- Zero dependencies — single HTML file with inline CSS and JS
- Uses CSS custom properties for theming, so it inherits the host app's color scheme (light/dark mode)
- No repeat logic prevents back-to-back duplicate prompts
- Responsive layout, max-width 540px
