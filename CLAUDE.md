# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A static single-page Renekton (League of Legends) champion guide focused on combo references. The entire site is a single `index.html` file with inline CSS, accompanied by MP4 video demonstrations in `videos/`.

## Architecture

- **index.html** — The complete guide: inline `<style>` block, no JavaScript, no build tools, no dependencies. Sections cover: summary, builds, abilities, matchups, tips, auto-reset mechanics, combos, and full combo sequences.
- **videos/** — MP4 clips demonstrating specific combos and mechanics. Named after the combo they show (e.g., `Panther.mp4`, `W-R.mp4`, `AA-Q.mp4`). These are referenced conceptually in the guide but not all are wired up with `<video>` tags yet.

## Development

No build step. Open `index.html` directly in a browser or serve with any static file server:

```
python3 -m http.server 8000
```

## Content Status

- Video embeds are placeholder text, not yet linked to the MP4 files in `videos/`.
