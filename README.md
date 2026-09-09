# SAFER Utah

Static site for [saferut.org](https://saferut.org). Plain HTML and CSS, no build step, runtime JavaScript, third-party fonts, trackers, or cookies.

## Local preview

```sh
python3 -m http.server 4173 -d public
```

## Structure

- `public/`: deployable site
- `recovery/`: preserved copy and original media recovered from the final 2026 Wayback snapshot of saferdrinks.org

The canonical site is `https://saferut.org`. `saferutah.org` should redirect there at the edge.

## Edit and publish from the ChatGPT desktop app

This site needs no local build, account keys, or terminal commands. GitHub Pages publishes the contents of `public/` whenever `main` is pushed.

### One-time setup for Crystal

1. Accept a GitHub invitation with **Write** access to `carlkibler/saferut`.
2. Clone this repository with any graphical Git client, such as GitHub Desktop.
3. In the ChatGPT desktop app, switch to **Codex** and open the cloned `saferut` folder as a local project.

### Everyday workflow

Tell Codex what should change, then say: **“Review this, commit it to main, push it, and verify the live site.”** It can review the diff and use its built-in Git controls to commit and push without opening a terminal. The GitHub Actions `Deploy site` workflow then publishes the change automatically.

Use `public/` for the live site. `recovery/` is archive material only. Keep images, fonts, CSS, and scripts local; do not add trackers, cookies, or forms without also updating `public/privacy/index.html`.
