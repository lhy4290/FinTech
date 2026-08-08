# FinTech — South Asian Digital Wallet Ecosystem LTV Data Mining

Customer Lifetime Value (LTV) data mining research on South Asian digital wallet users. Clustering models identify user segments by value and risk profile, distinguishing high-value customers from high-fraud-risk ones. Findings are compiled into a formal research paper and demonstrated through an interactive web-based decision engine simulator — the **Intelligent Behavioral Incentive & Anti-Fraud Decision Engine**.

## Overview

Digital wallets across South Asia generate large volumes of behavioral and transactional data, but turning that data into actionable customer strategy — who to invest retention budget in, and who represents fraud risk — is non-trivial. This project applies clustering-based data mining to a digital wallet user dataset to:

- Segment users by lifetime value and behavioral patterns
- Surface features that distinguish high-value users from high-risk/fraudulent ones
- Translate the analysis into a simulator that visualizes how incentive and anti-fraud decisions would play out across segments

Full findings are written up in the accompanying paper *南亞數位金融生態圈生命週期價值資料探勘研究分析* (South Asian Digital Financial Ecosystem LTV Data Mining Research Analysis).

## Contents

| File | Description |
|---|---|
| `digital_wallet_ltv_dataset.csv` | Digital wallet user behavior and transaction dataset |
| `Data.ipynb` | Clustering analysis notebook — segments users and extracts value/risk features |
| `final_cluster_results.csv` | Output of the clustering analysis (per-user segment assignments) |
| `index.html` | Interactive decision engine simulator (dark tech-themed UI) |

## Decision Engine Simulator

`index.html` turns the clustering research into an interactive front-end: a dark, tech-styled interface (Noto Sans TC + JetBrains Mono) that lets users explore how behavioral incentive and anti-fraud rules would apply across the identified customer segments — making the research results explorable rather than static.

To run it locally, just open `index.html` in a browser (no build step required).

## Methodology

1. **Data preparation** — clean and structure the digital wallet dataset (`Data.ipynb`).
2. **Clustering** — group users based on behavioral and transactional features to reveal natural segments.
3. **Segment interpretation** — characterize each cluster along value (LTV) and risk (fraud likelihood) dimensions.
4. **Simulation** — expose the segment logic through an interactive web simulator for non-technical exploration.

## Tech Stack

Python, Pandas, Clustering algorithms, Jupyter Notebook, HTML/CSS (vanilla front-end simulator)

## Research Paper

Full analysis and findings: *南亞數位金融生態圈生命週期價值資料探勘研究分析* (PDF)
