# 🫀 Heart-Disease-Prediction



##   Overview

This project is an end-to-end machine learning pipeline designed to predict the presence of heart disease in patients based on clinical attributes. It's built for binary classification and implements essential data science workflows, from exploratory data analysis (EDA) to model tuning and evaluation.

The dataset used comes from the **Cleveland Heart Disease dataset**, made accessible via [Kaggle](https://www.kaggle.com/datasets) and originally from the UCI Machine Learning Repository.

---

## 📌 Objectives

- Understand the heart disease dataset through visual and statistical EDA.
- Build and compare multiple classification models.
- Optimize models using hyperparameter tuning.
- Evaluate models using metrics beyond accuracy (precision, recall, F1, AUC).
- Interpret model decisions through feature importance.
- Apply reproducible and ethical data science practices.

---

##   Project Structure

heart-disease-prediction/
├── data/ # Dataset (link to Kaggle API)
├── notebook.ipynb # Full end-to-end Jupyter notebook
├── images/ # Visuals used in README
├── requirements.txt # Python dependencies
└── README.md # Project documentation (this file)

---

## 🧬 Dataset

The dataset includes 303 samples and 14 features:

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
| `ca`        | Number of major vessels (0–3) colored by fluoroscopy     |
| `thal`      | Thalium stress result (normal/fixed/reversible defect)   |
| `target`    | Heart disease present (1) or not (0)                     |

---

## 🔁 ML Workflow

| Step | Description |
|------|-------------|
| 1️⃣ Problem Definition       | Predict presence of heart disease (binary classification) |
| 2️⃣ Data Exploration (EDA)  | Understand the data structure and relationships            |
| 3️⃣ Model Building          | Logistic Regression, KNN, Random Forest                    |
| 4️⃣ Model Evaluation        | Confusion Matrix, ROC AUC, Precision, Recall, F1           |
| 5️⃣ Hyperparameter Tuning   | RandomizedSearchCV, GridSearchCV                           |
| 6️⃣ Insights & Reporting    | Feature importance, cross-validated metrics                |

---

## ⚙️ Tech Stack

- Python 3.11+
- pandas, NumPy
- Matplotlib, Seaborn
- Scikit-Learn
- Jupyter Notebook

---

## 📊 Results

- **Best model**: Logistic Regression (tuned)
- **Accuracy**: ~85% (cross-validated)
- **Precision**: ~82%
- **Recall**: ~93%
- **F1-score**: ~87%
- **ROC AUC**: > 0.90

---

## 📁 How to Run

```bash
git clone https://github.com/<your-username>/heart-disease-prediction.git
cd heart-disease-prediction
pip install -r requirements.txt
jupyter notebook

🤝 Acknowledgements
UCI Machine Learning Repository – Heart Disease Dataset

Zero to Mastery – Machine Learning Course by Daniel Bourke

📬 Contact
Lyna Bouikni
* Junior Data Scientist | AI & Neuroscience
* lynabouiknia@gmail.com
🔗 [LinkedIn](https://www.linkedin.com/in/lyna-b-231a41126/)
