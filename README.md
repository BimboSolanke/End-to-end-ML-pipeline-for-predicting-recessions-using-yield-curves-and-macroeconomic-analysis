# Recession Prediction Analysis

## Project Overview
This project develops machine learning models to predict U.S. recessions using yield curve inversions, credit spreads, and macroeconomic indicators. 
The analysis addresses key feedback from initial submission and implements comprehensive statistical testing and robustness checks.

## Data
- Treasury yields from Federal Reserve H.15 dataset
- Economic indicators from FRED (Federal Reserve Economic Data)
- All data included locally - no API access required

## Requirements
- Python 3.8+
- Dependencies listed in requirements.txt

## Installation & Usage
```bash
# Clone repository
(https://github.com/BimboSolanke/End-to-end-ML-pipeline-for-predicting-recessions-using-yield-curves-and-macroeconomic-analysis)
cd _recession-prediction-analysis

# Install dependencies
pip install -r requirements.txt

# Run analysis
_recession_prediction_analysis_python_notebook_finalVer
(for full automation, code is written to access required data listed above straight from the web, however the local copies of the data are attached here.)

## Key Features
- Statistical hypothesis testing with formal null/alternative formulations
- Multiple yield spread analysis (8 different maturity combinations)
- Random Forest and XGBoost models, Random Forest model achieving 0.817 AUC
- 12-month forward recession prediction
- Comprehensive robustness testing across economic regimes

## Feedback Implementation
This project incorporates substantial improvements based on prof. Omid's feedback:
1. **Statistical Rigor**: Reformulated hypotheses with testable null/alternative pairs
2. **Expanded Analysis**: Incorporated multiple yield spreads beyond 3M-10Y
3. **Hypothesis Linkage**: Connected descriptive findings directly to research hypotheses

See [docs/Feedback_Implementation.md](docs/Feedback_Implementation.md) for detailed responses.

## Repository Structure
├── data/                    # Raw and processed data files
├── notebooks/               # Jupyter notebooks for analysis (developed to run automatically while loading all relevant data from the web)
├── notebooks/               # .py notebook same as jupyter (backup) (developed to run automatically while loading all relevant data from the web)
├── src/                     # Python source code
├── results/                 # Model outputs and visualizations
├── docs/                    # Documentation
│   ├── Feedback_Implementation.md
│   ├── Statistical_Tests.md
│   └── Robustness_Analysis.md
└── requirements.txt         # Python dependencies
(All local copies of data accessed directly from the web are attached here as well)
**Results Summary**
Primary Finding: Yield curve inversions predict recessions with 71.4% accuracy within 18 months
Best Model: Random Forest (AUC 0.817) outperforms logistic regression (AUC 0.769)
Key Predictors: Unemployment dynamics (39.2%), Term spread (31.5%), Credit spread (23.6%)

**Academic Context**
Course: Data Analytics Case Study 3 (DAMO-611-6)
Institution: University of Niagara Falls, Canada
Instructor: Prof. Omid Isfahanialamdari
Term: Summer 2025

**Author**
Bimbo Olukoya Solanke
