# ClaudeStats

**▶ Open it live: https://friedsalad21.github.io/ClaudeStats/**

A personal Claude Code usage dashboard. Point it at your `.claude\projects` folder (or drag the folder onto the page) and it parses the transcript `.jsonl` files right in your browser. Nothing is uploaded.

What it shows:

- API-equivalent cost (what the usage would cost at Anthropic API list prices), total tokens split into input / output / cache read / cache write, API requests, sessions, prompts, active days, current and longest streak
- Cost and tokens over time, daily / weekly / monthly
- A GitHub-style year heatmap and an hour-of-day × weekday heatmap
- Breakdowns by model (donut), project and entrypoint, plus your most-used tools
- Cache hit rate and how much money caching saved
- The most expensive sessions, and a date range filter

The `.claude` folder is hidden on Windows: in the folder picker, paste `%USERPROFILE%\.claude` into the address bar and pick `projects`. The computed summary is cached in localStorage, so a reload doesn't need the folder again. There's also a "Load sample data" button with made-up data.

Single `index.html`, no build step; Chart.js from cdnjs.
