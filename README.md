# WPL Performance Analytics Dashboard (2023–2026)

**Project Documentation | Power BI Desktop 2.159.883.0**

## Project Overview
This project analyses Women’s Premier League (WPL) match data across the 2023, 2024, 2025 and 2026 seasons. The three-page interactive Power BI dashboard covers competition overview, individual player performance and team performance.

Python was used for data preparation; Power BI was used for data modelling, DAX calculations and visual analytics.

## Business Objectives
- Summarise WPL activity across four seasons.
- Compare team batting output, bowling performance and match wins.
- Identify leading batters and bowlers using player-level statistics.
- Explore team, season and player performance through dashboard visuals.

## Dataset and Scope
- **Source:** Cricsheet ball-by-ball cricket data.
- **Coverage:** 88 matches across four seasons (22 matches per season), 2023–2026.
- **Teams:** MI, DC, RCB, GG and UPW.
- Cricsheet YAML files were converted into tabular CSV datasets for analysis.

## Tools and Technologies
- Python and Pandas — data preparation and transformation.
- Power BI Desktop **2.159.883.0** — data modelling and dashboard development.
- DAX — measures and dynamic KPI calculations.
- Cricsheet — match data source.

## Data Preparation
- Converted Cricsheet YAML match files into structured tables.
- Organised match-level and delivery-level data.
- Standardised team names, including consolidating Royal Challengers Bangalore under Royal Challengers Bengaluru (RCB).
- Prepared team, season and player summary datasets.
- Cross-checked aggregate statistics and dashboard values.

## Main Tables
| Table | Purpose |
|---|---|
| `matches_cleaned` | Match-level details, season and winner |
| `team_performance` | Overall team runs, wickets, runs conceded, runs per innings and economy |
| `season_batting` | Season-wise team batting summaries |
| `season_team_bowling` | Season-wise team bowling summaries |
| `batting_summary` | Player-level batting statistics |
| `bowling_summary` | Player-level bowling statistics |
| `best_batter_each_season` | Seasonal leading batter summary |
| `best_bowler_each_season` | Seasonal leading bowler summary |
| `DimSeason` | Season dimension |
| `BattingPlayerImages`, `BowlingPlayerImages` | Player selection and image lookup |

## Dashboard Pages
### 1. WPL Overview
Competition KPIs, season selection, leading batter and bowler highlights, team runs, team wins and bowling economy insights.

### 2. Player Performance
Batter and bowler selection, dynamic player images, batting KPIs (runs, average, strike rate, fours and sixes), bowling KPIs (wickets, economy, average and overs), and top-five player charts.

### 3. Team Performance
Overall team KPIs and comparisons, team batting and bowling comparison, bowling economy, bowling average, season-wise team runs, season-wise bowling economy and season-wise wins.

## Key Data Highlights
- **Matches:** 88
- **Seasons:** 4 (2023–2026)
- **Teams:** 5
- **Overall team runs in prepared team summary:** 27,378
- **Bowler-credited wickets in prepared team summary:** 1,000
- **Team wins:** 87; one tied match had no winner
- **Leading batter:** Nat Sciver-Brunt — 1,348 runs
- **Leading bowler:** Amelia Kerr — 54 wickets

## Validation Notes
- KPI values and chart totals were cross-checked against the prepared datasets.
- Bowler-credited wickets (1,000) are distinct from all recorded dismissals (1,079).
- The season slicer is intentionally used on the Overview page. Player and Team pages retain page-specific interactions rather than forcing one global slicer across all visuals.

## Conclusion
This project demonstrates data preparation, analytical modelling, DAX and Power BI visualisation through a multi-season WPL performance dashboard.

## Suggested Repository Structure
```text
WPL-Performance-Analytics/
├── data/
├── notebooks/
├── dashboard/
├── screenshots/
└── README.md
```

*Note: Include only datasets and files that you are permitted to redistribute. Add your own dashboard screenshots and notebook links before publishing the repository.*
