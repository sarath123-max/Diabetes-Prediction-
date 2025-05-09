
---

# 🧪 Diabetes Prediction Using Naïve Bayes Classifier

This project demonstrates how to build a **Naïve Bayes classification model** to predict whether a person has diabetes based on medical features. The dataset used is `Diabetes.csv`.

---

## 🧬 Overview

The goal is to predict the presence of diabetes using features like glucose levels, BMI, age, etc., by training a **Gaussian Naïve Bayes** classifier.

---

## 📁 Dataset

The dataset should be named `Diabetes.csv` and must contain:

- Independent Features (e.g., `Pregnancies`, `Glucose`, `BloodPressure`, etc.)
- Target Column: `diabetes` (0 or 1)

> Ensure this file is in the same folder as your script.

---

## ⚙️ Technologies Used

- `pandas` for data manipulation
- `scikit-learn` for model building and evaluation

### 📦 Installation
Install the required packages using pip:
```bash
pip install pandas scikit-learn
```

---

## 🧠 Model Details

- **Algorithm:** Gaussian Naïve Bayes
- **Train-Test Split:** 20% training, 80% testing
- **Evaluation Metric:** Accuracy Score

---

## ▶️ How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/diabetes-prediction.git
   cd diabetes-prediction
   ```

2. Make sure `Diabetes.csv` is placed in the project directory.

3. Run the script:
   ```bash
   python diabetes_prediction.py
   ```

4. Sample Output:
   ```
   Model Accuracy: 77.32%
   ```

---

## 📊 Code Summary

```python
from sklearn.naive_bayes import GaussianNB
from sklearn.metrics import accuracy_score

# Train the model
model = GaussianNB()
model.fit(x_train, y_train)

# Predict and evaluate
accuracy = accuracy_score(y_test, model.predict(x_test))
```

---

## 📬 Contact

For any suggestions or questions, feel free to open an issue or reach out.

---
