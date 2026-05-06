# ARCADE OPS: EXCEL QUEST — v2

> **Un univers gamificat care combină puzzle-uri Excel, prioritizare operațională și un hub arcade futurist într-o experiență single-file.**

Built by Laura Andreea — RO/EN bilingual portfolio project demonstrând product thinking, UX design, frontend engineering și visual identity.

---

## 📦 Structura proiectului

```
arcade-ops-excel-quest/
├── index.html       # Aplicația principală (~232KB, 6,500+ linii)
├── about.html       # Landing page de prezentare pentru recruiteri
└── README.md
```

**Zero dependențe externe.** Două fișiere HTML self-contained.

---

## ⚡ Ce e nou în v2

### 🔊 Sound design
Engine audio sintetizat cu **Web Audio API** — zero fișiere externe:
- Click-uri subtile pe butoane
- Arpeggii ascendente la success
- Combo escalation (frequency creste cu combo-ul)
- Boss hit cu noise burst
- Rank-up flourish (4 note triumfătoare)
- Buton de mute în HUD (♪ / ⊘)

### 🔥 Daily Challenges + Streak System
- **3 provocări noi** generate determinist din data zilei
- Streak counter cu **bonus XP până la +50%**
- Timer real-time până la reset
- 6 tipuri de challenges: triage perfect, formula streak, workflow first-try, combo, missions count, high score

### ✨ Customization Station
- **6 avatar skins** unlock-abile cu coins (Neon Clasic, Cyan Pulse, Lime Circuit, Amber Flame, Gold Elite, Prizm Master)
- **5 neon themes** (Magenta Ops, Cyber Blue, Toxic Lime, Sunset Hunt, Matrix Green)
- Theme-ul schimbă paleta întregului joc **live** (CSS variables)
- Avatar-ul se aplică și în Hub și în Profile

### 📚 Conținut extins
- Triage Rush: **12 → 25 task-uri** (Stripe webhook, GDPR, vendor disputes, DDoS, etc.)
- Formula Lab: **8 → 21 puzzle-uri** (VLOOKUP, INDEX-MATCH, ROUND, MAX, IFERROR, LEN, TEXT, TRIM, TODAY, LEFT/RIGHT, AND/OR, COUNTIF criteria)

### 🎓 Onboarding tutorial
Overlay 5-step pentru first-time users:
1. Welcome → context-ul jocului
2. Triage Rush → 4 acțiuni + keyboard shortcuts
3. Formula Lab → puzzle-uri + tipuri
4. Progression → XP, ranks, combo
5. Districts & Boss → world map + Queue Hydra

Skip option oricând. Detectează automat first-time vs returning user.

### 🌐 Landing page (`about.html`)
Pagină separată orientată spre recruiteri:
- Hero cu shimmer animation
- 4 pillars (concept overview)
- 9 systems (toate feature-urile)
- 4 skill columns (Product / UX / Frontend / Visual)
- Tech stack badges
- CTA card
- Mobile responsive

---

## 🎮 Mecanici principale

| Modul | Conținut | Mecanică |
|-------|----------|----------|
| **Triage Rush** | 25 task-uri | Resolve / Escalate / Defer / Assign |
| **Formula Lab** | 21 puzzle-uri | Multiple choice cu hints |
| **Workflow Builder** | 5 procese | Drag-to-reorder steps |
| **Crisis Room** | Mixed mode | Triage + boss elements |
| **Boss: Queue Hydra** | 3 faze | Multiplicare la greșeală |

---

## 🎯 Progresie

- **8 ranguri** de la Trainee → Master Operator
- **12 achievement-uri** (badges)
- **6 districte** unlock-abile progresiv
- **XP + Coins** economy
- **localStorage** persistence (key: `arcade-ops-excel-quest-v1`)

---

## ⌨️ Keyboard shortcuts

**Triage Rush:** `1` `2` `3` `4` (sau `R` `E` `D` `A`)
**Formula Lab:** `A` `B` `C` `D` (sau `1-4`)
**Global:** `Esc` pentru exit

---

## 🚀 Deployment pe GitHub Pages

1. Creează repo nou: `arcade-ops-excel-quest`
2. Push ambele fișiere (`index.html` și `about.html`)
3. Settings → Pages → Source: `main` branch, root folder
4. Demo va fi disponibil la: `https://laurandreea10.github.io/arcade-ops-excel-quest/`
5. Landing page la: `https://laurandreea10.github.io/arcade-ops-excel-quest/about.html`

**Pentru CV/LinkedIn:** trimite link-ul către `about.html` (este orientat spre cititor) și include și link-ul direct către `index.html` pentru cei care vor să joace direct.

---

## 🛠️ Tech stack

- HTML5 / CSS3 / Vanilla JavaScript
- Web Audio API (SFX)
- localStorage (persistence)
- CSS custom properties (theming)
- Google Fonts (Orbitron, Rajdhani, JetBrains Mono)
- Zero build tools, zero npm packages

---

## 📊 Metrici

- **~232 KB** un singur fișier (index.html)
- **~22 KB** landing page (about.html)
- **6,500+** linii de cod
- **0** dependențe externe
- **2** limbi (RO + EN)
- **51** task-uri și puzzle-uri unice
