# 💡 UXMap App – Ideation Pad

This document captures raw ideas, potential features, and brainstorming notes for the UXMap app.

---

## 🔭 Vision
To create a mobile-first tool (Flutter + OpenAI) that:
- Analyzes a website’s UI/UX (live or static)
- Builds a customer journey map (auto-generated)
- Suggests UX improvements or scores
- Outputs visuals (e.g. journey flow, heatmap, annotated screenshot)

---

## 🧠 Raw Ideas

- [ ] Focus on "clickable elements only" to stay within token limits
- [ ] Start with 3-click journey depth
- [ ] Capture page title, load time, and UX score per node
- [ ] Add a "crawl & snapshot" mode (headless browser or API)
- [ ] Output PNG + JSON journey
- [ ] Track user flow time (time per page or dwell time?)

---

## 🤖 AI Ideas

- Use OpenAI GPT API to:
  - Label page purpose (landing, product, checkout, etc.)
  - Assign UX score (1–5) with rationale
  - Extract sentiment tone or visual consistency
- Maybe experiment with vision models (later)

---

## 🛠️ Features by Phase

### MVP
- [ ] URL input
- [ ] Crawl 3 steps deep
- [ ] Display flow map (text or simple UI)

### v1.0
- [ ] Image-based output (journey map)
- [ ] UX scoring model
- [ ] CSV/JSON export

---

## 🧩 Questions to Solve
- How to limit token cost per site?
- Can GPT analyze image-based screenshots affordably?
- What’s the best way to extract clickable elements in Flutter?

---
_Last updated: 2025-06-20_
