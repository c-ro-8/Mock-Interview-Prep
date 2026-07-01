# Mock Interview Prep — Powered by Claude

A browser-based mock interview tool that uses the Anthropic Claude API to generate targeted interview questions and give instant, scored feedback on your answers.

Built as a portfolio project for the [Claude Corps Fellowship](https://www.anthropic.com/claude-corps).

---

## What it does

1. **Generates custom questions** — paste a job title, organization, and job description, and Claude generates realistic interview questions tailored to that specific role
2. **Gives scored feedback** — after you type your answer, Claude rates it across Clarity, Relevance, and Specificity (1–10) and gives direct coaching notes
3. **Tracks your session** — a progress bar and summary screen show how you performed across all questions
4. **Supports multiple formats** — behavioral (STAR), situational, technical, and social-impact/motivation questions

---

## Who it's for

Early-career applicants practicing for nonprofit, government, and mission-driven tech roles — the exact kinds of organizations Claude Corps places fellows at (Braven, Code for America, World Vision, etc.).

---

## How to use it

### Option 1: Open directly in a browser (no install needed)
1. Download or clone this repo
2. Open `index.html` in any modern browser
3. Enter your Anthropic API key ([get one free at console.anthropic.com](https://console.anthropic.com))
4. Fill in the role and org, and start practicing

### Option 2: Run from GitHub Pages
1. Fork this repo
2. Go to **Settings → Pages → Source → Deploy from branch (main)**
3. Your live URL will be `https://yourusername.github.io/mock-interview-prep`

---

## Tech stack

- Plain HTML, CSS, and vanilla JavaScript — no frameworks, no build step
- [Anthropic Claude API](https://docs.anthropic.com) (`claude-sonnet-4-6`) via browser `fetch`
- Zero dependencies, zero backend — runs entirely in the browser

---

## API key security note

Your API key is entered directly in the browser and is only sent to `api.anthropic.com`. It is never stored, logged, or sent anywhere else. For a production deployment, you would move the API call to a backend server to keep the key out of the browser entirely.

---

## Project structure

```
mock-interview-prep/
└── index.html     # The entire app — questions, feedback, summary, all in one file
└── README.md      # This file
```

---

## What I'd build next

- Save session history to `localStorage` so you can review past practice runs
- Add a "model answer" feature that shows an example strong response after feedback
- Export a PDF summary of your session to share with a mentor
- Add voice input so you can practice speaking your answers out loud

---

## About

Built by c-ro-8 as part of a Claude Corps fellowship application. Inspired by Braven's mission to help first-generation college students land strong first jobs through career readiness practice.
