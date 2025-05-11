# 🏦 Loan Approval Prediction using Machine Learning

This project aims to predict whether a loan should be approved based on applicant data using multiple machine learning models. The project was created as a showcase of my learning in Python for Machine Learning, focusing on real-world data handling, model comparison, and interpretability.

---

## 📌 Problem Statement

Loan approval is a critical decision-making process for financial institutions. This project uses historical data to predict loan approval (`Loan_Status`) based on factors such as income, credit history, employment status, and more.

---

## 📊 Dataset

- Source: [Loan Prediction Problem Dataset (Kaggle)](https://www.kaggle.com/datasets/altruistdelhite04/loan-prediction-problem-dataset)
- Files used:
  - `Train_data.csv` – training and validation
  - `Test_data.csv` – final unseen prediction

---

## 🧹 Data Preprocessing

- **Missing values** handled using median (for numeric) and mode (for categorical).
- **Outliers** detected using IQR method and replaced with column median.
- **Categorical variables** encoded using one-hot encoding.
- **Feature scaling** applied using `StandardScaler` (for models like Logistic Regression, KNN).
- **Irrelevant features** like `Loan_ID` dropped. 
- **Fairness-aware**: Features like `Gender` were evaluated and dropped due to ethical concerns despite minor accuracy gain.

---

## 🤖 Models Used

| Model               | Accuracy | Precision | Recall  | F1 Score |
|--------------------|----------|-----------|---------|----------|
| Logistic Regression| 82.7%    | 81.5%     | 98.5%   | 89.2%    |
| K-Nearest Neighbors| 81.08%    | 81.13%     | 96.26% | 88.05%    |
| Random Forest       | 79.45%    | 81.57%     | 92.53%   | 86.71%    |

---

## ✅ Final Model Selected

**Logistic Regression** was selected due to:
- High **recall** (98.5%) – minimizing false negatives is important in financial approval.
- Consistency across feature variations.
- Simplicity and interpretability for deployment.

---

## 📦 Project Structure

├── Loan_Prediction.ipynb       # Full analysis and modeling
├── Train_data.csv              # Training data
├── Test_data.csv               # Unlabeled test data
├── README.md                   # Project overview (this file)



---

## 📈 Key Visualizations

- Box plots for outlier detection
- Heatmaps to analyze feature correlations
- Confusion matrices and performance bar plots for model comparison

---

## 📤 Model Deployment Note

Although the dataset includes a separate test file, this project focuses on training, validating, and comparing models using the training dataset only. Final model predictions on unseen data were not performed in this version but could be implemented as a next step.


---

## 🙋‍♂️ Author

**Rohit Anand Bangar**  
*Aspiring Data Scientist | Machine Learning Enthusiast*

📌 Built to apply and showcase skills learned in Python, Pandas, NumPy, and scikit-learn.

---

## 🔗 Connect

- https://www.linkedin.com/in/rohit-bangar-24b174305/
- 

---

## ⭐ Acknowledgements

Thanks to Kaggle(https://www.kaggle.com/) for providing the dataset.




