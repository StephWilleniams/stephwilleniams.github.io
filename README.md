# stephwilleniams.github.io

Personal academic site, built automatically by GitHub Pages (Jekyll) on every push.

## Common edits

**Add an update:** create a file in `_posts/` named `YYYY-MM-DD-short-slug.md`:

```markdown
---
title: My new paper
kind: Paper            # Paper, Talk, Poster, Teaching…
summary: One sentence shown in the updates list and on the homepage.
links:
  - label: Paper
    url: https://doi.org/...
---

The full text of the update, in Markdown.
```

It appears at `/updates/short-slug/`, at the top of `/updates/`, and in the homepage News list.

**Add a figure:** upload images to `images/research/`. The research pages already look for:
`internalCavity.jpg`, `flowExample.jpg`, `biofilms.png`, `channelFilling.png`.
Any that are missing are simply hidden.

**Add a study system:** add an entry to `_data/organisms.yml`, and a page at
`research/<slug>/index.md` (copy an existing one).

**Share a file:** put it in `files/`. It is served at `/files/<name>`.

**Add an LLM-fun item:** put its files in `llm-fun/<slug>/` (an `index.html` there is served as is),
add a card image to `images/llm-fun/`, and add an entry to `_data/llm_fun.yml`. It appears on `/llm-fun/`.

## Layout

- `index.html`: homepage
- `research/`: research overview and one page per study system
- `updates/`: list of all updates; each post lives in `_posts/`
- `_layouts/`: shared page templates (header, footer, post, organism page)
- `assets/css/site.css`: styles
- `sims/`: standalone interactive simulations, shown together on `interactive/`
- `fun-stuff/`: the Fun stuff page and its Music page; it also links to `llm-fun/`
- `llm-fun/`: side projects built with language models; the list comes from `_data/llm_fun.yml`
- `redirects/`: forwards old URLs from the previous site to the new pages
