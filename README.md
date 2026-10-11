# VNIT BuilderBase 🚀

> **The definitive discovery base of startups, products, and ventures built by VNIT alumni. Connect with founders in 1 click.**

[![License: MIT](https://img.shields.io/badge/License-MIT-amber.svg)](LICENSE)
[![Status: Production](https://img.shields.io/badge/Status-Production%20Ready-emerald.svg)](#)
[![Deployment: Vercel](https://img.shields.io/badge/Deploy-Vercel-black.svg?logo=vercel)](#)

---

## ⚡ Overview

**VNIT BuilderBase** is a community-driven discovery engine designed to bridge current students, alumni, and angel operators with companies and products built by graduates of **Visvesvaraya National Institute of Technology (VNIT), Nagpur**.

* **1-Click Founder Reach**: Instant verified LinkedIn, X (Twitter), and direct founder pitch drawers.
* **Engineering Department Telemetry**: Dynamic live leaderboard indexing venture distribution across departments (CSE, ECE, Mechanical, Electrical, Chemical, Civil, Metallurgy, Mining, Architecture).
* **Live In-Memory & Cloud Search**: Instant zero-latency search by founder name, company, sector tag, batch year, and technology stack.
* **Get Listed Pipeline**: 30-second submission portal for newly emerging alumni ventures with live receipt review.
* **Community Contributions**: Integrated support modal for hosting and infrastructure maintenance.

---

## 🛠️ Tech Stack & Architecture

* **Frontend**: Pure Vanilla HTML5 & CSS3 with modern Design Tokens.
* **Typography**: *Plus Jakarta Sans*, *Instrument Serif* (editorial kinetic verb), and *JetBrains Mono*.
* **State & Logic**: Pure Vanilla ES6+ Javascript (`js/app.js`) with responsive drawer orchestration.
* **Database & Submissions**: Supabase Postgres Backend with fallback offline JSON hydration (`data/seed_startups.json`).
* **Deployment**: Optimized for single-click deployment on **Vercel** (`vercel.json`).

---

## 📂 Project Structure

```text
├── index.html            # Core entry application & production layout
├── vercel.json           # Vercel routing, cache control & security headers
├── .gitignore            # Clean git configuration
├── LICENSE               # MIT Open Source License
├── README.md             # Project documentation
├── css/
│   └── style.css         # Complete design system, aurora mesh, & responsive styles
├── js/
│   └── app.js            # Reactive search, filters, modals, & submission engine
├── data/
│   ├── seed_startups.json           # Offline seed database
│   └── supabase_startups_import.csv # CSV structured data
└── assets/
    ├── logos/            # Company marks & brand assets
    └── Profile Pics/     # Verified founder profile imagery
```

---

## 🚀 Deployment to Vercel

1. Fork or push this repository to your GitHub account (`vnit-builderbase`).
2. Go to **[vercel.com/new](https://vercel.com/new)**.
3. Import your GitHub repository: `vnit-builderbase`.
4. Leave all build settings as default (**Framework Preset: Other**, Root Directory: `./`).
5. Click **Deploy**. Your app will be live with full SSL in under 20 seconds at:  
   `https://vnit-builderbase.vercel.app`

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
