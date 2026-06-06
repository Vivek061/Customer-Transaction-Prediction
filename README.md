# Customer Transaction Prediction

## 📌 Project Overview

Customer Transaction Prediction is a machine learning classification project that predicts whether a customer will make a transaction based on anonymized customer attributes. The goal is to build an accurate predictive model that helps businesses identify potential customers and improve marketing efficiency.

This project includes data preprocessing, exploratory data analysis (EDA), model training, hyperparameter tuning, and performance evaluation using multiple machine learning algorithms.

---

## 🎯 Business Problem

Organizations often struggle to identify customers who are likely to make a purchase. By predicting customer transaction behavior, businesses can:

* Improve customer targeting
* Reduce marketing costs
* Increase conversion rates
* Enhance customer engagement
* Support data-driven decision making

---

## 📂 Dataset Information

* **Total Records:** 200,000
* **Total Features:** 202
* **Target Variable:** `target`

  * 0 = No Transaction
  * 1 = Transaction
* **Feature Variables:** `var_0` to `var_199`
* **ID Column:** `ID_code`

The dataset contains anonymized numerical features, making feature engineering and model selection critical for achieving good performance.

---

## 🛠️ Project Workflow

### 1️⃣ Data Collection

* Imported dataset using Pandas
* Examined dataset structure and dimensions

### 2️⃣ Data Preprocessing

* Checked missing values
* Checked duplicate records
* Separated features and target variable
* Performed train-test split

### 3️⃣ Exploratory Data Analysis (EDA)

* Target variable distribution analysis
* Feature distribution analysis
* Correlation investigation
* Statistical summary of variables

### 4️⃣ Model Building

The following machine learning models were implemented:

* Logistic Regression
* Decision Tree Classifier
* Random Forest Classifier
* Tuned Random Forest (GridSearchCV)

### 5️⃣ Model Evaluation

Evaluation metrics used:

* Accuracy Score
* Precision
* Recall
* F1-Score
* Confusion Matrix
* ROC-AUC Score

---

## 📊 Model Performance

| Model               | Accuracy |
| ------------------- | -------- |
| Logistic Regression | 91.00%   |
| Decision Tree       | 83.43%   |
| Random Forest       | 89.76%   |
| Tuned Random Forest | 89.76%   |

### Best Performing Model

✅ **Logistic Regression**

Achieved the highest test accuracy while maintaining a balanced performance across classes.

---

## 🔍 Feature Importance

Random Forest Feature Importance analysis identified several highly influential variables, including:

* var_81
* var_12
* var_139
* var_53
* var_110

These features contributed significantly to transaction prediction.

---

## 📈 Key Insights

* Logistic Regression outperformed tree-based models on the test dataset.
* Decision Tree showed overfitting tendencies.
* Random Forest improved generalization but struggled with minority class prediction.
* Class imbalance affected recall for transaction prediction.
* Feature importance analysis provided insights into the most influential variables.

---

## 🚀 Future Improvements

* Apply SMOTE for class balancing
* Perform advanced feature engineering
* Experiment with XGBoost
* Implement LightGBM
* Try CatBoost
* Optimize hyperparameters further
* Use cross-validation for more robust evaluation

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* Jupyter Notebook

---

## 📁 Project Structure

```text
Customer-Transaction-Prediction/
│
├── Customer Transaction Prediction.ipynb
├── README.md
├── dataset.csv
│
├── images/
│   ├── confusion_matrix.png
│   ├── roc_curve.png
│   └── feature_importance.png
│
└── requirements.txt
```

---

## ⚙️ Installation

```bash
git clone https://github.com/yourusername/Customer-Transaction-Prediction.git

cd Customer-Transaction-Prediction

pip install -r requirements.txt
```

---

## ▶️ Run the Project

```bash
jupyter notebook
```

Open:

```text
Customer Transaction Prediction.ipynb
```

and run all cells.

---

## 📌 Results

The project successfully predicts customer transaction behavior with **91% accuracy** using Logistic Regression. The findings demonstrate the effectiveness of machine learning in customer behavior prediction and provide valuable business insights for targeted marketing strategies.

---

## 👨‍💻 Author

**Vivek Bhosale**

* Data Scientist
* Data Analyst
* Frontend Developer
* Linux Enthusiast

If you found this project useful, consider giving it a ⭐ on GitHub.
