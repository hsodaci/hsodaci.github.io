---
title: "EuroVolley 2023 vs 2026"
permalink: /projects/eurovolley-2023-2026/
layout: page
excerpt: A data pipeline for comparing Türkiye's 2023 and 2026 CEV Women's EuroVolley championship runs.
comments: false
---

<p class="pub-meta">Filenin Sultanları &middot; 2026</p>

<div class="pub-tags">
  <span class="pub-tag">Python</span>
  <span class="pub-tag">Web Scraping</span>
  <span class="pub-tag">Pandas</span>
  <span class="pub-tag">Sports Analytics</span>
</div>

Türkiye won the CEV Women's EuroVolley Championship in both 2023 and 2026. This project builds a clean player- and team-level dataset to compare the two championship runs and study how Türkiye's statistical profile changed across three years.

<div class="pub-actions">
  <a class="pub-btn pub-doi" href="#">GitHub Repository</a>
</div>

<!-- TODO: the GitHub link above is a placeholder — swap in the real repo URL. -->

#### Situation

Türkiye won the CEV Women's EuroVolley Championship in both 2023 and 2026, but no clean, comparable dataset existed to study how the team's statistical profile changed between the two title runs.

#### Task

Build a player- and team-level dataset from CEV's official public match-report system that makes the 2023 and 2026 championships directly comparable, covering serving, reception, attacking, blocking, scoring, and set participation.

#### Action

Collected official match statistics directly from CEV's public match-report system across:

- 2 tournaments
- 152 matches
- 18 Türkiye matches
- player-level and team-level statistics

Built a two-notebook pipeline:

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

```text
01_scrape_eurovolley_data.ipynb
02_clean_eurovolley_data.ipynb
```

The cleaning step handled several issues in the original CEV data: separating team totals from player rows, correctly converting placeholder values, distinguishing missing percentages from true 0%, separating set participation from rotation position, standardizing player and team names, converting names to ASCII, and validating results against known matches.

#### Result

Two analysis-ready datasets:

```text
eurovolley_2023_2026_players_clean.csv
eurovolley_2023_2026_team_totals_clean.csv
```

Data collection and cleaning are complete; analysis is in progress. The next phase compares Türkiye's two title runs across attack efficiency, serve pressure, reception quality, blocking, error control, and player contribution — to identify which characteristics of Türkiye's championship performance were stable, changed over time, or depended on specific players.

<p class="pub-meta">Data collection: complete &middot; Data cleaning: complete &middot; Analysis: in progress</p>
