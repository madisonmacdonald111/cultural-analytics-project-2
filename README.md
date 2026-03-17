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
│   ├── project-workflow.ipynb      <- full analysis lives here
│   ├── project-workflow.html
│   └── network_output/
│       ├── marvel_Avengers.graphml
│       ├── marvel_Defenders_and_Mystic_Heroes.graphml
│       ├── marvel_Fantastic_Four.graphml
│       ├── marvel_Spider-Mans_World.graphml
│       ├── marvel_Thor_and_Cosmic_Heroes.graphml
│       └── marvel_X-Men.graphml
├── data/
│   ├── nodes.csv
│   ├── edges.csv
│   └── hero-network.csv
├── figures/
│   ├── interactive_community_0.html
│   ├── interactive_community_1.html
│   ├── interactive_community_8.html
│   └── interactive_community_13.html
├── environment.yaml
├── index.html
└── README.md
```

---

## How to Run

1. Clone the repo
2. Create and activate the conda environment:
```bash
conda env create -f environment.yaml
conda activate cultural_analytics
```
3. Launch Jupyter and run `code/project-workflow.ipynb` top to bottom

All random operations use `SEED = 230` so results are fully reproducible.

---

## Environment

All dependencies are managed via `environment.yaml` using the `cultural_analytics` conda environment. Key packages include `networkx`, `pyvis`, and `plotly` for network analysis and visualization, alongside `pandas`, `numpy`, `matplotlib`, and `scikit-learn` for general data processing.

---

## References

**Dataset**
- Sanhueza, C. (2017). *The Marvel Universe Social Network*. Kaggle. https://www.kaggle.com/datasets/csanhueza/the-marvel-universe-social-network

**Network Analysis Methods**
- Blondel, V. D., Guillaume, J. L., Lambiotte, R., & Lefebvre, E. (2008). Fast unfolding of communities in large networks. *Journal of Statistical Mechanics: Theory and Experiment*, 2008(10), P10008.
- Newman, M. E. J. (2010). *Networks: An Introduction*. Oxford University Press.
- Barabási, A. L., & Albert, R. (1999). Emergence of scaling in random networks. *Science*, 286(5439), 509–512.

**Marvel Lore**
- DeFalco, T., Sanderson, P., Brevoort, T., Teitelbaum, M., Wallace, D., Darling, A., ... & Cowsill, A. (2019). *Marvel Encyclopedia*. DK Publishing.
- Gruenwald, M., Grant, S., & Layton, B. (1982). *Marvel Super Hero Contest of Champions* #1–3. Marvel Comics.

**Academic Network Analysis of Marvel**
- Alberich, R., Miro-Julia, J., & Rossello, F. (2002). Marvel Universe looks almost like a real social network. *arXiv preprint cond-mat/0202174*.

**Course Materials**
- Course Holmes co-occurrence notebook (`holmes_cooccurrence_networks.ipynb`), INFO 230: Cultural Analytics, Spring 2026.

By Maddie MacDonald | UC Berkeley Statistics, MA