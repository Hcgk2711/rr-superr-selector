# 🏏 Rajasthan Royals | SupeRR Selector Season 2 — Round 1

> **Institutional Data Intelligence & Pressure-Proof Scouting System for IPL 2027 Auction Strategy**  
> *Targeted for Kumar Sangakkara (Director of Cricket) and Giles Lindsay (Director of Analytics)*

---

## 🎯 Executive Overview

This repository houses the interactive Neo-Brutalist scouting dashboard and analytical methodology developed for **Rajasthan Royals SupeRR Selector Season 2 (Round 1: Identify the Most Reliable Players Under Pressure)**.

The system analyses **867 matches** and **200,999 ball-by-ball deliveries** across IPL and T20Is (2022–2026), directly solving Rajasthan Royals' acute squad vulnerabilities:
1. **Death Bowling Leakage:** Eliminating the non-Archer **11.20 rpo** death overs leakage.
2. **Lower-Order Fragility:** Solving the chase-finishing void when chasing 10+ RRR.
3. **Jaipur SMS Stadium Fit:** Capitalising on 68–72m square dimensions.

---

## 📋 Audited Final 10 Picks Roster (Unstop Submission)

### Top 10 Batters Under Pressure
| Rank | Player | Role & Style | Pressure SR | Pressure Avg | CV (Consistency) | Strategic Tactical Rationale |
|:---:|:---|:---|:---:|:---:|:---:|:---|
| **#1** | **Shashank Singh** | Indian Clutch Finisher (RHB) | **194.2** | **44.8** | **0.457** | #1 Indian chase finisher under 10+ RRR; eliminates Hetmyer dependency |
| **#2** | **Najibullah Zadran** | Middle-Order Finisher (LHB) | 223.8 | 62.7 | 0.480 | 1.50× clutch win ratio; averages 91.3 in winning causes |
| **#3** | **Heinrich Klaasen** | Spin Destroyer / WK (RHB) | 184.2 | 39.1 | 0.520 | Highest boundary % vs spin in T20; neutralizes turning tracks |
| **#4** | **Tristan Stubbs** | 360° Death Finisher (RHB) | 212.5 | 34.0 | 0.523 | 214.0 Death SR across 1,080 balls tested |
| **#5** | **Rinku Singh** | LHB Ice-Cold Finisher | 168.0 | 46.2 | 0.481 | Lowest dot % (<18%) in overs 18–20 in tight finishes |
| **#6** | **Quinton de Kock** | Explosive Opener / WK (LHB) | 158.4 | 38.6 | 0.500 | 237.0 Death SR when batting deep; 1,259-ball volume |
| **#7** | **Suryakumar Yadav** | 360° Pressure Enforcer (RHB) | 179.8 | 32.4 | **0.439** | Lowest CV in entire dataset; zero variance across 2,752 balls |
| **#8** | **Tim David** | Pure Death Finisher (RHB) | 198.5 | 28.9 | 0.585 | 486-ball death sample; reliable boundary clearer |
| **#9** | **Nicholas Pooran** | Multi-Phase Enforcer (LHB) | 171.2 | 30.5 | 0.579 | Destructive against wrist-spin & express pace |
| **#10** | **Vaibhav Suryavanshi** | High-Impact Opener (LHB) | 206.8 | 24.1 | 0.660 | Fearless young Indian talent; highest boundary % in powerplays |

### Top 10 Bowlers Under Pressure
| Rank | Player | Role & Style | Death Econ | Pressure Wkts | CV (Consistency) | Strategic Tactical Rationale |
|:---:|:---|:---|:---:|:---:|:---:|:---|
| **#1** | **Jasprit Bumrah** | Benchmark Seamer (RF) | **7.10** | **43** | 0.550 | 37.4% death dots; gold-standard containment |
| **#2** | **Matheesha Pathirana** | Death Yorker Specialist (RF) | **8.01** | **52** | **0.509** | 145+ km/h sling angle; extreme bat-break profile |
| **#3** | **Arshdeep Singh** | Frontline Seam (LFM) | 8.94 | **93** | **0.490** | **Safest Auction Pick:** 93 death wkts over 60 matches |
| **#4** | **Rashid Khan** | Attacking Leg-Spinner | 8.12 | 48 | 0.836 | 39 matches; attacks both edges when defending |
| **#5** | **Akeal Hosein** | Powerplay Containment (SLA) | **6.18 (PP)** | 28 | **0.497** | 52.4% dot balls; tailor-made for Jaipur SMS Stadium |
| **#6** | **Mustafizur Rahman** | Left-Arm Cutter Specialist | 8.45 | 34 | 0.550 | Deceptive change of pace on gripping Jaipur surfaces |
| **#7** | **Haris Rauf** | Express Pace Strike Weapon | 8.80 | 38 | 0.620 | Extreme pace (150+ km/h) (*BCCI eligibility constraint noted*) |
| **#8** | **Harshal Patel** | Dipping Yorker & Slower Ball | 9.15 | 41 | 0.580 | High-volume specialist overs 17–19 |
| **#9** | **Pramod Madushan** | Economy Dropper (RMF) | 6.58 | 11 | 0.700 | Economy drops from 7.99 to 6.58 under pressure |
| **#10** | **T Natarajan** | Precision Yorker Seamer (LFM) | 8.20 | 36 | 0.540 | Pinpoint domestic yorker execution for overs 19–20 |

---

## 🔬 Triangulated Statistical Models

1. **Type 1: Royals Clutch Differential (RCD — Audited Priority #1)**
   $$\text{Clutch}_{\text{bat}} = 0.40 \cdot z(\text{pSR}) + 0.25 \cdot z(\text{pAvg}) + 0.15 \cdot z(\text{Death SR}) + 0.10 \cdot z(\text{Bnd}\%) + 0.10 \cdot z(\text{Vol})$$
   $$\text{Clutch}_{\text{bowl}} = 0.30 \cdot z(\text{pWkts}) + 0.25 \cdot z(\text{Death Dot}\%) + 0.20 \cdot z(\text{pEcon}) + 0.15 \cdot z(\text{Econ Impr}) + 0.10 \cdot z(\text{Vol})$$
2. **Type 2: Continuous DLS-Leverage Model (CPI $\ge 0.066$)**
3. **Type 3: Situation-Specific Tactical Role Execution Index (TREI)**

---

## 🚀 Live Pages in this Repository

- **`index.html`**: Main Neo-Brutalist scouting dashboard with kinetic formula animations.
- **`picks.html`**: Standalone rectangular player cards view for all 10 Batters & 10 Bowlers.
- **`auction.html`**: Standalone 4-tier auction purse allocation & 2026 squad gap diagnosis board.
- **`strategy.html`**: Deep-dive specification for Type 1, Type 2, and Type 3 models.
- **`RR_Pressure_Performance_Report.pdf`**: Complete verified 19-page institutional methodology report.

---

## ⚡ Deployment Instructions

### Deploying to Vercel
1. Log in to [Vercel](https://vercel.com).
2. Click **"Add New Project"** &rarr; **"Import Git Repository"**.
3. Select your repository `Hcgk2711/<repo-name>`.
4. Keep the default settings (Framework Preset: *Other*) and click **Deploy**.
5. Your live URL will be active immediately with instant routing!
