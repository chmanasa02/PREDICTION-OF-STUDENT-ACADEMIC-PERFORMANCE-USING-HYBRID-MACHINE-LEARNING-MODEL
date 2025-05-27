# 📚 Student Academic Performance Prediction Using Hybrid ML Model
This repository contains a hybrid machine learning model designed to predict student academic performance. It leverages classification algorithms to identify students at risk of underperforming, helping educators make data-informed decisions to support and improve academic outcomes.
## 📊 Project Overview

### 📌 **Problem Statement** 
The goal of this project is to predict student academic performance using demographic, academic, and behavioral data. The system should help educators intervene early for students at risk.

---

### 🧾 **Dataset** 

* **Source**: `dataset.csv` (CSV format)
* **Records**: \~4400 students
* **Features**: Age, study time, parental education, past grades, absences, etc.
* **Target Variable**: `Target` – Academic performance classification (e.g., Pass/Fail)

---

### 🔄 **Workflow Steps**

#### ✅ **Step 1: Data Preprocessing**

* Checked for null values and data types
* Handled categorical variables with label encoding
* Visualized distributions and correlations using seaborn and matplotlib

#### ✅ **Step 2: Feature Engineering**

* Extracted input features (X) and target variable (y)
* Split the data into training and testing sets (70/30 split)

#### ✅ **Step 3: Model Building**

Trained multiple classification algorithms:

* K-Nearest Neighbors (KNN)
* Logistic Regression (LR)
* Decision Tree (DT)
* Random Forest (RF)
* Support Vector Machine (SVM)
* Neural Networks (MLP Classifier)
* Naive Bayes
* Voting Ensemble
* **Stacked Ensemble Model** (final hybrid model)

#### ✅ **Step 4: Evaluation Metrics**

* Accuracy
* Precision, Recall, F1-score
* Confusion Matrix
* Matthews Correlation Coefficient (MCC)

---

### 🤖 **Algorithms Used & Accuracy**

| Algorithm              | Accuracy (%) |
| ---------------------- | ------------ |
| K-Nearest Neighbors    | \~70.0%      |
| Logistic Regression    | \~78.2%      |
| Decision Tree          | \~69.3%      |
| Random Forest          | \~79.5%      |
| Support Vector Machine | \~74.6%      |
| Neural Network (MLP)   | \~76.8%      |
| Naive Bayes            | \~68.2%      |
| Voting Ensemble        | \~72.8%      |
| **Stacked Ensemble**   | **99.6%**    |

---

### 💡 **Key Insights**

* Hybrid model combining KNN,LR, RF, DT, SVM, MLP, and NB yielded the best performance.
* Features such as **study time, parental education, absences, and past grades** were highly predictive.
* Logistic Regression and Random Forest individually performed well, but stacking improved overall accuracy.

---

### 🛠️ **Tools and Libraries**

* **Languages**: Python
* **Libraries**: Scikit-learn, Pandas, NumPy, Seaborn, Matplotlib
* **Platform**: Jupyter Notebook / Google Colab

---

### 🚀 **How to Run**

```bash
# Clone this repository
git clone https://github.com/your-username/PREDICTION-OF-STUDENT-ACADEMIC-PERFORMANCE-USING-HYBRID-MACHINE-LEARNING-MODEL.git 

# Install dependencies
pip install -r requirements.txt

# Run the notebook
jupyter notebook notebooks/CODE.ipynb
```
