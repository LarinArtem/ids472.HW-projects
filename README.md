Data Mining hw and final project (IDS 472)

This repository contains coursework and a comprehensive final project from a Predictive Analytics and Supervised Learning course, with a strong emphasis on end-to-end model development, evaluation, and interpretation. The central focus of the project is a customer churn prediction problem using the Telco Customer Churn dataset, a widely used benchmark in applied machine learning.

The project follows a structured analytical workflow beginning with data preprocessing and feature engineering. Raw customer data is cleaned and transformed using Pandas, with categorical variables encoded into numerical representations and continuous features appropriately scaled. Missing values are systematically handled to ensure model robustness and prevent data leakage. These steps reflect industry best practices in preparing real-world business data for supervised learning tasks.

Multiple classification algorithms are implemented and compared using scikit-learn, including:

k-Nearest Neighbors (KNN) for distance-based classification,

Decision Trees for interpretable, rule-based modeling,

Multi-Layer Perceptron (MLP) neural networks to capture non-linear relationships.

The dataset is partitioned into training and testing subsets using a hold-out validation framework (train_test_split) to evaluate out-of-sample performance. Model effectiveness is assessed with detailed performance metrics—accuracy, precision, recall, and F1-score—via classification_report, allowing for nuanced comparison across models and an understanding of trade-offs between predictive power and interpretability.

Beyond technical implementation, the project emphasizes model evaluation and business relevance. The churn predictions are framed in a decision-making context, demonstrating how supervised learning can be used to identify at-risk customers and inform retention strategies. The analysis highlights strengths and limitations of each modeling approach, reinforcing the importance of model selection based on both statistical performance and practical deployment considerations.

Overall, this repository demonstrates strong proficiency in applied machine learning, predictive modeling, and data-driven decision support, with clear evidence of the ability to translate raw business data into actionable insights using professional analytics tools.
