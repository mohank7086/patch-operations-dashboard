# Live Patch Operations Dashboard 🖥️

**A real-time, role-based web dashboard for tracking Windows Server patching operations.**

No backend. No login accounts. Just open and operate.

Login as Engineer Pin: 2024

🔗 **[Try Live Demo →](https://pmonitor1.netlify.app)**

---

## The Problem

During live server patching windows, engineers had no real-time visibility into progress:

- Progress tracked in notepad or memory
- Managers had no way to monitor without interrupting the engineer
- Steps missed under time pressure
- Closure notes written from scratch post-session (~30 min)
- No consistent format or audit trail

---

## The Solution

A single HTML file — zero infrastructure — that gives engineers full control and
gives managers/viewers live read-only visibility into every patching session.

---

## Access Modes

### 🔧 Engineer Mode (PIN protected)
- 4-digit PIN login — no accounts needed
- Full control over the patching session
- Tick off steps in real time per server
- Drag-and-drop reorder steps on the fly
- Add or delete steps mid-session without losing progress
- Log drive space (C, G, M, F, H) per server
- Publish live state via JSONBin API — viewers see updates instantly
- One-click export of formatted closure note

### 👁️ Viewer Mode (open access)
- No PIN required
- Read-only view of live patching state
- Managers and directors can monitor progress without interrupting the engineer
- Refresh on-demand to see latest state

---

## Key Features

- **Session config** — set hospital/site name, maintenance window, server list before starting
- **Per-server step templates** — APP / SQL / TERM server templates with predefined checklists
- **Real-time state sync** — engineer publishes state via JSONBin REST API; viewers pull instantly
- **Drive space reporting** — visual bars flag critical (<20%) and warning (<40%) thresholds
- **Activity feed** — time-stamped log of every action during the session
- **Closure note export** — Salesforce-ready formatted note generated in one click
- **Zero infrastructure** — single HTML file hosted on Netlify free tier

---

## Operational Impact

| Metric | Result |
|---|---|
| Time saved per session | ~30 minutes (closure note auto-generated) |
| Manager visibility | 100% live, zero interruptions |
| Infrastructure cost | $0 (Netlify + JSONBin free tier) |
| Audit trail | Full — every action time-stamped |

---

## Tech Stack

- Vanilla HTML / CSS / JavaScript
- JSONBin REST API (state persistence)
- Netlify (hosting)

---

## Author

**Mohan Kumar K (Gus)**  
Senior Application Support Engineer → Platform / Infra Automation Engineer  
[![LinkedIn](https://img.shields.io/badge/LinkedIn-blue?style=flat&logo=linkedin)](https://www.linkedin.com/in/mohan-kumar-krishnappa/)
