# VALORANT-Champions-Tour-2025-Match-Outcome-Analysis-Modeling

Exploratory analysis and predictive modeling of professional VALORANT match data to evaluate how team performance metrics relate to competitive match outcomes.

---

## Overview

This project analyzes professional matches from the 2025 VALORANT Champions Tour (VCT) season to assess whether commonly used team-level performance metrics provide reliable predictive signal for match outcomes.

Rather than assuming that strong historical performance directly translates to future success, the analysis evaluates how predictive patterns behave across tournaments by training models on earlier events and testing on later competitions. This approach mirrors real-world forecasting conditions where predictions must be made sequentially over time.

---

## Data Source

**Dataset:** Kaggle – VALORANT Champions Tour Match Data (2025)

The dataset contains match-level and player-level statistics from official VCT tournaments. For this analysis, player-level statistics were aggregated to the team-match level to align with the prediction target (win/loss outcome).

Only major international events were included to maintain competitive consistency.

---

## What Was Done

- Cleaned and prepared raw match and player performance data  
- Aggregated player statistics into team-level performance features  
- Conducted exploratory data analysis and correlation screening for feature selection  
- Engineered input features based on match performance metrics  
- Trained multiple logistic regression models for match outcome prediction  
- Applied temporal train-test splits to preserve chronological order and prevent data leakage  

---

## Modeling Approach

Logistic regression was selected as a baseline classification model to balance interpretability and predictive performance.

Models were trained on earlier tournament data and evaluated on later events to measure generalization across competitions. This temporal validation strategy reflects realistic deployment conditions where future match outcomes are unknown at training time.

---

## Key Outputs

- Feature correlation visualizations and exploratory performance plots  
- Model evaluation metrics for tournament-based train-test splits  
- Comparative performance results across validation windows  

---

## Limitations

- Only observable in-game performance statistics were used  
- External factors such as team composition changes, patch updates, and strategy shifts were not explicitly modeled  
- Results reflect statistical associations rather than causal relationships  

---

## Tools Used

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Scikit-learn  
- Jupyter Notebook  

---

## Author

**Nathanael Theodore M. Fenomeno**  
BS Data Science and Business Administration — Asian Institute of Management

