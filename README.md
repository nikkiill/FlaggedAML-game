# Flagged — AML Detection Simulator

> An interactive browser-based simulation of how UK financial crime detection systems catch money laundering across all three stages: Placement, Layering, and Integration.

**[▶ Play Live](https://nikkiill.github.io/AML-Laundromat-Game/)** &nbsp;|&nbsp; Built by [Nikhil Shinde](https://linkedin.com/in/nikhil-shinde-55a0a210b) — KYC/AML Product Specialist

---

## What Is This?

You start with **£1,000,000 in criminal proceeds**. You have nine decisions across three stages to move it into the legitimate economy without triggering a Suspicious Activity Report.

Every choice maps to a real money laundering typology. Every detection alert references actual AML legislation. Every real-world case is drawn from regulatory enforcement records.

The game is not designed to teach you how to launder money. It is designed to show you — in five minutes — how detection systems think, why they catch what they catch, and what the regulated sector is actually up against.

---

## Features

- **Branching paths** — your Stage 1 choice affects heat levels and detection logic in Stage 2 and Stage 3. Choose smurfing and the branch network velocity flag follows you forward.
- **Heat system** — a real-time detection score (0–100%) built from cumulative risk across all three stages.
- **4-tier outcome engine** — Ghost / Escaped / Flagged / Caught, each with distinct regulatory consequences.
- **Efficiency score** — measures how much you cleaned relative to heat generated. The metric compliance teams actually care about.
- **NCA overlay** — fires when consent is refused under POCA 2002 s.335, with authentic case reference numbers and timestamps.
- **Surveillance cameras** — appear at heat thresholds (30% / 50% / 70% / 85%) as the system closes in.
- **Audit trail** — a live decision log tracking every choice, heat contribution, and stage.
- **Personalised share text** — one-click LinkedIn share that includes your exact route through the simulation.
- **Difficulty modes** — Analyst (standard thresholds) and Compliance Officer (heat multiplied, earlier SAR triggers).
- **NCA alarm sound** — fires on consent refusal via Web Audio API.
- **Mobile responsive** — fully playable on phones, where most LinkedIn traffic lands.

---

## Real Cases Referenced

| Case | Value | Typology Illustrated |
|---|---|---|
| NatWest — FCA Fine | £264.8m | Structuring / smurfing across branches |
| HSBC — US Settlement | $1.9bn | Cash-intensive business commingling |
| BNP Paribas — US Fine | $8.9bn | Trade-based value transfer / sanctions evasion |
| Panama Papers — Mossack Fonseca | 11.5m documents | Shell company layering / nominee directors |
| Tornado Cash — OFAC Sanctions | $7bn+ laundered | Cryptocurrency mixing / Travel Rule |
| Zamira Hajiyeva — NCA UWO | £22m at Harrods | Overseas property / unexplained wealth |
| Mansoor Mahmood Hussain — Conviction | £9.7m confiscated | Loan-back scheme / POCA s.335 |

---

## Regulatory Framework

Every detection alert in the simulation references real legislation and guidance:

- **POCA 2002** — Proceeds of Crime Act (ss.327–336, consent regime)
- **MLR 2017** — Money Laundering Regulations (EDD, CDD, SAR obligations)
- **FATF Typologies** — Recommendations 16, 20 and Trade-Based ML Report 2020
- **FCA Financial Crime Guide** — Chapters 2–3
- **JMLSG Guidance** — Parts I and II, 2023 edition
- **NCA Annual SARs Report 2024** — 901,255 SARs filed in 2023–24
- **Economic Crime Act 2022** — Register of Overseas Entities, UWOs
- **Wolfsberg Group** — Trade Finance Principles

---

## Technical Stack

| Layer | Detail |
|---|---|
| Language | Vanilla HTML / CSS / JavaScript — zero dependencies |
| Build | Single-file, no bundler, no framework |
| Deployment | GitHub Pages |
| Fonts | Outfit (UI) + JetBrains Mono (terminal elements) via Google Fonts |
| Audio | Web Audio API (NCA alarm) |
| Storage | None — no data is collected or stored |

The entire simulation is one `index.html` file (approximately 1,000 lines). No Node, no npm, no build step. Fork and open in a browser.

---

## How to Run Locally

```bash
git clone https://github.com/nikkiill/AML-Laundromat-Game.git
cd AML-Laundromat-Game
open index.html
```

No installation required.

---

## Background

This project was built from three years of direct experience as a KYC/AML Product Owner — sitting in typology reviews, reading FATF reports and NCA SAR data, and building detection logic into financial crime compliance products.

The gap between how compliance training describes money laundering and how detection systems actually experience it is significant. Most professionals working adjacent to financial crime have never felt what it looks like from the other side of the detection engine.

This simulation is an attempt to close that gap in five minutes.

---

## Data Sources

- NCA Financial Intelligence Unit — Annual SARs Report 2023–24
- FATF — Typologies and Guidance Documents (2020–2024)
- FCA — Financial Crime Guide (FCG), Enforcement Decisions
- JMLSG — Prevention of Money Laundering / Combating Terrorist Financing (2023)
- Companies House — PSC Register and Entity Data
- HMRC — High Value Dealer Registration and CITEX Trade Data
- Law Society — AML Guidance for Solicitors (2023)

---

## Author

**Nikhil Shinde** — Product & Operations Analyst | KYC/AML Product Specialist

- LinkedIn: [linkedin.com/in/nikhil-shinde-55a0a210b](https://linkedin.com/in/nikhil-shinde-55a0a210b)
- Portfolio: [nikhil2617shinde.netlify.app](https://nikhil2617shinde.netlify.app)

---

## Disclaimer

This project is an educational simulation built for awareness and professional development. All scenarios are hypothetical and based on publicly documented regulatory cases. No actual financial crime is facilitated, described in actionable detail, or encouraged.

---

*£100bn is laundered through the UK every year. Less than 1% of criminal money is ever seized globally. The gap between those two numbers is a product problem.*
