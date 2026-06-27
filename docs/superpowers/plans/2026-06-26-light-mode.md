# Cordyceps Light Mode Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Add a faithful light mode to the Cordyceps Obsidian theme.

**Architecture:** Keep one theme file and add `.theme-light` support alongside the existing dark rules. Shared structural selectors should apply to both modes, while light mode overrides colors with an aged-paper palette.

**Tech Stack:** Obsidian CSS theme, Markdown docs, static HTML preview.

---

### Task 1: CSS Light Mode

**Files:**
- Modify: `theme.css`

- [x] Verify current missing behavior:
  Run `rg -n "\.theme-light\b" theme.css`
  Expected: no `.theme-light` selector in the production CSS.

- [x] Add `.theme-light` variables using paper, charcoal, tarnished-gold, field-olive, rust, and burnt-orange tones.

- [x] Share existing structural rules between `.theme-dark` and `.theme-light`.

- [x] Add light-specific overrides for backgrounds, chrome, headings, links, callouts, tags, code, forms, menus, canvas, scrollbars, and mobile chrome.

- [x] Verify:
  Run `rg -n "\.theme-light\b|theme-light" theme.css`
  Expected: `.theme-light` selectors exist.

### Task 2: Docs And Preview

**Files:**
- Modify: `README.md`
- Modify: `preview.html`

- [x] Update README wording from dark-only to dark and light support.

- [x] Update preview so it uses the real `.theme-light` class instead of a private preview-only class.

- [x] Verify:
  Run `awk` brace-balance checks on `theme.css` and `preview.html`.
  Run `curl -I http://localhost:8000/preview.html`.
  Expected: brace balance ok and HTTP 200.
