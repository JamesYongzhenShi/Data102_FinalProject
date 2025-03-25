# Data102 Final Project: Transportation Statistics and Safety Analysis

**Authors:** James Shi, Peng Zheng, Joe Zhou, Chloe Liu  
**Course:** Data 102 (Fall 2022)  
**Repository:** [Data102_FinalProject](https://github.com/JamesYongzhenShi/Data102_FinalProject)

---

## Project Overview

This project analyzes transportation data sourced from the U.S. Bureau of Transportation Statistics and additional data from FRED and FAA. The primary goals are to:

- **Predict Passenger Rail Total Train Miles** using both non-parametric methods (Decision Tree & Random Forest) and Generalized Linear Models (GLM).
- **Conduct causal inference** to assess the impact of state and local government construction spending on aviation fatality rates.
- **Perform data ingestion, cleaning, and wrangling** on a multi-source dataset with varying granularities.
- **Evaluate model performance** using cross-validation, bootstrap estimation, and R² metrics.
  
---

## Key Components

### 1. Process & Tools

- **Data Ingestion:** Importing and merging datasets from multiple sources (census data, FRED, FAA).
- **Data Wrangling:** Cleaning missing values, feature engineering (e.g., logarithmic scaling, lagged features, and categorical variables such as pre/post COVID).
- **Exploratory Data Analysis (EDA):** Visualizations and correlations to select features.
- **Modeling:**
  - **Non-Parametric Methods:** Decision Tree and Random Forest regressors.
  - **GLM Approaches:** Both frequentist (via statsmodels) and Bayesian (via PyMC3) regression to predict rail miles.
- **Causal Inference:** Inverse Probability Weighting (IPW) and outcome regression to explore the relationship between government spending and aviation fatality rates.

### 2. Project Structure

- `data102_final_project.py`: Main Python script with the full workflow (data ingestion, cleaning, EDA, modeling, and causal inference).
- Additional notebooks and reports:
  - `GLM and NP.ipynb`: Notebook (for interactive analysis).
  - `Final_Report_Data102.pdf`: Detailed project report and discussion.

### 3. Setup & Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/JamesYongzhenShi/Data102_FinalProject.git
   cd Data102_FinalProject
