# 🏛️ VNIT BuilderBase — Constant Design Principles & Master Design System
*The canonical design specification, aesthetic philosophy, color tokens, typographic scales, micro-interaction physics, and component blueprints used across VNIT BuilderBase.*

---

## 🧭 1. Executive Philosophy: The "Architectural Foundry" Aesthetic

VNIT BuilderBase was engineered to deliberately break away from generic, forgettable web design. It is built on three unbreakable tenets:

### 1.1 The "Anti-AI-Slop" Doctrine
Subreddits like `r/web_design`, `r/UI_Design`, and `r/Frontend` highlight an acute "banner blindness" toward websites that look AI vibe-coded. 
* **NO Purple/Violet Gradients:** Overused by LLMs and crypto templates. Signals low-effort or generic SaaS.
* **NO Blurry Glassmorphism:** Heavy frosted-glass cards destroy text contrast and strain the user's eyes.
* **NO Neon Cyberpunk Outlines:** Pitch-black backgrounds with glowing neon borders feel sterile and cause optical halation.
* **NO Generic 3-Card Grids:** Three centered cards with icons and corporate buzzwords (*"Speed, Quality, Scale"*) immediately betray a lack of thoughtful design.

### 1.2 The Architectural Foundry Metaphor
VNIT is one of India's premier engineering institutions, deeply rooted in civil, mechanical, metallurgical, and electrical foundations. The design reflects this heritage:
* **The Canvas:** Warm stone, tactile architectural drawing paper, precision blueprints.
* **The Ink:** High-contrast carbon ink (WCAG AAA compliant), crisp hairline 1px borders, and technical mono telemetry.
* **The Accent (10% Rule):** Burnished technical amber (`#D97706`). Like a high-visibility laser level in an architectural studio—used strictly for focused user actions, never for decorative clutter.

### 1.3 The 60-30-10 Rule in Practice
* **60% Dominant Base:** Warm Canvas Stone (`#FBFBF9`) and Crisp Elevated Card White (`#FFFFFF`). Lets the company logos and text breathe without glare.
* **30% Structural Chrome:** Hairline borders (`#E4E4E7` / `#D4D4D8`), Zinc ink hierarchy (`#18181B` to `#71717A`), and technical monospace data rails.
* **10% Focal Accent:** Burnished Amber (`#D97706`), reserved solely for active filter tabs, primary CTA buttons, typing carets, and key status signals.

---

## 🎨 2. Master Color System & Exact Hex Tokens

All color tokens are functionally categorized. Never mix semantic signals with decorative whims.

### 2.1 Surfaces & Canvas (60%)
| Token Name | Hex Code | RGB | Purpose & Placement |
| :--- | :--- | :--- | :--- |
| `--surface-canvas` | `#FBFBF9` | `rgb(251, 251, 249)` | Master background canvas (warm stone, paper texture). Eliminates pure `#FFFFFF` monitor glare. |
| `--surface-card` | `#FFFFFF` | `rgb(255, 255, 255)` | Elevated card surface (startup cards, modal dialogs, toolbar inputs). |
| `--surface-card-subtle` | `#FBFBF9` | `rgb(251, 251, 249)` | Secondary panel surface (support panel in dock, subtle nested cards). |
| `--surface-elevated` | `#F4F4F0` | `rgb(244, 244, 240)` | Shaded sub-canvas (ecosystem dock, footer background, milestone tracks). |
| `--surface-footer` | `#F8FAFC` | `rgb(248, 250, 252)` | Shaded card footer bar (houses alumni chips and city tag). |

---

### 2.2 Ink Hierarchy (WCAG AAA Tested)
| Token Name | Hex Code | Zinc / Slate Scale | Purpose & Usage |
| :--- | :--- | :--- | :--- |
| `--ink-primary` | `#18181B` | Deep Carbon (Zinc 900) | Primary headlines, company names, modal titles, high-emphasis metrics. |
| `--ink-secondary` | `#3F3F46` | Warm Zinc 700 | Body paragraphs, 2-line startup elevator pitches, secondary labels. |
| `--ink-muted` | `#71717A` | Warm Zinc 500 | Metadata, branch subtitles, search icons, counter labels, timestamps. |
| `--ink-subtle` | `#A1A1AA` | Warm Zinc 400 | Border hints, subtle placeholders, disabled states, divider dots. |

---

### 2.3 Crisp 1px Hairline Border System
In modern software design, **crisp hairline borders create physical grounding** that soft blurry shadows cannot replicate.

| Token Name | Hex Code | Application |
| :--- | :--- | :--- |
| `--border-subtle` | `#E4E4E7` | Subtle internal section dividers, table rows, input boundaries. |
| `--border-card` | `#D4D4D8` / `#CBD5E1` | Standard card outer bounding stroke (1px solid). |
| `--border-hover` | `#18181B` | High-contrast card hover stroke, signaling active cursor focus. |

---

### 2.4 Brand & Interaction Accent System (Burnished Amber - 10%)
| Token Name | Hex Code | Role in Interface |
| :--- | :--- | :--- |
| `--action-primary` | `#D97706` | Primary action buttons (`Submit Your Startup`), active filter bar, typing caret. |
| `--action-primary-hover` | `#B45309` | Hover state on primary buttons, active interactive states. |
| `--cobalt-tint-bg` | `#FEF3C7` | Soft amber tint background for badges, active filter tabs, batch pills. |
| `--cobalt-tint-border` | `#FDE68A` | Hairline border framing amber badges and active tabs. |
| `--cobalt-tint-text` | `#92400E` | High-contrast readable dark amber text inside badges. |

---

### 2.5 Semantic Functional Signals (Status & Third-Party)
| Signal | Tokens & Hex Codes | Visual Meaning |
| :--- | :--- | :--- |
| **Live Pulse / Verified** | Background: `#ECFDF5`<br>Border: `#A7F3D0`<br>Text: `#065F46`<br>Pulse Dot: `#10B981` | Real-time active status, telemetry live dot, verified company badges. |
| **Bootstrapped / Milestone** | Background: `#FFFBEB`<br>Border: `#FDE68A`<br>Text: `#92400E` | Bootstrapped startup indicator, heritage callouts, warning notices. |
| **LinkedIn Outbound** | Button: `#0A66C2`<br>Hover: `#004182`<br>Border: `#0855A3`<br>Text: `#FFFFFF` | Direct founder profile connect button. High-contrast, authentic brand recognition. |
| **Support / Heart** | Icon: `#E11D48`<br>Hover Bg: `#FFF1F2`<br>Border: `rgba(225, 29, 72, 0.28)` | GitHub sponsor / community support button. |
| **Location Pin** | Pin SVG: `#EF4444`<br>Container: `#F1F5F9`<br>Text: `#18181B` | City & hub indicator on startup cards. |

---

### 2.6 Department Leaderboard Color Palette
Each department has an assigned gradient or tone that represents its engineering identity:
* **CSE (Computer Science):** `linear-gradient(90deg, #B45309 0%, #D97706 70%, #F59E0B 100%)` (Burnished Amber)
* **ECE (Electronics & Comm):** `linear-gradient(90deg, #C2410C 0%, #EA580C 100%)` (Deep Orange)
* **EEE (Electrical & Electronics):** `linear-gradient(90deg, #A16207 0%, #CA8A04 100%)` (Technical Ochre)
* **Civil Engineering:** `#047857` (Foundational Deep Emerald)
* **Mining Engineering:** `#92400E` (Earthy Rich Ochre)
* **Mechanical / MME / Architecture / Chemical:** `#71717A` (Industrial Zinc Muted)

---

## 🔤 3. Typographic Engine & Font System

VNIT BuilderBase pairs **three distinct typefaces**, each serving an intentional structural purpose:

```
┌────────────────────────────────────────────────────────────────────────┐
│ 1. Plus Jakarta Sans : Primary UI Grotesque (Clarity, Headers, Body)   │
│ 2. JetBrains Mono    : Technical Telemetry, Dates, Badges, Tabular Data│
│ 3. Instrument Serif  : Editorial Italic Accent ("Built by VNITians")   │
└────────────────────────────────────────────────────────────────────────┘
```

### 3.1 Font Families
* **`--font-primary`:** `'Plus Jakarta Sans', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif`
  * *Why:* Crisp geometric structure with humanist warmth. Superior legibility at 11–13px on mobile screens.
* **`--font-mono`:** `'JetBrains Mono', ui-monospace, Menlo, Monaco, Consolas, monospace`
  * *Why:* Engineered for high scannability. Used for batch years (`'19`), percentage shares (`20.0%`), rank tags (`01`), and timestamps. Always paired with `font-feature-settings: 'tnum'` (tabular numbers).
* **Editorial Accent Font:** `'Instrument Serif', Georgia, serif` *(Italic, Weight: 400)*
  * *Why:* Used as an **editorial punctuation** in the hero headline for the single word *"Built"*. Creates the high-status Stripe/Linear aesthetic by breaking geometric monotony.

---

### 3.2 Master Type Scale & Component Matrix

| UI Component | Font Family | Size | Weight | Line Height | Letter Spacing | Case |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **Hero Main Headline** | Plus Jakarta Sans | `clamp(38px, 4.2vw, 54px)` | 800 (Bold) | `1.12` | `-1.6px` | Normal |
| **Editorial Accent ("Built")**| Instrument Serif | `1.12em` | 400 (Italic)| Normal | `-0.01em` | Normal |
| **Navbar Brand Title** | Plus Jakarta Sans | `19px` (Mob: 16.5px)| 800 (Bold) | `1.0` | `-0.03em` | Normal |
| **Navbar Campus Tag** | Plus Jakarta Sans | `12px` | 700 (Bold) | `1.0` | `+0.14em` | UPPERCASE |
| **Startup Card Title** | Plus Jakarta Sans | `18.5px` (Mob: 16px)| 800 (Bold) | `1.18` | `-0.02em` | Normal |
| **Elevator Pitch** | Plus Jakarta Sans | `13px` (Mob: 12.5px)| 500 (Reg) | `1.48` | `-0.01em` | Normal |
| **Batch / Branch Badges** | JetBrains Mono | `10px` | 600 (Med) | `1.0` | Normal | Normal |
| **Leaderboard Branch Code**| Plus Jakarta Sans | `12.5px` | 800 (Bold) | `1.1` | `-0.01em` | UPPERCASE |
| **Leaderboard Metrics** | JetBrains Mono | `9px` / `12.5px` | 700 (Bold) | `1.1` | Normal | Tabular |
| **Filter Section Header** | Plus Jakarta Sans | `10.5px` | 700 (Bold) | `1.0` | `+0.8px` | UPPERCASE |
| **Filter Item Label** | Plus Jakarta Sans | `11.5px` | 600 (Med) | `1.25` | Normal | Normal |
| **Footer Legal Links** | JetBrains Mono | `11px` | 500 (Reg) | `1.0` | Normal | Normal |
| **Byline Attribution** | JetBrains Mono | `11.5px` | 700 (Bold) | `1.0` | Normal | Normal |

---

## 📐 4. Spacing, Radii & Surface Depth Architecture

### 4.1 Border Radii
* `--radius-sm`: **`4px`** — Precision rank badges (`01`), facet counts, technical chips.
* `--radius-md`: **`6px`** — Primary buttons (`.btn-submit`), startup cards (`.venture-card`), form inputs.
* `--radius-lg`: **`8px`** — Modal panels, filter containers, search bar wrappers.
* `--radius-xl`: **`12px`** — Ecosystem dock cards, drawer headers, mobile bottom sheets.
* `--radius-pill`: **`9999px`** — Live status pills, telemetry badges, avatar chips.

### 4.2 Elevation Shadows
* `--shadow-sm`: `0 1px 2px rgba(24, 24, 27, 0.04)` — Resting state for cards and inputs.
* `--shadow-md`: `0 4px 14px rgba(24, 24, 27, 0.08)` — Card hover elevation and dropdowns.
* `--shadow-lg`: `0 12px 36px -6px rgba(24, 24, 27, 0.12)` — Sticky navigation bars and floating tooltips.
* `--shadow-selected`: `0 8px 24px -4px rgba(217, 119, 6, 0.16)` — Active card state with warm amber glow.

---

## 🧩 5. Component-by-Component Design Blueprints

### 5.1 The Sticky Navbar
* **Background:** `rgba(248, 250, 252, 0.94)` with `backdrop-filter: blur(12px)`.
* **Border:** 1px hairline bottom border (`#E4E4E7`).
* **Brand Lockup:**
  - `VNIT` tag: `#94A3B8`, letter-spacing `0.14em`, right border `1.5px solid #CBD5E1`.
  - `BUILDERBASE` title: `#0F172A`, weight 800, with `BASE` highlighted in burnished amber (`#F97316`).
* **Live Status Pill:** `#ECFDF5` background with emerald text and an SVG animated pulse dot (`#10B981`, 2s loop).
* **CTAs:**
  - `Submit Your Startup`: Primary amber button (`#D97706`). Triggers a pulse ripple cue (`submitCue`) if the user returns to the top after scrolling through the entire feed.
  - Heart Support Button: `31x31px` circular button with `#E11D48` border and heart icon.

---

### 5.2 The Hero Section & Ambient Glacial Aurora
* **Canvas:** Pure white background (`#FFFFFF`) with zero harsh grids or polka dots.
* **Ambient Lighting:** 3 Gaussian-blurred radial orbs (`blur: 140px`) drifting on prime-number cycle durations (`29s`, `37s`, `43s`). Prime numbers ensure the gradient movement **never repeats noticeably**.
* **Anti-Banding Shield:** An ultra-subtle SVG fractal noise overlay (opacity: `2.2%`, mix-blend-mode: `overlay`) eliminates color banding on 8-bit displays.
* **Interactive Cursor Wake:** A dynamic 680px spotlight follows the mouse coordinates (`var(--mouse-x)`, `var(--mouse-y)`), gently illuminating text surfaces.
* **Typing Animation:** A snappy typing caret (`#D97706`, `width: 3px`) blinks every `0.75s` next to alternating dynamic keywords (*Startups*, *Companies*, *Products*).
* **Live Telemetry Pill:**
  - Floating pill: `rgba(255, 255, 255, 0.78)` with `backdrop-filter: blur(10px)`.
  - Content: `750 Unique Visitors • 2,215 Views`.
  - Live indicator: Pulsing `#10B981` dot with an expanding ripple ring.

---

### 5.3 The 9-Department Founder Leaderboard
* **Visual Metaphor:** An architectural blueprint telemetry panel displaying branch volume and percentage share.
* **Structure:**
  - Header: 4 columns (`Rank`, `Department`, `Track`, `Count & Share`).
  - Rows: Highlighted top-tier leaders with subtle amber hover tint (`rgba(217, 119, 6, 0.05)`).
  - Segmented Track: Milestone hash marks positioned precisely at **25%, 50%, and 75%** width.
* **Desktop Cursor Inspector (`.branch-hover-inspector`):**
  - An Apple-style floating tooltip (`width: 224px`, `blur: 24px saturate(190%)`) that glides with the cursor when hovering over leaderboard rows.
  - Displays the full department name, verified startup count, campus percentage share, and top alumni names.

---

### 5.4 The Startup Card (Stage 1 Card Component)
* **Architecture:** 75-Unit Calibrated List View.
* **Dimensions & Padding:** `padding: 15px 18px`, gap `16px`.
* **Company Logo Tile:**
  - `66x66px` crisp white tile with hairline border and subtle shadow.
  - Image: `object-fit: contain`. Hover effect scales logo by `1.04x`.
* **Clamped Elevator Pitch:**
  - 2 lines clamped (`-webkit-line-clamp: 2`).
  - Min-height strictly reserved (`calc(2 * 1.48em)`) so cards **never shift vertically or bounce** when filters or drawers open.
* **High-Catch Action Button:**
  - Direct LinkedIn connect button: `#0A66C2` with white LinkedIn icon.
  - Prominently positioned on the top right for instant 1-click reachouts.
* **Verified Alumni Footer Bar (`#F8FAFC`):**
  - Displays alumni founder chips: circular 22px avatar, founder name, graduation year (`'16`), and department code (`CSE`).
  - Location tag: Shaded gray badge with a `#EF4444` location pin.
* **Active Selected State:**
  - Uses an **inset 3.5px amber bar** (`box-shadow: inset 3.5px 0 0 #D97706`).
  - *Why:* Never uses thick outer borders that push neighboring content laterally.

---

### 5.5 The In-Place Inspection Drawer (Stage 2 Component)
* **Desktop:**
  - An in-place sliding sheet (`width: 380px`) anchored to the right of the feed.
  - The feed narrows gracefully (`transition: flex 0.28s`) without hiding the user's scroll position or dimming the background.
  - Drag Handle: A 4px vertical grip bar on the left allows dragging to dismiss.
* **Mobile (Native Bottom Sheet):**
  - Hardware-accelerated sliding sheet (`translate3d(0, 100%, 0)`) anchored to the bottom.
  - Top handle pill (`42x5px`, `#CBD5E1`).
  - Max height: `86dvh` with smooth momentum scrolling.

---

### 5.6 The Mobile Two-Way Filter Drawer
* **Problem Solved:** Long accordion filter lists force endless scrolling on mobile.
* **Architecture:**
  - **Left Rail (38% width, `#F8FAFC`):** Displays category tabs (*Branch*, *Sector*, *City*, *Year*) with item count badges. Active tab has an amber left accent bar.
  - **Right Rail (62% width, `#FFFFFF`):** Displays selectable checkboxes for the active category.
  - Selected options highlight in warm amber (`#FEF3C7`) with bold checkmarks (`✓`).
* **Continuous Scroll Lock:** Background document is strictly locked (`overflow: hidden; touch-action: none`) when the drawer is open to prevent background scrolling.

---

### 5.7 The "Quiet Builder" Footer & Maker Attribution
* **Design Rationale:** Placing creator credit in the hero section is perceived as narcissistic. True craft speaks through the product first.
* **Byline Placement:**
  - Quiet, understated monospace line in the footer: `Designed & built by Nandan`.
  - Clicking `Nandan` opens the interactive **Maker Modal**.
* **Maker Modal Architecture:**
  - 3-part layout: Identity & Origin, Mission statement (framing BuilderBase as a selfless campus initiative), and clean social links (X, LinkedIn, Mail).

---

## ⚡ 6. Animation Physics & Micro-Interactions

| Interaction | Duration | Timing Function | Visual Sensation |
| :--- | :--- | :--- | :--- |
| **Primary State Transitions** | `0.18s` – `0.22s` | `cubic-bezier(0.16, 1, 0.3, 1)` | Linear/Apple fluid deceleration. Snappy, immediate, zero drag. |
| **Drawer Slide-Out** | `0.26s` – `0.34s` | `cubic-bezier(0.22, 1, 0.36, 1)` | Weighted mechanical sheet sliding out on tracks. |
| **Mobile Sheet Slide-Up** | `0.32s` | `cubic-bezier(0.2, 0.9, 0.2, 1)` | Native iOS/Android bottom sheet momentum. |
| **Card Press Effect** | `0.09s` | `ease` | `transform: scale(0.988)` tactile mechanical depression. |
| **Live Pulse Ripple** | `2.0s` | `cubic-bezier(0.4, 0, 0.6, 1)` (Infinite) | Organic respiration, indicating live telemetry. |
| **Ambient Orbs** | `29s`, `37s`, `43s`| `ease-in-out` (Infinite alternate) | Deep celestial drift with zero perceptible loop seam. |

---

## 📋 7. Quick-Reference Copy-Paste CSS Variables

```css
:root {
  /* FONT STACK */
  --font-primary: 'Plus Jakarta Sans', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
  --font-mono: 'JetBrains Mono', ui-monospace, Menlo, Monaco, Consolas, monospace;

  /* SURFACES */
  --surface-canvas: #FBFBF9;
  --surface-card: #FFFFFF;
  --surface-card-subtle: #FBFBF9;
  --surface-elevated: #F4F4F0;
  --surface-footer: #F8FAFC;

  /* INK HIERARCHY (WCAG AAA) */
  --ink-primary: #18181B;     /* Zinc 900 */
  --ink-secondary: #3F3F46;   /* Zinc 700 */
  --ink-muted: #71717A;       /* Zinc 500 */
  --ink-subtle: #A1A1AA;      /* Zinc 400 */

  /* CRISP 1PX HAIRLINE BORDERS */
  --border-subtle: #E4E4E7;
  --border-card: #D4D4D8;
  --border-hover: #18181B;

  /* 10% VIBRANT INTERACTION TOKENS (BURNISHED TECHNICAL AMBER) */
  --action-primary: #D97706;
  --action-primary-hover: #B45309;
  --cobalt-tint-bg: #FEF3C7;
  --cobalt-tint-border: #FDE68A;
  --cobalt-tint-text: #92400E;

  /* SEMANTIC STATUS SIGNALS */
  --emerald-bg: #ECFDF5;
  --emerald-border: #A7F3D0;
  --emerald-text: #065F46;
  --emerald-dot: #10B981;

  /* ELEVATION & SHADOWS */
  --shadow-sm: 0 1px 2px rgba(24, 24, 27, 0.04);
  --shadow-md: 0 4px 14px rgba(24, 24, 27, 0.08);
  --shadow-lg: 0 12px 36px -6px rgba(24, 24, 27, 0.12);
  --shadow-selected: 0 8px 24px -4px rgba(217, 119, 6, 0.16);

  /* RADII */
  --radius-sm: 4px;
  --radius-md: 6px;
  --radius-lg: 8px;
  --radius-xl: 12px;
  --radius-pill: 9999px;
}
```

---

## 🏆 The 10 Golden Laws of Future Product Extensions

1. **Never use generic blue/purple buttons.** Every primary action is Burnished Technical Amber (`#D97706`).
2. **Never use pure black (`#000000`) or pure white (`#FFFFFF`) for background canvases.** Always ground the canvas on Warm Stone (`#FBFBF9`).
3. **Always use 1px hairline borders for depth.** Never rely on heavy, fuzzy drop shadows to separate cards.
4. **Never let dynamic content jump or bounce.** Always clamp and reserve height for text blocks (e.g. 2-line pitches).
5. **Pair geometric sans with an editorial accent.** Use *Instrument Serif Italic* sparingly for single-word editorial emphasis.
6. **Use Monospace for all telemetry and tabular data.** Graduation years, percentages, and counters must always use `JetBrains Mono` with `tabular-nums`.
7. **Keep mobile touch targets at or above 44px.** Buttons, filter rows, and close icons must never be cramped on touchscreens.
8. **Slide drawers inline on desktop; use bottom sheets on mobile.** Never force desktop users into full-screen modal overlays when comparing items.
9. **Never self-promote above the fold.** Keep maker credits humble, understated, and anchored in the footer. Let the product's craft earn the respect.
10. **Design for the 1.5-second triage.** Every view, card, or modal must answer: *What is this, who built it, and what single action can I take next?*
