# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

**MIKA | Trading Terminal** — VIP Discord community resources for crypto traders.
Hosted on GitHub Pages: `https://mika-trading-terminal.github.io/vip/`
GitHub repo: `https://github.com/mika-trading-terminal/vip`

## Deploying

All HTML files are deployed via GitHub Pages from the `main` branch.

```bash
# Push a new or updated file live
git add <file> && git commit -m "<description>" && git push
```

Each resource lives in its own folder for clean URLs:
- `risikomanagement/index.html` → `/vip/risikomanagement`
- `psychology/index.html` → `/vip/psychology`
- `pre-trading-routine/index.html` → `/vip/pre-trading-routine`

New resources follow the same pattern: create a folder with `index.html` inside.

## Design System

All VIP resources use the same design — do not deviate from these values.

| Token | Value | Usage |
|---|---|---|
| Electric Cyan | `#00E5FF` | Primary headings, links, highlights |
| Deep Violet | `#7C3AED` | Secondary headings, accents |
| VIP Gold | `#D4A017` | VIP badges, premium elements |
| Alert Pink | `#FF2D7B` | Warnings, alerts |
| Void Black | `#0A0A14` | Page background |
| Ice White | `#E0E7FF` | Body text |

Background grid overlay, JetBrains Mono for code/labels, Inter for body text.

## Rules

- **Always mobile-responsive** — one file with `@media (max-width: 768px)` breakpoints, never two separate files
- **No Crypto Terminal** — brand name is always **Trading Terminal**
- **No Fear & Greed Index, Funding Rate, or Open Interest** references in any resource
- Every new resource gets its own folder (`foldername/index.html`) for clean URLs
- PDF exports via Chrome headless: `"/Applications/Google Chrome.app/Contents/MacOS/Google Chrome" --headless --no-sandbox --print-to-pdf="OUTPUT.pdf" --no-pdf-header-footer "file:///PATH/TO/FILE.html"`
