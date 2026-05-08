# 🚀 Cosmic OS v1 — Mission Control

**A personal gamified life OS + learning management system** designed to turn ambitious goals into achievable systems through XP tracking, streak management, and strategic learning phases.

> Built by **Abhishek Pandey** · Nagpur → Germany → B.Sc. Physics & Astronomy → Astrophysicist

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Features](#-features)
- [How It Works](#-how-it-works)
- [Architecture](#-architecture)
- [Getting Started](#-getting-started)
- [Systems & Curriculum](#-systems--curriculum)
- [XP & Rank System](#-xp--rank-system)
- [Modules](#-modules)
- [Data & Storage](#-data--storage)
- [Browser Support](#-browser-support)

---

## 🌌 Overview

**Cosmic OS** is a personalized productivity and learning platform built for a single mission:

| Field | Detail |
|-------|--------|
| **Builder** | Abhishek Pandey (@abhi.astrophysics) |
| **Route** | Nagpur → Studienkolleg T-Kurs → Germany → B.Sc. Physics & Astronomy |
| **Goal** | Become an Astrophysicist |
| **Stack** | Single HTML file · Zero dependencies · Browser localStorage |

This is a **single-page HTML application** — no backend, no server, no cost. Open the file and it works.

---

## ✨ Features

### 🎮 Gamification Layer
- **XP System** — earn 3–15 XP per completed task depending on difficulty
- **6-Tier Rank System** — Cadet → Observer → Explorer → Navigator → Astronomer → Astrophysicist
- **Streaks** — track consecutive study days; 3+ days unlock bonus XP
- **12 Achievement Badges** — unlock for milestones, consistency, and system mastery
- **Level-Up Notifications** — animated pop-up celebrates every rank promotion

### 📊 Dashboard & Metrics
- Real-time counters: Today / Week / Streak / Total XP / STK Phase
- XP progress bar towards next rank
- Weekly completion bar chart
- XP earned per day chart
- Subject-specific breakdown analytics

### 🎯 Daily Mission Card
- Set **one main focus** for each day — the one thing that must get done
- Mark complete → feeds into streak and badge system
- Resets every day automatically

### 📈 Subject Health Strip
- Visual traffic lights for 6 subjects: Maths, Physics, German, Python, Mind, Luxastra
- 🟢 Studied today · 🟡 Within 3 days · 🔴 4+ days ago
- Stops subjects from silently being neglected

### 📅 6-Tab Interface

| Tab | Purpose |
|-----|---------|
| **Tracker** | Daily task completion across 5 systems, week navigation, streak dots |
| **Planner** | 7-day grid to plan the week + XP growth line chart across weeks |
| **Charts** | Task completion bar chart + XP per day + subject breakdown |
| **Badges** | 12 achievement cards — locked (grey) or unlocked (black) |
| **Resources** | 40+ curated books, videos, apps filtered by subject |
| **🇩🇪 STK** | Full 5-phase Studienkolleg T-Kurs tracker with deadlines + resources |

### 📚 Resource Library
- 40+ curated resources across all subjects
- Filterable by: Mathematics, Physics, Astronomy, German, Psychology, Python
- Priority stars (★) mark must-use resources
- Status tracking: `add` → `using` → `done`

### 🇩🇪 Studienkolleg T-Kurs Tracker
- Full 5-phase Germany roadmap: Preparation → Application → Visa → T-Kurs Year → FSP
- Phase-coloured accent bars (indigo, blue, emerald, amber, red)
- Deadline tracking with date badges
- Resource recommendations per phase
- Checklist with tagged task types (critical / exam / milestone / document)

---

## 🔧 How It Works

### Daily Flow
```
Morning   → Open Cosmic OS → Set today's mission
Day       → Check off tasks → Earn XP → Watch rank bar fill
Evening   → Review streak → Log mission log entry
Sunday    → Strategy day → Weekly review + plan next week
```

### Weekly Cycle
- **Mon–Sat**: 5 active systems with interconnected tasks
- **Sunday**: Strategy day — revision, mixed problems, planning, documentary
- **Goal**: Maintain daily completion for streak bonuses (+5 XP per day beyond day 2)

---

## 🏗️ Architecture

```
index.html  (single file — ~87KB)
│
├── CSS Variables (Pure Minimal White theme)
├── Particle field canvas background
│
├── HTML Structure
│   ├── Mission card
│   ├── Health strip
│   ├── XP panel + rank badge
│   ├── 5-card metrics bar
│   ├── 6-tab nav
│   └── Tab panels (Tracker / Planner / Charts / Badges / Resources / STK)
│
└── JavaScript (vanilla, no libraries)
    ├── State management (localStorage key: cosmicos_v1)
    ├── XP + rank engine
    ├── Streak calculator
    ├── Render functions (per tab)
    ├── Achievement checker (12 badges)
    ├── STK phase engine (5 phases)
    └── Responsive particle field animation
```

---

## 🚀 Getting Started

### Option 1 — GitHub Pages (recommended)
```
1. Fork or download this repo
2. Make sure the file is named index.html
3. Go to Settings → Pages → Source → main branch
4. Your site: https://yourusername.github.io/cosmic-os
```

### Option 2 — Local
```
1. Download index.html
2. Open in any browser
3. That's it — no setup needed
```

> All data is saved to `localStorage` automatically. Nothing leaves your browser.

---

## 📚 Systems & Curriculum

### System 1 — Core (Maths + Physics) `#333`
| Task | XP |
|------|----|
| Maths — 1.5 hr morning deep work | +15 |
| Physics — 1.5 hr morning deep work | +15 |
| Physics numericals / derivations — 1 hr | +10 |
| Maths practice — 45 min | +8 |

### System 2 — German A1 → A2 → B1 `#555`
| Task | XP |
|------|----|
| Vocabulary — 15–20 new words (Anki) | +6 |
| Grammar study — 30 min | +8 |
| Write 5–10 sentences | +6 |
| German listening — 20 min | +6 |
| Speak aloud — shadowing / recording | +7 |

### System 3 — Mind (Psychology + Philosophy) `#888`
| Task | XP |
|------|----|
| Psychology / Philosophy — 30 min | +5 |
| Astronomy reading / video — 20 min *(optional)* | +5 |

### System 4 — Python + ML `#777`
| Task | XP |
|------|----|
| Python practice — 30 min | +8 |
| Star Classifier / Binary Star project | +12 |
| Astronomy coding *(optional)* | +10 |

### System 5 — Luxastra Lab (Startup) `#aaa` — Low priority
| Task | XP |
|------|----|
| Research idea / niche — 30 min | +5 |
| Improve website / design | +5 |
| Brainstorm features | +4 |
| Market research | +4 |
| Write ideas / notes | +3 |

### Sunday — Strategy Day
| Task | XP |
|------|----|
| Revise whole week | +10 |
| German weekly review | +8 |
| Mixed Maths + Physics questions | +10 |
| Watch astronomy documentary | +5 |
| Plan next week | +8 |
| Progress check | +5 |

---

## 🏆 XP & Rank System

### Rank Table
| Rank | Level | XP Required | XP to Next |
|------|-------|-------------|------------|
| Cadet | 1 | 0 | 100 |
| Observer | 2 | 100 | 150 |
| Explorer | 3 | 250 | 250 |
| Navigator | 4 | 500 | 400 |
| Astronomer | 5 | 900 | 600 |
| Astrophysicist | 6 | 1500 | MAX |

### Bonus XP
- **3-day streak**: +5 XP per day beyond day 2
- **Consistent daily study**: compounds over weeks

### Daily max XP (approx)
- Full Core + German + Python + Mind day: ~**101 XP**
- Sunday strategy day: ~**54 XP**

---

## 🧩 Modules

### Achievement Badges (12 total)
| Badge | Icon | Condition |
|-------|------|-----------|
| First step | 🌱 | Complete any task |
| 3-day streak | 🔥 | 3 consecutive study days |
| 7-day warrior | ⚡ | 7 consecutive study days |
| 100 XP earned | 💯 | Reach 100 total XP |
| 500 XP club | ⭐ | Reach 500 total XP |
| Astrophysicist | 🏆 | Reach 1500 XP (max rank) |
| Guten Morgen | 🇩🇪 | Complete a full German system day |
| Physics beast | ⚛ | Complete a full Core system day |
| STK started | 🎓 | Complete any STK task |
| India ready | ✈️ | Complete all Phase 1 STK tasks |
| Strategist | 🗓 | Complete a full Sunday review |
| On a mission | 🎯 | Complete today's main focus |

### 🇩🇪 Studienkolleg Phases
| Phase | Label | Color |
|-------|-------|-------|
| 01 | Preparation in India | Indigo |
| 02 | Application to Studienkolleg | Sky blue |
| 03 | Visa + Arrival in Germany | Emerald |
| 04 | T-Kurs Year at Studienkolleg | Amber |
| 05 | Feststellungsprüfung (FSP) | Red |

---

## 💾 Data & Storage

All data is stored in **browser localStorage** under the key `cosmicos_v1`.

### Storage schema
```
cosmicos_v1 = {
  // Daily tasks
  "w{week}d{day}_{taskId}": true/false,

  // Weekly reflections
  "ref_w{week}d{day}": "string",

  // Resource library
  "res_{resourceId}": "none" | "active" | "done",

  // STK tasks
  "stk_{taskId}": true/false,

  // STK deadlines
  "stkdl_{deadlineId}": true/false,

  // STK resources
  "stkrs_{resourceId}": "none" | "using" | "done",

  // Daily mission
  "mission_{yyyy}_{m}_{d}_text": "string",
  "mission_{yyyy}_{m}_{d}_done": true/false,

  // Weekly planner
  "plan_w{week}_d{day}": "string"
}
```

### Resetting data
Open browser DevTools → Application → Local Storage → Delete `cosmicos_v1`

---

## 🌐 Browser Support

| Browser | Support |
|---------|---------|
| Chrome / Brave | ✅ Full |
| Firefox | ✅ Full |
| Safari (iOS) | ✅ Full |
| Edge | ✅ Full |
| Add to Home Screen (iOS/Android) | ✅ Works as PWA-like app |

---

## 📱 Responsive Design

- **Mobile (< 600px)**: 2-col metrics, scrollable nav, compact cards, stacked mission
- **Tablet (600–900px)**: Standard layout
- **PC (> 900px)**: Wider container, larger typography, more breathing room

---

## 🔭 About the Builder

**Abhishek Pandey** — HSC graduate from Nagpur, Maharashtra. Astronomy & astrophysics enthusiast, science communicator, and co-founder of Luxastra Lab.

- Instagram: [@abhi.astrophysics](https://instagram.com/abhi.astrophysics)
- Portfolio: [ap6635514.github.io](https://ap6635514.github.io)
- LinkedIn: [abhishek-pandey-034a732a1](https://linkedin.com/in/abhishek-pandey-034a732a1)

> *"Discipline over motivation. Consistency over intensity. Stars over everything."*

---

## 📄 License

Personal use. Built with ❤️ for one mission: **Nagpur → Germany → Stars**.
