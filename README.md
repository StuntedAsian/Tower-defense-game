# CORE//DEFEND — Circuit Tower Defense

A single-file HTML/CSS/JS tower defense game. No build step, no dependencies — just open `index.html`.

## Play locally
Double-click `index.html`, or serve it with any static server.

## Deploy to GitHub Pages
1. Create a new repo on GitHub (e.g. `core-defend`).
2. Add this `index.html` to the repo root and push:
   ```bash
   git init
   git add index.html README.md
   git commit -m "Initial commit: CORE//DEFEND tower defense"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
   ```
3. On GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, choose `main` and `/ (root)`, then Save.
4. After a minute or two, your game is live at:
   `https://<your-username>.github.io/<repo-name>/`

## How to play
- Pick a tower type in the sidebar, then click an open (non-path) grid tile to deploy it.
- Click a placed tower to inspect it, **upgrade** it (boosts damage/range, raises cost), or **sell** it for a partial refund.
- Click **Launch Next Wave** to send enemies down the circuit path toward the core.
- Survive all 15 waves without your Core Integrity hitting 0 to win.
- The **⚡ Infinite Credits** button is a built-in cheat toggle — flip it on any time for unlimited money.

## Tower types
| Tower | Cost | Style |
|---|---|---|
| Pulse Node | 50c | Fast, balanced single-target |
| Cannon Node | 90c | Slow, splash damage |
| Beam Node | 130c | Instant hit, high fire-rate |
| Frost Node | 75c | Splash + slows enemies |

Everything (HTML, CSS, JS) lives in `index.html` — feel free to tweak balance numbers, add tower types, or reskin the theme directly in that file.
