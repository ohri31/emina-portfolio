# SendBase Case Study — Project Guide

## What this project is
A **static single-file HTML portfolio case study** documenting a UX/UI design internship project (SendBase data importer). No build step, no server, no framework.

## Technical constraints — read before touching anything

- **One file:** All HTML, CSS, and content lives in `sendbase-case-study-v3.html`. Do not split it.
- **No dev server:** Open the file directly in a browser (`file://`). Do not create `launch.json`, run `npm`, `npx serve`, or any server command.
- **No packages:** There is no `package.json`. Do not install dependencies.
- **Pure HTML + CSS:** No React, Vue, Tailwind, or any JS framework. Write plain HTML5 and CSS.
- **Fonts:** Loaded from Google Fonts via `<link>` in `<head>` — Inter (300/400/500/600) and DM Serif Display. Do not add new font imports unless instructed.
- **Images:** Stored in `images/` directory, referenced with relative paths.
- **CSS location:** Inline `<style>` block inside `<head>`. Keep all CSS there. Match the existing compact/minified style (multiple rules per line, short class names).

## How to preview
Open `sendbase-case-study-v3.html` directly in a browser. No server needed.

## Page structure
Sections are numbered 01–11, each with a matching `id`:

| Section | ID | Content |
|---|---|---|
| 01 | `#context` | Project overview |
| 02 | `#research` | Competitive analysis |
| 03 | `#opportunities` | Design opportunities |
| 04 | `#personas` | User personas |
| 05 | `#problem` | Problem statement |
| 06 | `#strategy` | Strategic foundation |
| **07** | **`#design-system`** | **Design system: typography, colours, components** |
| 08 | `#design` | HiFi screens |
| 09 | `#testing` | Usability testing |
| 10 | `#reflection` | Reflection |
| 11 | `#future` | Future opportunities |

## CSS conventions
- Class names are short (`.tsr`, `.swrow`, `.ds-palette`) — keep new ones concise with a short prefix
- CSS custom properties in `:root` define the colour palette — use them: `--black`, `--s1`, `--s2`, `--s3`, `--text`, `--muted`, `--accent`, `--white`, `--line`, `--faint`
- The page is **dark-themed** — adapt any light-themed Figma designs to fit the dark background
- Add mobile overrides inside the existing `@media(max-width:660px)` block

## Working with Figma
- Use the Figma MCP tools (`get_screenshot`, `get_design_context`) to extract specs from provided links
- Figma designs are light-themed (white bg, black text) — translate colours to the dark theme
- Do NOT copy Figma's React/Tailwind output literally — convert to plain HTML/CSS
- Font sizes from Figma are in `px` — convert to `rem` (divide by 16) unless matching an exact design spec inline
