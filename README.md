# rAIse — Responsible AI Social Evaluation

> **Microsoft ISD · 2026**
> Interactive AI readiness assessment and technology prescription tool.

## What is rAIse?

rAIse evaluates your organization's readiness for AI adoption across 7 strategic pillars and automatically generates a technology prescription tailored to your maturity level and technology context.

**Live site:** `https://<your-org>.github.io/raise/`

---

## How to Deploy to GitHub Pages

### Option A — Simple (docs folder, no Actions needed)

1. Create a new **public** GitHub repository (e.g., `raise`)
2. Copy `index.html` into the repo root (or a `docs/` folder)
3. Go to **Settings → Pages**
4. Set source: `main` branch, `/ (root)` folder (or `/docs` if you placed it there)
5. Save — GitHub Pages will publish within a minute

Your site will be available at: `https://<org>.github.io/raise/`

### Option B — GitHub Actions (recommended, already configured)

The `.github/workflows/deploy.yml` file is included. Just:

1. Push this entire folder to a new GitHub repository
2. Go to **Settings → Pages → Source** → select **GitHub Actions**
3. Push any change to `main` to trigger deployment

---

## Structure

```
raise/
├── index.html                  ← Full self-contained web app
├── README.md
└── .github/
    └── workflows/
        └── deploy.yml          ← GitHub Pages deployment workflow
```

---

## Features

| Tab | Description |
|-----|-------------|
| **Overview** | Tool introduction, pillar descriptions, quadrant framework |
| **Assessment** | 35 questions × 7 pillars, scores 1–5, auto-saved in browser |
| **Tech Profile** | 6 technology context questions (T1–T6) |
| **Prescription** | Full auto-generated recommendation: quadrant, STU teams, ISD solution plays, security layers, 30-day action, roadmap |

---

## Quadrant Framework

| Quadrant | Description | Focus |
|----------|-------------|-------|
| Q1 — AUGMENT | Low Autonomy · Low Complexity | Human-augmented AI tools (M365 Copilot) |
| Q2 — AUTOMATE | High Autonomy · Low Complexity | Task automation agents |
| Q3 — ORCHESTRATE | Low Autonomy · High Complexity | Enterprise orchestration platforms |
| Q4 — TRANSFORM | High Autonomy · High Complexity | Multi-agent AI-native transformation |

---

Microsoft ISD | FY26 Cloud & AI Platforms Portfolio
