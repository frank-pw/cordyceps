# Cordyceps

> An Obsidian theme inspired by *The Last of Us* — survival logs, tarnished gold, worn borders, and the quiet weight of a world after, with dark and faithful light modes.

![Obsidian](https://img.shields.io/badge/Obsidian-1.5%2B-8fa35c?style=flat-square&logo=obsidian&logoColor=white)
![Version](https://img.shields.io/badge/version-1.0.1-d8b85a?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-4a432f?style=flat-square)

---

## Preview

<!-- Replace with an actual screenshot -->
![Cordyceps preview](preview.png)

---

## Design

The theme draws from the visual language of *The Last of Us*: blackened charcoal panels, olive-green navigation, tarnished-gold accents, faded paper text, worn borders, and a subtle CRT grain layered over everything. The dark palette keeps the theme weathered and high-contrast, while light mode translates the same mood into aged paper, charcoal text, field olive, rust, and burnt orange. It is built entirely in CSS — no plugins, no external assets, no fonts that need downloading (the theme falls back to system monospace if IBM Plex Mono is absent).

### Color palette

| Token | Hex | Role |
|---|---|---|
| Background | `#0d0d0a` | Main canvas |
| Panel | `#11110d` | Sidebars, tabs |
| Text | `#d8d0bd` | Body copy — faded paper |
| Gold | `#d8b85a` | Accents, active tabs, links |
| Olive | `#8fa35c` | Navigation, H3 headers, folder icons |
| Orange | `#fa9442` | Open folders, warm warning accents |
| Rust | `#7a553d` | Subtle warmth |
| Border | `#4a432f` | Worn edges |

The CSS also defines softer and darker supporting variants for text, gold, olive, borders, code blocks, selections, and interactive states. Light mode remaps the same tokens to a faithful paper-log palette rather than a plain white UI.

---

## Features

- **Pure CSS** — no snippets, plugins, or internet connection required
- **Dark and light modes** — light mode keeps the worn survival-log mood instead of flattening into a neutral theme
- **Subtle CRT scanline + film grain** overlay via a single `::before` pseudo-element
- **Radial gradient panel vignettes** on sidebars and reading view
- **File explorer folder icons** — closed folders in olive, open folders in orange, no arrows
- **Monospace typography** throughout using IBM Plex Mono (or system fallback)
- **Styled headings**: H1 with a bottom rule, H2 in warm gold, H3 in uppercase olive, plus distinct H4-H6 accents
- **Callouts, blockquotes, tables, code blocks** — all reskinned to match the palette
- **Custom checkboxes** with a gold fill and tick on completion
- **Clearer focus and active states** for tabs, files, inputs, dropdowns, and canvas nodes
- **Worn horizontal rules** that fade right to transparent
- **Custom scrollbars**, graph view colors, metadata panel, modal and menu styling
- **Mobile-ready** — adjusted padding for small screens

---

## Installation

### Via Obsidian Community Themes *(recommended)*

1. Open **Settings → Appearance → Themes**
2. Click **Manage** and search for `Cordyceps`
3. Click **Install and use**

### Manual

1. Download or clone this repository
2. Copy the `Cordyceps` folder into your vault's themes directory:

```
<your vault>/.obsidian/themes/Cordyceps/manifest.json
<your vault>/.obsidian/themes/Cordyceps/theme.css
```

3. In Obsidian go to **Settings → Appearance → Themes**, refresh the list, and select **Cordyceps**

> **Note:** do not nest the folder — Obsidian requires the `manifest.json` to sit directly inside `.obsidian/themes/Cordyceps/`.

### Optional font

The theme is designed with [**IBM Plex Mono**](https://fonts.google.com/specimen/IBM+Plex+Mono). Install it on your system for the intended look; the theme degrades gracefully to `SFMono-Regular`, `Menlo`, or `Consolas` if it is absent.

---

## Compatibility

- Obsidian **1.5.0** and later
- Dark and light mode

---

## License

MIT © Francesco Palermi
