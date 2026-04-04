# MidBoss.com

Jekyll-powered site for MidBoss, hosted on GitHub Pages.

## Quick Start

1. Clone this repo
2. Copy image assets from the old site into `assets/imgs/`
3. Push to GitHub
4. Enable GitHub Pages in repo settings (deploy from main branch)

## Adding a Blog Post

Create a new file in `_posts/` with the format:

```
YYYY-MM-DD-your-post-title.md
```

Add front matter at the top:

```yaml
---
title: "Your Post Title"
date: 2026-04-03
---

Your content here in Markdown.
```

## Adding a Game

Create a new file in `_games/` (e.g. `my-game.md`):

```yaml
---
title: "Game Title"
media: Game
release_date: "2026"
image: /assets/imgs/game-image.jpg
order: 1
excerpt: "Short description for the card."
links:
  - label: Steam
    url: https://store.steampowered.com/app/XXXXX
---

Full description in Markdown here.
```

The `order` field controls sort position (lower = first).

## Local Development

```bash
gem install bundler
bundle install
bundle exec jekyll serve
```

Then visit http://localhost:4000

## Image Assets Needed

Copy these from the old repo's `imgs/` folder into `assets/imgs/`:

- MidBossLogo.svg
- MidBossLogoMobile.svg
- MidBossLogoCastle.svg
- Neurodiver_W3.jpg
- 2064.jpg
- ComicWorks3.png
