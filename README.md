# Football Data Project

This repository contains the analytical assets for the Champ Engineering Data Track football intelligence project.

## Project Overview

- **Scope:** Develop data-driven tooling that supports player valuation and segmentation for professional football clubs.
- **Deliverables:** Two production-ready analytics pipelines accompanied by curated datasets and exploratory notebooks.
- **Users:** Sporting directors, scouting departments, and analytics teams operating under constrained transfer budgets.

## Business Problem

- Football clubs with limited budgets must consistently buy undervalued players and sell at peak value while ensuring squad fit.
- Manual scouting alone struggles to surface comparable player profiles across leagues and competition levels.

## Objectives

### Main

- Predict each player's market value trajectory using historical performance and contextual features.
- Group players into performance-based archetypes to streamline recruitment shortlists.

### Optional

- Establish a foundation for future match-outcome prediction models that combine player, team, and external signals.

## Solution Design

- **Market Value Pipeline:** Time-series regression powered by LSTM/Transformer/NN architectures over player statistics, demographic features, and competition metadata.
- **Player Clustering Pipeline:** Unsupervised learning on per-90 action metrics and physique attributes to derive role-specific clusters.
- **Future Enhancement:** Integrate player and team embeddings with external feeds to forecast match outcomes.

## Data Sources

- [fbref](https://fbref.com/en) — time-series player statistics (limited coverage for under-the-radar players).
- [Transfermarkt](https://www.transfermarkt.com/) — community-maintained market value benchmarks used as labels.
- [Understat](https://understat.com/) — match-level performance aggregates for contextual features.
- [Kaggle: player-scores](https://www.kaggle.com/datasets/davidcariboo/player-scores/data) — curated Transfermarkt export used for cross-validation.

## Stakeholder Perspectives

- **Ta:** High-stakes transfer markets demand quantitative decision support to capture value at scale.
- **Tanny:** Rich, multi-source data enables experimentation with a diverse set of analytical techniques.
- **Touch:** Opportunity to explore an emerging application domain with tangible on-field impact.
- **Nac:** Niche yet expansive problem space with numerous data-driven applications (and a passion for the sport).

## Dataset Inventory

- **fbref** (Google Drive [folder](https://drive.google.com/drive/folders/1VRIjqljWRwSherisYYVwU8fr-V9qIK3t))
  - Player statistics: `Keeper`, `Outfield`
  - Team statistics
- **kaggle** (download via Kaggle Hub)
  - Transfermarkt tables (Games, Players, Clubs, Appearances, etc.): [dataset](https://www.kaggle.com/datasets/davidcariboo/player-scores/data)
