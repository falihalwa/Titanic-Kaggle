# Titanic Survival Prediction (Kaggle) This is a simple but insightful Machine Learning project where I explore the Titanic dataset to understand which factors influenced passenger survival, and how a model can capture those patterns.

## 🔍 Objectives

- Practice end-to-end ML workflow: from EDA, preprocessing, feature engineering, to model training & evaluation
- Learn the behavior of tree-based models (Decision Tree & Random Forest)
- Extract meaningful insights from limited, historical data
- Build an interpretable model, not just a performant one

## 📊 Key Insights

- **Gender** plays a major role in survival prediction. Female passengers had significantly higher survival rates.
- The **Cabin** feature was mostly missing, but that missingness itself carries a strong signal. Many passengers with missing cabin info were not survived — possibly because their location couldn't be confirmed.
- Instead of dropping missing values, I preserved them by creating new flags such as `Missing_Age` and `Missing_Cabin`, to retain hidden information.
- Decision Tree was intuitive and easy to interpret, but Random Forest gave more stable and better generalization.

## ⚙️ Modeling Approach

- **Models used**: Decision Tree (baseline), then Random Forest (improved)
- **Cross-validation**: Implemented to evaluate model consistency across different splits
- **No hyperparameter tuning yet** — focus was on understanding the data and model behavior first

## 📁 Structure

- `notebooks/`: Jupyter notebooks for EDA and model training
- `data/`: Contains the training and test sets
- `submission.csv`: Final prediction for the test set (public score: 0.78229 on Kaggle)

## 💡 Future Work

- Try hyperparameter tuning (e.g., GridSearchCV)
- Explore different model types (e.g., Gradient Boosting, Logistic Regression)
- Build a custom pipeline for preprocessing & training
- Try SHAP/LIME for model explainability

## 🧠 What I Learned

This project taught me that good ML is not always about better scores — it's about understanding your data and making thoughtful decisions at each step. Even with limited features, there's value in questioning what’s missing, what patterns exist, and how models actually learn.

---

> “Keep the model simple, keep the reasoning deep.”— Exploratory ML Project 

