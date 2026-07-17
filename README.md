# Bible Bowl Study — 1 & 2 Corinthians (pilot) — MOVED

> **This site has moved to <https://bible-bowl-study.web.app/>** (Firebase
> Hosting, served from the `bible-bowl-study` repo). The GitHub Pages site now
> only redirects there. This repo is frozen as a historical snapshot.

A self-contained static quiz + reading-plan site covering **1 & 2 Corinthians**,
built from the config-driven engine in
[`warnerwes/bible-bowl-study`](https://github.com/warnerwes/bible-bowl-study)
(`generator/pilots/corinthians`). The site **never hosts scripture text** —
passages link out to Bible Gateway (NKJV).

> **Status:** the questions are **placeholders** (reference-based demos) pending
> real student seeds and review. The engine JS here is a **copy** — see
> [`.bbs-engine.json`](.bbs-engine.json).

## Not live yet — publishing is manual

Pages deployment is intentionally **manual-only** so nothing goes public until
you choose. To publish to `https://warnerwes.github.io/bible-bowl-corinthians/`:

- **GitHub UI:** Actions tab → **Deploy to GitHub Pages** → **Run workflow**, or
- **CLI:** `gh workflow run "Deploy to GitHub Pages" -R warnerwes/bible-bowl-corinthians`

The first run auto-enables Pages. To publish on every push instead, add a
`push: branches: [main]` trigger to `.github/workflows/deploy.yml`.

## Run locally

```
npx -y http-server . -p 5137 -c-1
# then open http://127.0.0.1:5137
```

## Regenerate

This repo holds the **built** site. To change it, edit the source in
`bible-bowl-study/generator/pilots/corinthians`, run `node build-site.mjs`, and
copy the resulting `_site/` contents here.
