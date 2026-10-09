# 🚀 GitHub Launchpad

![vanilla JS](https://img.shields.io/badge/vanilla-JS-f7df1e?logo=javascript&logoColor=black)
![no API](https://img.shields.io/badge/API-none-3dff9e)
![license](https://img.shields.io/badge/license-MIT-4dd0e1)

**You wrote the code. You skipped the packaging. Now nobody finds it. Fill in what your repo does → get a ready-to-paste description (≤350 chars), validated topics, social preview text and README opening — all from templates, all local.**

> Part of [The Antigle](https://github.com/mukund-buddy) 🔥 — AI-assisted build, hand-tested.
> Born from auditing my own repos and finding 6 of them with no topics and a one-word description.

**Live demo:** _coming soon_ · [Repository](https://github.com/mukund-buddy/github-launchpad)

---

## 🎯 Why This Exists

GitHub's discoverability levers are boring and skipped by nearly everyone:

| Field | What it does | What people write |
|-------|--------------|-------------------|
| **Description** | shows in search + Google | nothing, or "my project" |
| **Topics** | the actual search index | nothing |
| **Social preview** | decides if a link gets clicked | the default screenshot |

These three fields are free, take 60 seconds, and matter more than your 12th feature.
Launchpad generates all of them from one form — no API key, no account, no upload.

## ✨ Features

- **Description** — composed from name + "what it does" + who it's for, with a live counter that turns amber at 300 and red past GitHub's 350-char limit
- **Topics** — auto-derived from your repo name, stack tags, detected keywords and project type; validated against GitHub's rules (`a-z 0-9 -`, ≤50 chars, ≤20 topics), remove/add chips
- **Social preview** — 2–3 lines that survive the smallest embed
- **README opening** — H1 + one-line `>` tagline + the Antigle credit block
- **Honest constraints** — checkbox clauses ("Client-side only.", "No build step.") that are added **only if you tick them** — the generator never claims what it can't know
- **Everything persists** — form, chips and constraints survive refresh (localStorage)
- **Copy everything** — one block with all four outputs, ready to paste

## 🚀 Quick Start

```bash
git clone https://github.com/mukund-buddy/github-launchpad
start index.html
```

Fill the left column → copy the right column into your repo settings + README.

## 🧱 How It Works

```
index.html   →  input form + four output cards
style.css    →  mission-control theme (phosphor green, scanlines, mono only)
app.js       →  recipes: TYPE_POOL, KEYWORDS, build*() functions
```

Generation is **template + recipe table** driven — deliberately not an LLM. That's why
it's instant, offline and free. Editing the recipes in `app.js` retunes the voice for
your whole output.

## ⚠️ Honest Note

The tool can't verify your claims — you tick the constraints. If your project *does*
have a backend, don't tick "Client-side only." Topics are a suggestion: keep the ones
that are true, drop the ones that aren't.

## 🗺️ Roadmap

- [x] Description / topics / preview / README (v1)
- [ ] Topic research: show approximate GitHub search volume per topic
- [ ] Badge row generator (`shields.io` line for the README)
- [ ] Multi-repo mode for an entire org

## 🏷️ Suggested GitHub Topics

`github` `seo` `metadata` `open-source` `developer-tools` `topics` `readme` `repository` `vanilla-js` `the-antigle`

(Yes — using this repo's own generator on this repo's own topics is the intended flex.)

Add them under **Settings → General → Topics**.

---

Part of **[The Antigle](https://github.com/mukund-buddy)** — browser tools and web products, built with AI and finished by hand.

## 📄 License

MIT
