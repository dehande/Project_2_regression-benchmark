# Project 2 — Complex Regression Model (Benchmark)

This project benchmarks multiple regression approaches on a single dataset:
- Linear Regression (baseline)
- Polynomial Regression (degree=5)
- Ridge Regression (degree=5, alpha=0.5)
- Lasso Regression (degree=5, alpha=10)

Evaluation:
- Train MAE
- Test MAE
- Generalization gap (test_mae - train_mae)
- Lasso sparsity (number of zero coefficients)

## How to run
Option A — Run in Google Colab:
1) Open the notebook in Colab:
   https://colab.research.google.com/github/dehande/Project_2_regression-benchmark/blob/main/Proje2_Complex_Regression_Model.ipynb
2) No dataset upload is required — the notebook auto-generates `regression_playground.csv` if it is missing.
   (Optionally, you can upload your own `regression_playground.csv` with `age` and `salary` columns to override.)
3) Runtime > Run all

Option B — Run locally:
- Requires Python + common ML stack (pandas, numpy, scikit-learn)

## Key result (summary)

In this dataset, the baseline linear model (degree=1) achieved the lowest test MAE.
Lasso reduced model complexity by zeroing out some polynomial terms.

## Files
- `Proje2_Complex_Regression_Model.ipynb` — main notebook

Update: The notebook is now fully runnable out-of-the-box on Colab (no external data required).
