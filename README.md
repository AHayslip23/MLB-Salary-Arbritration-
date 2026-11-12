# MLB Salary Arbitration

An analysis of MLB salary arbitration cases: 387 player cases with service time, the player's ask, the team's offer and contract outcomes. It uses EDA, k-means clustering and regression models.

## Repository Contents

| File | Description |
|---|---|
| `mlb salary arbirtration data.ipynb` | Full analysis: EDA, clustering and regression models (44 charts) |
| `mlb salary arbirtation data.csv` | Arbitration dataset (387 cases) |

## Commit History

### `a0be157`: Upload of the notebook and dataset (2022-05-18)
- **EDA:**
  - most arbitration-eligible players are 28–29 years old, right-handed and earn $0–2 million per year
  - the Mets have the most eligible players, and the NL West has the most by division
  - it's rare for teams to buy out arbitration
- **K-means clustering:** grouped players by age and service time, salary, and player ask vs. team offer. The clusters separate:
  - players asking for and offered $5 million or less
  - mid-tier cases, where teams offer $7.5–10 million to players with 4–5 years of service time
  - $20 million+ "superstar" outliers
- **Regression models:**
  - predicting salary after arbitration: **87.6%** fit, e.g. predicting $13.3M vs. an actual $13.4M (the notebook notes it needs more data)
  - another salary model: 54.8%
  - predicting age (35% and 8.3%) and service time (28.8%) was much less accurate

## Tools
Python, pandas, NumPy, scikit-learn, matplotlib, seaborn, Jupyter Notebook
