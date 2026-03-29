# 🚢 Titanic Survival Prediction: End-to-End ML Pipeline

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)

## 📌 Project Overview
This project predicts the survival probability of passengers on the Titanic using machine learning. It covers the full data science lifecycle: from handling messy, real-world data to optimizing a classification model.

### Key Achievements:
* **Resolved Overfitting:** Identified and fixed a "100% accuracy" data leakage issue.
* **Feature Engineering:** Created custom features like `IsAlone` and extracted `Titles` from names to improve predictive power.
* **Model Optimization:** Compared Random Forest and Logistic Regression to find the best fit for the dataset size.

---

## 🛠️ Data Strategy

### 1. Data Cleaning
* **Age:** Imputed missing values using the median to maintain distribution.
* **Embarked:** Filled missing entries with the most frequent port ('S').
* **Feature Dropping:** Removed high-cardinality features like `Ticket` and `Cabin` (which had >70% missing data).

### 2. Feature Engineering
* **Sex/Embarked:** Converted categorical strings into numerical values using mapping.
* **IsAlone:** A binary feature derived from `SibSp` (siblings) and `Parch` (parents).

---

## 📊 Model Performance

I tested multiple configurations to find the balance between bias and variance.

| Model | Accuracy | Strategy |
| :--- | :--- | :--- |
| **Random Forest** | **[INSERT YOUR %]** | Main model with tuned `max_depth` |
| **Logistic Regression** | **[INSERT YOUR %]** | Used as a baseline for smaller data slices |

---

## 🚀 How to Use
1.  **Clone the Repo:** `git clone https://github.com/YOUR_USERNAME/Titanic-Survival-Predictor.git`
2.  **Install Dependencies:** `pip install pandas scikit-learn`
3.  **Run the Notebook:** Open `Titanic_Analysis.ipynb` in Jupyter or Colab.

---

## 💡 Lessons Learned
* **Data Quality > Algorithm:** Even a complex Random Forest can't fix a tiny or messy dataset.
* **Validation is Key:** Using Train/Test splits is essential to ensure the model generalizes to new passengers.
