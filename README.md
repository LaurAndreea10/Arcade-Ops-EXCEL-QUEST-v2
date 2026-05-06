# ARCADE OPS: EXCEL QUEST

> Un univers gamificat care combină puzzle-uri Excel, prioritizare operațională și un hub arcade futurist. Single-file HTML/CSS/JS — zero dependențe, zero build.

**Live demo:** https://laurandreea10.github.io/arcade-ops-excel-quest

---

## Concept

Joci ca un **Operator** într-un HQ digital neon. Misiunea: prioritizezi task-uri, repari formule Excel, optimizezi workflow-uri și lupți cu boss-uri pentru a avansa de la `TRAINEE` la `MASTER OPERATOR`. Un univers care arată simultan game design, UX systems, progression design și product thinking.

## Ce conține

**Hub & Navigation**
- Splash screen cu animații neon
- HQ Hub central cu player card, world map, mission terminal, live feed
- HUD persistent cu rank, XP, coins
- Profile screen cu stats, mastery bars și 12 achievements

**Mini-games funcționale**
- **Triage Rush** — 12 task-uri reale (incidents, requests, bugs), 4 acțiuni (Resolve / Escalate / Defer / Assign), timer, combo system, queue preview
- **Formula Lab** — 8 puzzle-uri Excel cu mock spreadsheet, formula bar și 4 răspunsuri multiple. Acoperă SUM, IF, COUNTIF, AVERAGE, XLOOKUP, SUMIF, CONCAT
- **Workflow Builder** — 5 procese reale de aranjat (onboarding client, procesare factură, bug fix, marketing campaign, recrutare)
- **Crisis Room** — mod combinat, intens, time-pressured
- **Boss Battle: The Queue Hydra** — 3 faze, stability bar, mecanica de "multiplicare" la greșeli

**Sisteme**
- 8 ranks: Trainee → Master Operator
- 12 achievements cu condiții reale
- Progresie pe districte cu unlock-uri condiționate
- Mastery tracking pe 4 categorii
- LocalStorage persistent (state survive la refresh)
- Bilingv RO/EN (toggle live)

**Game feel**
- Scoring multi-strat: base + combo + speed bonus + perfect bonus
- Combo bursts, score popups, screen shake la greșeli
- Toast notifications pentru rank-ups și badges
- Keyboard shortcuts (1/R, 2/E, 3/D, 4/A pentru triage; A/B/C/D pentru formula; Esc pentru exit)

## Stack

- **HTML/CSS/JS pur** într-un singur fișier (~165KB)
- Fonts: Orbitron + Rajdhani + JetBrains Mono (Google Fonts)
- Zero build step, zero dependencies
- Funcționează offline după prima încărcare

## Deploy pe GitHub Pages

```bash
# 1. Clonează / creează repo
git init
git add index.html README.md
git commit -m "ARCADE OPS: EXCEL QUEST initial"

# 2. Push pe GitHub (creează un repo nou: arcade-ops-excel-quest)
git remote add origin https://github.com/LaurAndreea10/arcade-ops-excel-quest.git
git branch -M main
git push -u origin main

# 3. În repo Settings → Pages → Source: main / root → Save
# 4. Live la: https://laurandreea10.github.io/arcade-ops-excel-quest
```

## Structura proiectului

```
arcade-ops-excel-quest/
├── index.html    # Tot proiectul într-un singur fișier
└── README.md     # Acest fișier
```

## Keyboard shortcuts

| Acțiune | Tastă |
|---|---|
| Triage / Boss: Resolve | `1` sau `R` |
| Triage / Boss: Escalate | `2` sau `E` |
| Triage / Boss: Defer | `3` sau `D` |
| Triage / Boss: Assign | `4` sau `A` |
| Formula Lab: răspuns A/B/C/D | `1`-`4` sau `A`-`D` |
| Exit oricând | `Esc` |

## Decizii de design

- **Single-file** — pentru rapiditate de iterare și ușurință de share. Tot proiectul stă într-un fișier, exact ca BASKET-VS-AI și NEXUS ARCADE.
- **Neon arcade + dark mode dashboard** — paletă cyan / magenta / electric purple / lime, font display Orbitron, mono JetBrains Mono. Mix între cabinet de arcade și SaaS dashboard premium.
- **RO-first cu EN toggle** — UI-ul nativ în română, toate task-urile / puzzle-urile / explicațiile traduse în ambele limbi.
- **Conținut realist** — task-urile de triage sunt scenarii reale (P1 outage, GDPR risk, vendor invoice, etc.), nu placeholder-uri. Puzzle-urile Excel acoperă funcții pe care le folosești zilnic.
- **Progression-driven, nu gating-driven** — districtele se deblochează prin progres, nu sunt blocate artificial cu paywall-uri.

## License

MIT — folosește, fork-uiește, învață din el.

---

**Built by [Laura Andreea](https://github.com/LaurAndreea10)** • Part of the [CodePen Portfolio](https://laurandreea10.github.io/codepen-portfolio/) collection.
