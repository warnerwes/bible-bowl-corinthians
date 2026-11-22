# Bible Bowl Study — 1 & 2 Corinthians (pilot) — MOVED

> **This site has moved to <https://bible-bowl-study.web.app/>** (Firebase
> Hosting, served from the `bible-bowl-study` repo). The GitHub Pages site now
> only redirects there. This repo is frozen as a historical snapshot.

## Corinthians release handoff

The update adds 106 NKJV questions and source-linked **Go deeper** notes across
all 29 chapters of 1 and 2 Corinthians. All 15 weeks have five-question rounds.

- [Tested release patch](releases/go-deeper-corinthians.patch) applies to the
  previous Firebase Hosting build's static files.
- [Build source at commit `22499a6`](https://github.com/warnerwes/bible-bowl-study/tree/22499a6f40d031cd24117c8a28db20d104ce8210/generator/pilots/corinthians)
  contains the runnable game. Use this commit to produce the Firebase upload.

From the root of the `warnerwes/bible-bowl-study` checkout, build and test:

```sh
node generator/pilots/corinthians/build-site.mjs
node --test engine/tests/test-pilot-build.mjs
```

Firebase Hosting uses `generator/pilots/corinthians/_site`. The legacy Pages
redirects in this repository have their own manual workflow.
