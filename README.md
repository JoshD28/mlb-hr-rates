# MLB Home Run Rates (Bayesian Hierarchical Model)

This repository contains a course lab estimating **MLB player home run rates (HR/AB)** for the **2025 season** using a **Bayesian hierarchical model**. The lab reports posterior summaries for top players, evaluates model fit via a **posterior predictive check (PPC)**, and includes a short reflection on **shrinkage**.

## Lab Goals
1. Estimate **home run rate (HR / AB)** for each player in the 2025 MLB season using a **Bayesian hierarchical model**.
2. Report **posterior means + 95% credible intervals** for the **top 20 players**.
3. Produce a **Posterior Predictive Check (PPC)** figure.
4. Provide a ~150-word reflection on **shrinkage** in hierarchical modeling.

## Data
- **Season:** MLB 2025
- **Unit of analysis:** Player-season
- **Key columns:** at-bats (AB), home runs (HR) (and any identifiers used)

If the dataset is included, it lives at `data/batting_stats_2025.csv`.
If not included, see `data/README.md` for how to add it locally.

## Methods
- **Model:** Bayesian hierarchical model for binomial outcomes (HR successes out of AB trials)
- **Outputs:** posterior means, 95% credible intervals, ranking of players by posterior mean rate
- **Model checking:** Posterior Predictive Check (PPC)

## Outputs
- Table of **top 20** HR rate estimates with **95% credible intervals**
- **PPC plot** comparing observed vs simulated outcomes
- Brief written reflection on **shrinkage**

## How to Run
1. Clone/download this repository.
2. Ensure the dataset is available at `data/batting_stats_2025.csv`.
3. Open and run:
   - `notebooks/Lab_5_MLB_HR_Rates.ipynb`

## Requirements
- Python 3.x
- pandas, numpy, matplotlib
- (optional) pybaseball (if used for data retrieval)
