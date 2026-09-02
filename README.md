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
