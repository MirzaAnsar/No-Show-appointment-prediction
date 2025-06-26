# No-Show Appointment Prediction 🚑

This project aims to predict whether a patient will show up for their scheduled medical appointment. The dataset contains over 110,000 records from Brazilian hospitals, and this work was completed as part of my Data Science Capstone at DePaul University.

---

## 📊 Problem Statement

Missed medical appointments ("no-shows") cause significant disruptions in healthcare services. This project builds and evaluates multiple machine learning models to predict no-shows, with a focus on handling class imbalance and identifying key risk factors.

---

## 🧠 Key Features

- Data preprocessing with feature engineering (e.g., `WaitingDays`)
- SMOTE applied to balance class distribution
- Comparison of multiple ML models:
  - Logistic Regression
  - Decision Tree
  - Random Forest
  - XGBoost
  - ANN (Keras)
- Threshold tuning and ensemble learning (Soft Voting)
- Feature importance analysis

---

## 🛠️ Technologies Used

- Python (Pandas, NumPy, Scikit-learn, XGBoost, TensorFlow/Keras)
- Matplotlib, Seaborn for visualization
- SMOTE for class imbalance (from imblearn)
- Jupyter Notebook

---

## 📈 Results

| Model                     | Accuracy | Recall (No-Show) | F1-Score |
|--------------------------|----------|------------------|----------|
| Tuned Decision Tree      | 52.9%    | 59%              | 42%      |
| ANN (threshold = 0.3)    | 41.1%    | 86%              | 45%      |
| Ensemble (RF + XGBoost)  | 63.9%    | 39%              | 38%      |

---

## 📂 Dataset

Data Source: [Kaggle - Medical Appointment No Shows](https://www.kaggle.com/joniarroba/noshowappointments)  
(You may need to download the file manually due to licensing)

---

## 🚀 How to Run

```bash
# Clone the repo
git clone https://github.com/yourusername/no-show-appointment-prediction.git

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter Notebook
jupyter notebook
