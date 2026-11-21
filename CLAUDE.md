# MythoKoo Stories — Site Handoff

## Site identity
- **Name**: MythoKoo Stories
- **Series**: 16 Kindle eBooks · 2 seasons · Indian mythology picture books
- **Live artifact**: https://claude.ai/artifact/Rite3izNjGmm1q8YKLvvgK (Version 4)
- **Contact email**: mythokoo@quizykoo.com

## File structure
```
index.html          ← single-page source, matches live artifact
covers/
  book1.jpg         ← Ramayana books (Season 1, books 1–8)
  book2.jpg
  ...
  book9.jpg         ← Mahabharata books (Season 2, books 9–16)
  ...
  book16.jpg
logo.png            ← MythoKoo logo
```

## Seasons
| Season | Theme | Books |
|--------|-------|-------|
| Season 1 — Ramayana | The epic of Rama | 1–8 |
| Season 2 — Mahabharata | The epic of the Pandavas | 9–16 |

## Design tokens
- **Theme**: Dark indigo/gold — rich, mythological feel
- **Fonts**: Cinzel (headings, Google Fonts) + Crimson Pro (body) + Inter (UI)
- **Primary dark**: `#1a0a2e` · Gold accent: `#c9a84c`
- Dark-mode committed (single theme, no light variant)

## Book data
Book metadata (title, Amazon link, cover filename) is in the `books` array in the `<script>` block.
Each entry: `{ id, season, title, cover, link }` — `cover` maps to `covers/bookN.jpg`.

## To update and publish via Claude Code
```
# Open in Claude Code, then in Claude:
# 1. Edit index.html (update Amazon links, text, books, etc.)
# 2. Tell Claude: "Publish this to https://claude.ai/artifact/Rite3izNjGmm1q8YKLvvgK"
```

## Amazon links
Each book card links to its KDP product page. Links are in the books array in `index.html`.
Original covers (JPG) are in `covers/` folder in this handoff zip.

## Footer / Contact
Email appears in the footer as a mailto link: `mythokoo@quizykoo.com`
