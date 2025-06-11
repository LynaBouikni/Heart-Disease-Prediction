# 🫀 Heart Disease Prediction with Explainable Machine Learning

##   Overview

This project is an end-to-end machine learning pipeline for predicting the presence of heart disease based on clinical attributes. It explores a full data science workflow—from EDA and preprocessing to model building and SHAP-based interpretability.

The dataset used is the **Cleveland Heart Disease dataset**, available on [Kaggle](https://www.kaggle.com/datasets) and originally sourced from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/).

---

## 📌 Objectives

- Explore the dataset with statistical and visual EDA  
- Build and evaluate multiple classification models  
- Tune hyperparameters for optimal performance
- Evaluate models using metrics beyond accuracy (precision, recall, F1, AUC...etc).
- Use SHAP values for feature importance and prediction explanations  
- Generate patient-level explanations for model decisions  
- Reflect on clinical alignment and model trustworthiness  

---

##  📁 Project Structure

Heart-Disease-Prediction/

```
Heart-Disease-Prediction/
├── data/           # CSV files (raw or processed)
├── images/         # Visuals (SHAP, EDA plots, model comparisons)
├── notebook/       # Jupyter Notebooks
├── requirements.txt
└── README.md
```


---

## 📊 Dataset Features
The dataset contains 303 patient records with 14 attributes:

| Feature     | Description                                              |
|-------------|----------------------------------------------------------|
| `age`       | Age in years                                             |
| `sex`       | (1 = male; 0 = female)                                   |
| `cp`        | Chest pain type (0–3)                                    |
| `trestbps`  | Resting blood pressure                                   |
| `chol`      | Serum cholesterol (mg/dl)                                |
| `fbs`       | Fasting blood sugar > 120 mg/dl                          |
| `restecg`   | Resting electrocardiographic results                     |
| `thalach`   | Max heart rate achieved                                  |
| `exang`     | Exercise-induced angina                                  |
| `oldpeak`   | ST depression induced by exercise                        |
| `slope`     | Slope of the ST segment                                  |
| `ca`        | Number of major vessels (0–3) seen via fluoroscopy       |
| `thal`      | Thalium stress result (1, 3, 6, 7)                        |
| `target`    | Heart disease present (1) or not (0)                     |

---

## 🔁 Workflow Summary

| Step | Task |
|------|------|
| 1️⃣ | Define the problem (binary classification) |
| 2️⃣ | Perform EDA and check class balance |
| 3️⃣ | Preprocess the data (scaling, encoding) |
| 4️⃣ | Train multiple models (LogReg, KNN, RF) |
| 5️⃣ | Evaluate with metrics (F1, AUC, confusion matrix) |
| 6️⃣ | Optimize via GridSearchCV / RandomizedSearchCV |
| 7️⃣ | Interpret results using SHAP (global + local) |

---

## ⚙️ Tools & Libraries
- Python 3.11+  
- pandas, NumPy  
- Scikit-Learn  
- Matplotlib, Seaborn  
- SHAP  
- Jupyter Notebook  

---

## ✅ Results
- **Best model**: Logistic Regression (with hyperparameter tuning)  
- **Cross-validated Accuracy**: ~85%  
- **Precision**: ~82%  
- **Recall**: ~93%  
- **F1 Score**: ~87%  
- **ROC AUC**: > 0.90  

---

## 📈 Explainability with SHAP
- Global feature importance via beeswarm and bar plots  
- Local explanations for high-risk and low-risk patients  
- Clinical reflection on model behavior (e.g., counterintuitive treatment of `thalach` and `oldpeak`)  
- Waterfall plots to show feature contributions for individual predictions  

---

## 🧠 Clinical Takeaways
- The model aligns with known risk factors like `ca`, `thal`, and `cp`  
- Some features (e.g., `thalach`) reveal unexpected effects, possibly due to feature interactions  
- SHAP visualizations make it easier to debug, improve, and trust the model  
- Emphasizes the need for caution when using ML in clinical settings  

---

## ▶️ How to Run
```bash
git clone https://github.com/LynaBouikni/Heart-Disease-Prediction.git
cd Heart-Disease-Prediction
pip install -r requirements.txt
jupyter notebook
```

## 🤝 Acknowledgements
UCI Machine Learning Repository – Heart Disease Dataset

Zero to Mastery – Machine Learning Course by Daniel Bourke

## 📬 Contact
Lyna Bouikni
* Junior Data Scientist | AI & Computational Modeling
* lynabouiknia@gmail.com
🔗 [LinkedIn](https://www.linkedin.com/in/lyna-b-231a41126/)
