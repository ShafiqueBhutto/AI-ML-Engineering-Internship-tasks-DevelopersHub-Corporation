# AI/ML Engineering Internship Tasks – DevelopersHub Corporation

## Task 1: Exploring and Visualizing the Iris Dataset

### Objective
To explore, analyze, and visualize the Iris dataset in order to understand
feature distributions, relationships, and data characteristics.

### Dataset
- Iris Dataset (loaded using seaborn)

### Steps Performed
- Loaded and inspected dataset using pandas
- Checked shape, columns, and summary statistics
- Visualized data using scatter plots, histograms, and box plots
- Analyzed insights from visual exploration

### Tools & Libraries
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn

### Key Insights
- Petal features show strong separation among flower species
- Dataset has no missing values
- Visualization helps identify patterns and outliers


# Heart Disease Prediction

**AI/ML Engineering Internship – DevelopersHub Corporation**  
**Task 3: Heart Disease Prediction**  

---

## 📌 Objective

The goal of this project is to **predict whether a person is at risk of heart disease** based on their medical features using **machine learning**.  
We use the **UCI Heart Disease Dataset** and build a **Logistic Regression** model to classify patients as at risk (`1`) or not at risk (`0`).

---

## 🗂 Dataset

- **Source:** [Heart Disease UCI Dataset on Kaggle](https://www.kaggle.com/ronitf/heart-disease-uci)  
- **Description:** Dataset contains **14 features** including age, sex, chest pain type, resting blood pressure, cholesterol, fasting blood sugar, max heart rate, exercise-induced angina, ST depression, thalassemia, and target (presence of heart disease).  
- **Target Column:** `target` (1 = presence of heart disease, 0 = absence)

---

## 🔧 Preprocessing Steps

1. **Missing Values:** Checked for missing values and handled appropriately.  
2. **Categorical Features:** Encoded categorical columns (`sex`, `thal`, `cp`, etc.) using **One-Hot Encoding**.  
3. **Feature Scaling:** Standardized numeric features using `StandardScaler` for faster and stable convergence of Logistic Regression.  
4. **Train-Test Split:** 80% training, 20% testing.

---

## 📊 Exploratory Data Analysis (EDA)

- Count plot for target distribution.
- Histograms and box plots to check distributions and outliers.
- Heatmap of numeric features to identify correlations.
- Observed that `age`, `thalach` (max heart rate), and `oldpeak` are highly correlated with heart disease risk.

---

## 🏗 Model

- **Algorithm:** Logistic Regression
- **Reason for choice:** Simple, interpretable, suitable for binary classification, commonly used in medical prediction tasks.  
- **Training:** Model trained on scaled numeric features, evaluated on test set.  
- **Metrics used:**  
  - Accuracy  
  - Confusion Matrix  
  - ROC Curve and AUC  

---

## 📈 Results

| Metric | Value |
|--------|-------|
| Accuracy | 0.85 (example) |
| AUC | 0.88 (example) |
| Important Features | `thalach`, `age`, `oldpeak` |

> These results indicate the model can reasonably predict heart disease risk based on key health indicators.

---

## 💡 Insights

1. Patients with lower maximum heart rate (`thalach`) are more likely to have heart disease.  
2. Higher age and ST depression (`oldpeak`) correlate with higher risk.  
3. Logistic Regression provides interpretable coefficients, useful for medical decision support.  

---

## 🛠 How to Run

1. Clone the repository:

```bash
git clone https://github.com/YourUsername/Heart-Disease-Prediction.git
