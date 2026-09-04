# Pong-Test
Testing out coding abilities of Claude

## Play

A single-file, dependency-free Pong game lives in [`index.html`](index.html).

- Open `index.html` directly in a browser to play locally.
- Left paddle: `W` / `S`. Right paddle: `Arrow Up` / `Arrow Down`. Touch screens: drag on the left/right half of the screen.
- `Space` pauses/resumes. First to 7 points wins.

### CI and deployment

Every push and pull request runs an HTML validation check
(`.github/workflows/deploy.yml`). On pushes to `main`, once validation
passes, the workflow deploys the site to GitHub Pages automatically —
a broken push never goes live.

To enable this the first time:

1. In the repo, go to **Settings → Pages**.
2. Under **Build and deployment**, set **Source** to `GitHub Actions`.
3. Push to `main` (or re-run the workflow from the **Actions** tab). GitHub
   will publish the site at `https://<username>.github.io/<repo-name>/`
   within a minute or two, and keep it updated on every subsequent push.
