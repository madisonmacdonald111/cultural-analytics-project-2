# Mini Project 2: Marvel Universe Social Network
**INFO 230 | Spring 2026**

---

## Overview

Can the structure of a comic book universe reveal sixty years of editorial decisions? This project applies a full network analysis pipeline to the [Marvel Universe Social Network](https://www.kaggle.com/datasets/csanhueza/the-marvel-universe-social-network) from Kaggle (a dataset of 6,439 heroes and 96,104 co-appearances across 12,651 comic issues).

For the full analysis, results, discussion, and interpretations see **`code/project-workflow.ipynb`**.

---

## Dataset

**Source:** [Marvel Universe Social Network](https://www.kaggle.com/datasets/csanhueza/the-marvel-universe-social-network) — Kaggle

| File | Description |
|---|---|
| `nodes.csv` | All 19,090 nodes with type label (hero or comic) |
| `edges.csv` | Raw two-sided network — one row per hero-comic appearance |
| `hero-network.csv` | Pre-projected hero-to-hero co-appearance network |

---

## Repo Structure
```
cultural-analytics-project-2/
├── code/
│   └── project-workflow.ipynb      <- full analysis lives here
|   ├── project-workflow.html
├── data/
│   ├── nodes.csv
│   ├── edges.csv
│   └── hero-network.csv
├── figures/
│   ├── interactive_community_0.html
│   ├── interactive_community_1.html
│   ├── interactive_community_8.html
│   └── interactive_community_13.html
├── network_output/
│   └── marvel_Avengers
|   ├── marvel_Defenders_and_Mystic_Heroes.graphml
|   ├── marvel_Fantastic_Four.graphml
|   ├── marvel_network.graphml
|   ├── marvel_Spider-Mans_World.graphml
|   ├── marvel_Thor_and_Cosmic_Heroes.graphml
|   ├── marvel_X-men.graphml
├── index.html
└── README.md
```

---

## How to Run

1. Clone the repo
2. Install dependencies (see below)
3. Run `code/project-workflow.ipynb` top to bottom

All random operations use `SEED = 230` so results are fully reproducible.

---

## Dependencies
```
pandas
numpy
networkx
plotly
pyvis
```
```bash
pip install networkx pyvis plotly
```

---

## Course Context

Mini Project 2 — INFO 230: Cultural Analytics, Spring 2026  
Network analysis patterns draw on the course Holmes co-occurrence notebook (`holmes_cooccurrence_networks.ipynb`).

By Maddie MacDonald | UC Berkeley Statistics, MA