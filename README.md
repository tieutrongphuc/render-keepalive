# render-keepalive

Pings the CS3227 MP4 app (https://cs3227-2610-mp4.onrender.com/) on Render every 10 minutes so the free instance does not spin down.
The workflow is in `.github/workflows/keep-render-awake.yml`.

- To change the target, set a `RENDER_PING_URL` repository variable (Settings → Secrets and variables → Actions → Variables).
- Scheduled runs only start from the default branch, and GitHub pauses them after 60 days with no repository activity. Turn them back on from the Actions tab.
- To run it by hand: Actions → Keep Render awake → Run workflow.
