# IDS 472 — Data Mining & Predictive Analytics Coursework

Homework assignments and a team final project covering the supervised-learning workflow end to end: exploratory analysis, preprocessing, model training and comparison, cross-validation, and translating results into business recommendations. Built primarily with **scikit-learn**, plus **XGBoost** for the final project.

*Team: Artem Larin, Ihor Stepura, Krima Mehta, Arturo Perez.*

## Repository contents

| Notebook | Topic |
|---|---|
| `hw0_v4.ipynb` | Python/Pandas/NumPy/Matplotlib fundamentals warm-up |
| `hw1_v6.ipynb` | Introductory supervised learning with scikit-learn (train/test splits, first classifiers) |
| `hw2_v6.ipynb` | k-Nearest Neighbors — choosing K, comparing accuracy across K values, visual EDA with Seaborn |
| `IDS_472_HM3_D3.ipynb` | Regression analysis — probing (non)linearity of relationships, model fitting and diagnostics |
| `hw4_resubmission1.ipynb` | Naive Bayes on the `accidentsFull.csv` dataset (42,183 US automobile accidents, 2001) — naive rule baselines, conditional probabilities, injury prediction |
| `IDS_472_HM5_D2.ipynb` | Tree ensembles — CART vs. AdaBoost with 5-fold cross-validation, model selection by R² |
| `hw6_D3.ipynb` | Model complexity vs. class imbalance — why simpler models still struggle on imbalanced data |
| `IDS_472_Final_Project_D4.ipynb` | Full end-to-end final project (EDA → features → models → business insights) |

## Final project design (`IDS_472_Final_Project_D4.ipynb`)

The capstone follows a four-part structure mirroring a real analytics engagement:

1. **Exploratory Data Analysis & Preprocessing** — distribution analysis, missing-value handling, encoding of categorical variables, scaling; visual EDA with Matplotlib/Seaborn.
2. **Feature Engineering & Selection** — constructing informative features and pruning uninformative ones to reduce noise and leakage risk.
3. **Model Building & Evaluation** — multiple classifiers trained and compared (scikit-learn models plus **XGBoost**), evaluated on held-out data with accuracy, precision, recall, and F1 to expose trade-offs rather than relying on a single metric.
4. **Business Insights & Recommendations** — the models are interpreted in decision-making terms: which customers/records to act on, what drives predictions, and where each model's limitations matter in deployment.

## Themes across the coursework

- **Baselines first** — hw4 starts from the naive rule (predict the majority class) before Bayes methods, quantifying what a model must beat.
- **Validation discipline** — hold-out splits early on, then k-fold cross-validation (hw5) once model comparison becomes the point.
- **Interpretation over output** — notebooks include written reasoning for each result (e.g., why KNN accuracy plateaus across K, why class imbalance defeats complexity reduction in hw6), not just code cells.
- **Team workflow** — assignments are collaborative deliverables with clearly attributed question-by-question structure.

## Tech stack

Python, `pandas`, `numpy`, `scikit-learn` (KNN, decision trees, Naive Bayes, MLP, AdaBoost, CART), `xgboost`, `matplotlib`, `seaborn`.

## Running

```bash
pip install pandas numpy scikit-learn xgboost matplotlib seaborn
```
Each notebook is self-contained; place the referenced CSV datasets (e.g., `accidentsFull.csv`, the final-project dataset) alongside the notebook and run top to bottom.
