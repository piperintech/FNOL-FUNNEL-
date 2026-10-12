# FNOL Funnel — First Notice of Loss intake form

**A guided, mobile-friendly form that lets anyone involved in an auto accident report a claim online, with submissions flowing automatically into SharePoint for the claims team.**

[Live demo](https://piperintech.github.io/FNOL-FUNNEL-/) · Built for SNAP Insurance Service LLC

---

## The problem

First notice of loss happened mostly by phone. Clerks re-typed everything into the claims system, callers forgot details, and every claim took about **20 minutes** of intake time.

## What it does

- Walks the caller through the accident **one section at a time**: who they are, the loss, the insured vehicle and driver, the other party, police and injuries
- **Adapts to who's filling it out** (insured, relative, claimant, witness, attorney) and only asks what's relevant
- Plain, reassuring language for a bilingual customer base that may not know insurance terms ("Leave anything blank you don't know")
- Validates required fields before submitting
- Sends a structured JSON payload to a **Power Automate** HTTP trigger, which creates a record in **SharePoint** for the team

## Result

Intake time dropped from **~20 minutes to ~6 minutes** per claim, and every report arrives structured instead of as free-text notes.

## Stack

HTML, CSS, vanilla JavaScript · Power Automate (HTTP trigger) · SharePoint list · GitHub Pages

## Setup

The backend URL is a placeholder. To connect your own flow, create a Power Automate flow with the trigger **"When an HTTP request is received"**, then paste its URL into `BACKEND_URL` in `index.html`.

> Never commit a real trigger URL to a public repo. Anyone with the link can post to the flow.

---

Built by **Manuela Gonzalez Piper** · Product & AI · [GitHub](https://github.com/piperintech)
