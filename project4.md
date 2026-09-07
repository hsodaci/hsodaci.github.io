---
title: "EuroVolley 2023 vs 2026"
permalink: /projects/eurovolley-2023-2026/
layout: page
excerpt: A data pipeline for comparing Türkiye's 2023 and 2026 CEV Women's EuroVolley championship runs.
comments: false
---

**Filenin Sultanları** — Python · Web Scraping · Pandas · Sports Analytics

Türkiye won the CEV Women's EuroVolley Championship in both 2023 and 2026. This project builds a clean player- and team-level dataset to compare the two championship runs and study how Türkiye's statistical profile changed across three years.

#### Project

I collected official match statistics directly from CEV's public match-report system. The pipeline covers:

- 2 tournaments
- 152 matches
- 18 Türkiye matches
- player-level and team-level statistics

The data includes serving, reception, attacking, blocking, scoring, and set participation.

#### Pipeline

```text
CEV Match Reports
        ↓
Scrape match and player statistics
        ↓
Clean and validate the data
        ↓
Player-level dataset
Team-level dataset
        ↓
Statistical analysis
```

The project uses two notebooks:

```text
01_scrape_eurovolley_data.ipynb
02_clean_eurovolley_data.ipynb
```

#### Data cleaning

The cleaning process handles several issues in the original CEV data:

- separates team totals from player rows
- converts placeholder values correctly
- distinguishes missing percentages from true 0%
- separates set participation from rotation position
- standardizes player and team names
- converts names to ASCII
- validates results against known matches

#### Output

```text
eurovolley_2023_2026_players_clean.csv
eurovolley_2023_2026_team_totals_clean.csv
```

Both datasets are analysis-ready.

#### Next step

The next phase compares Türkiye's two title runs across:

- attack efficiency
- serve pressure
- reception quality
- blocking
- error control
- player contribution

The goal is to identify which characteristics of Türkiye's championship performance were stable, changed over time, or depended on specific players.

#### Status

- Data collection: **Complete**
- Data cleaning: **Complete**
- Analysis: **In progress**

**Links:** *(TODO — add the real GitHub repository URL; the one in the source draft was a placeholder)*
