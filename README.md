# March Madness Prediction Project

This project utilizes machine learning and historical sports data to predict the outcomes of the NCAA Men's Basketball Tournament. The repository contains a progression from baseline statistical analysis to advanced gradient-boosted modeling.

## 📓 Notebooks

### 1. [march_madness_bracket.ipynb](./march_madness_bracket.ipynb)
**Focus: Exploration & Baselines** This notebook serves as the project foundation, focusing on data inspection and establishing a performance floor.
* **Data Exploration:** Analyzes historical win rates by seed and evaluates the "Chalk" method (always picking the higher seed).
* **Baseline Performance:** Establishes a baseline accuracy of **~72%** for tournament predictions.
* **Betting Metrics:** Implements logic for calculating expected ROI and betting outcomes based on seed-based historical performance.

### 2. [bracket_ml.ipynb](./bracket_ml.ipynb)
**Focus: Machine Learning Pipeline** This is the core modeling notebook where the predictive engine is developed, tuned, and validated.
* **Advanced Preprocessing:** Normalizes regular-season performance and calculates **Score POE (Points Over Expectation)** to adjust for opponent strength.
* **Feature Engineering:** Develops key predictors including **Net Rating** (efficiency per 100 possessions) and **Conference Pedigree** (historical tournament success of a team's conference).
* **XGBoost Implementation:** Utilizes an XGBoost classifier with custom feature weights and early stopping to optimize for **Log Loss**.
* **Validation & Results:** Achieved a **79% prediction accuracy**, significantly outperforming the project's baseline.

## 📈 Key Results
* **Baseline Accuracy:** 72%
* **ML Model Accuracy:** 79%
* **Primary Metrics:** Log Loss, Seed-Based ROI, and Points Over Expectation (POE).

## 🛠️ Requirements
* Python 3.x
* Pandas / NumPy
* XGBoost
* Matplotlib / Seaborn
