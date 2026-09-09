# SAFER Utah site

The invariant is a tiny, accessible static site with no runtime dependency on third-party assets.

- `public/` deploys as-is. Do not add a build system without a concrete need.
- Keep `saferut.org` canonical; `saferutah.org` redirects there.
- Fonts, images, CSS, and scripts must be local. External links are fine.
- Do not add analytics, cookies, or forms without updating the privacy page to match reality.
- `recovery/` is source evidence from saferdrinks.org, not deployable site code.

## Editing and publishing

- Site content lives in `public/`. Do not edit `recovery/` unless the task is explicitly historical research.
- Make the smallest change that answers the request. Preserve the existing visual system and responsive behavior.
- Before publishing, check the changed files, run `git diff --check`, and preview the affected page when practical.
- A request to **publish** means: commit the reviewed change to `main`, push it to GitHub, wait for the `Deploy site` GitHub Actions workflow, then verify the changed live page at `https://saferut.org/` with a cache-busting query string.
- Normal content edits should not publish by surprise. Ask for a publish request, or follow the explicit shorthand `cpd`.
