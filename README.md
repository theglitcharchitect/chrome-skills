# Chrome Skills — Elite Custom Library

> Ten original, hardened **Chrome Skills** for **Gemini in Chrome** — reusable, injection-resistant prompts with copy-ready blocks and a clean, responsive reading experience.

![Skills](https://img.shields.io/badge/skills-10-2783DE)
![Add--ons](https://img.shields.io/badge/universal%20add--ons-4-46A171)
![Hardening](https://img.shields.io/badge/red--team%20%2B%20polish-8%C3%978%20each-7D7A75)
![Built with](https://img.shields.io/badge/built%20with-HTML%20%C2%B7%20CSS%20%C2%B7%20JS-111)
![No deps](https://img.shields.io/badge/dependencies-none-46A171)

**🔗 Live site: https://theglitcharchitect.github.io/chrome-skills**

---

## What are Chrome Skills?

[Skills in Chrome](https://blog.google/products-and-platforms/products/chrome/skills-in-chrome/) (launched April 14, 2026) let you save your most useful AI prompts and re-run them in **Gemini in Chrome** with a single click. A Skill runs on the page you're viewing **plus any other tabs you select**, and asks for confirmation before sensitive actions like sending an email or adding a calendar event.

This repository is an **independent, hand-built library** of ten Skills, each engineered against the feature's real constraints — multi-tab input, fast/error-prone models, and exposure to page-level prompt injection.

## How Skills work

| Step | Action |
|------|--------|
| **1. Save a prompt** | Write a prompt you'll reuse and save it as a Skill from your Gemini in Chrome chat history. |
| **2. Select your tabs** | Open the pages you want to work across — the Skill reads the current page plus any tabs you select. |
| **3. Run with `/`** | Type `/` or click `+` in Gemini in Chrome, pick your Skill, and it runs in one click. |

## The library

| # | Skill | What it's for |
|---|-------|---------------|
| 1 | **Cross-Tab Decision Matrix** | Weighted comparison of anything across open tabs — products, apartments, tools, offers, papers. |
| 2 | **Source & Claim Auditor** | Evidence quality, bias, spin, and what an article leaves out. |
| 3 | **Fine-Print X-Ray** | Risky clauses in ToS, privacy policies, leases, loans, and contracts. |
| 4 | **Community Consensus Distiller** | The real, weighted consensus from forums and reviews — minus astroturf. |
| 5 | **Deep-Learning Tutor** | Layered teaching, self-tests, and spaced-repetition recall cards. |
| 6 | **Opportunity Fit Analyzer** | Jobs, grants, RFPs, and gigs scored against your profile, with red flags. |
| 7 | **Universal Shopping Analyst** | Price, quality, regional pricing, and where-to-buy — with strict no-fabrication rules. |
| 8 | **Ghostwriter & Humanizer** | Human-voice writing and rewriting, free of the classic AI tells. |
| 9 | **Clinical Pharmacist & Drug Insight Analyst** | Pharmacist-grade drug workups with hard medical safety rails. |
| 10 | **Trip Architect — Flights, Stays & Deals** | End-to-end trip planning: flights, stays, verified promos, and an itinerary. |

Plus **four universal add-ons** (confidence tags, self-check pass, coverage meter, assumption ledger) you can paste into any Skill.

## How to use

1. Open the [live site](https://theglitcharchitect.github.io/chrome-skills) and find a Skill.
2. Click **Copy** on its prompt block.
3. In Gemini in Chrome, open `chrome://skills`, create a new Skill, and paste the prompt.
4. Edit freely to fit your workflow.

## Design

A single self-contained `index.html` — no build step, no dependencies:

- Responsive layout with a sticky, scroll-spying table of contents
- Automatic light/dark theme with a manual toggle (saved to `localStorage`)
- One-click copy on every prompt block
- Inline SVG graphics (no external image requests)

## Notes & caveats

- `chrome://skills` is a browser-internal page; this library is built from public documentation of the feature plus community sources, not a scrape of your local Skills page.
- Skills currently run in Gemini in Chrome on desktop (Mac, Windows, ChromeOS) with the display language set to English (US).
- Anything that sends or schedules is written to **propose** the action for Chrome's confirmation step, never to auto-execute.

## Credits

Feature background and quotes come from Google's announcement, ["Turn your best AI prompts into one-click tools in Chrome"](https://blog.google/products-and-platforms/products/chrome/skills-in-chrome/). This is an unofficial, independent project and is **not affiliated with or endorsed by Google**. "Chrome" and "Gemini" are trademarks of Google LLC.
