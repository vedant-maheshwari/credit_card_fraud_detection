# Credit Card Fraud Detection

This project explores **credit card anomaly detection** using a real-world imbalanced dataset. The key challenge is identifying fraudulent transactions from hundreds of thousands of legitimate ones.

## 📌 Overview
- Dataset is highly skewed towards **non-fraudulent transactions**.
- Applied **feature engineering**: time-based features, rolling statistics, risk encoding, etc.
- Tested multiple models: **Deep Learning architectures, Autoencoders, LightGBM, XGBoost**.
- Ensemble methods (LightGBM & XGBoost) outperformed deep learning in this case.
- Tuned models for different business goals: **high precision** vs. **high recall**.

## ⚙️ Workflow
1. **Data Exploration & Preprocessing**
   - Checked for missing values & duplicates.
   - Feature transformations (log scale, binning, categorical encoding).
   - Domain-specific features: transaction time patterns, distance calculation, merchant risk levels.

2. **Handling Imbalanced Data**
   - Used **SMOTE** oversampling for minority class.

3. **Modeling**
   - Tried Vanilla Deep Learning, Autoencoders, LightGBM, and XGBoost.
   - Hyperparameter tuning with **RandomizedSearchCV**.

4. **Evaluation**
   - Precision, Recall, F1-score, Confusion Matrix.
   - Two parameter sets:
     - **High Precision** (minimizing false positives)
     - **High Recall** (minimizing false negatives)

## 💡 Key Learnings
- **Data quality & feature engineering** often matter more than algorithm choice.
- Deep learning is not always the best—simpler ensemble methods can outperform.
- Avoid **data leakage**: ensure no target-dependent features are created.

## 📊 Example Outputs
- Fraud distribution chart
- Transaction amount vs fraud status plots
- Confusion matrices for different parameter sets

