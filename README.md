# Marvel Rivals Infographic

#### Author: Marie Tolteca, MEDS Student at **Bren School of Environmental Science & Management**

#### Date: March 9, 2026

# Marvel Rivals: Gameplay Analysis

A personal data analysis project exploring my Marvel Rivals gameplay statistics across **Seasons 3–6**, covering both Quick Match and Competitive modes.

## Main Question

**Am I optimizing my Marvel Rivals gameplay?** \#### Sub questions:

```         
Which hero do I use the most and what type of role is it?
What is my kill to death ratio for each hero and role used?
Which role do I win the most with?
```
## Marvel Rival Infographic
<img width="1039" height="1558" alt="mr_info" src="https://github.com/user-attachments/assets/b6cbbc02-8668-4aaa-b852-61914b79a049" />


## Data

-   **Source:** [Marvel Rivals Tracker API](https://rivalsmeta.com/) (`marvelrivalsapi.com`)
-   **Player Username:** `kpil11`
-   **Seasons:** 3–6 (Quick Match + Competitive)
-   **Fields:** hero, role, kills, deaths, assists, win/loss, damage, healing, match duration

## Repository

```         
├── data
│   ├── all_season_combined.csv
│   ├── clean_season.csv
│   ├── hero_kd_summary.csv
│   ├── hero_polar.csv
│   ├── role_kd_summary.csv
│   └── role_stats.csv
├── draft_2_files
├── draft_2.html
├── draft_2.qmd
├── drafting_viz_files
├── drafting_viz.html
├── drafting_viz.qmd
├── exploration_files
├── exploration.html
├── exploration.qmd
├── fonts
│   ├── Font Awesome 7 Brands-Regular-400.otf
│   ├── Font Awesome 7 Free-Regular-400.otf
│   └── Font Awesome 7 Free-Solid-900.otf
├── images
│   ├── Affinity_plots
│   │   ├── info.pdf
│   │   ├── info.png
│   │   ├── K:D Comparison_Heroes.pdf
│   │   ├── K:D Comparison_Heroes.png
│   │   ├── MarvelRivals_BG.png
│   │   ├── NEW_WIN_RAT.pdf
│   │   ├── NEW_WIN_RATE.png
│   │   └── old
│   │       ├── win_rate_role.png
│   │       └── win_rate.pdf
│   │   └── predators.jpg
│   ├── hero_duration.pdf
│   ├── hero_duration.png
│   ├── heroes
│   │   ├── angela.tif
│   │   ├── buckee.tif
│   │   ├── captainamerica.tif
│   │   ├── deadpool.tif
│   │   ├── gambit.tif
│   │   ├── ironman.tif
│   │   ├── jefftheshark.tif
│   │   ├── moonknight.tif
│   │   ├── phoenix.tif
│   │   ├── punisher.tif
│   │   ├── squirrelgirl.tif
│   │   ├── starlord.tif
│   │   └── venom.tif
│   ├── kd_plot.pdf
│   ├── kd_plot.png
│   ├── win_rate.pdf
│   └── win_rate.png
├── initial_analysis_files
├── initial_analysis.html
├── initial_analysis.qmd
├── output
│   ├── all_season_df.csv
│   ├── s3_s6_competitive.csv
│   ├── s4_competitive_matches.csv
│   ├── s4_quick_matches.csv
│   ├── s5_competitive_matches.csv
│   ├── s5_quick_matches.csv
│   ├── s6_competitive_matches.csv
│   ├── s6_quick_matches.csv
│   └── season_5_stats.csv
├── README.md
└── Tolteca-eds240-infographic.Rproj
```

## Visualizations

### 1. Hero Playtime

Scatter-style chart showing hours played per hero. Portrait fill indicates proportion of max playtime. **Moon Knight** and **Phoenix** are the most-played heroes.

### 2. Kill vs Death Comparison

Donut charts comparing kill/death percentages per hero, grouped by role (Duelist, Strategist, Vanguard). Most Duelists have kill rates between 64–73%.

### 3. Win Rate by Role

Bubble chart showing win rate per role. Bubble size = games played. Strategists have the highest win rate; Vanguards have the lowest.

## Key Findings

-   Kill-to-death ratios are generally positive, especially among Duelists.
-   Win rates differ by role — damage output alone doesn't drive wins.
-   Switching roles strategically based on team composition may improve outcomes.

## Libraries

`tidyverse`, `ggplot2`, `ggimage`, `ggtext`, `patchwork`, `magick`, `showtext`, `glue`, `forcats`, `httr`, `jsonlite`

## Game Modes Available

These are the type of games modes offered by Marvel Rivals, however I am comparing all the modes.
```
| Mode | Type |
|------|------|
| Convoy | Payload escort |
| Domination | King of the Hill |
| Convergence | Hybrid (capture + escort) |
```

