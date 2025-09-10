# Logistic Regression on Synthetic Datasets

📌 Overview

This repository demonstrates Logistic Regression for both binary and multi-class classification problems using synthetic datasets generated with NumPy.

We model two scenarios:

Student Performance → Predict whether a student passes or fails based on study and sleep hours.

Fruit Classification → Predict fruit type (Apple, Banana, Orange) based on sweetness and crunchiness.

⚙️ Features

Generate synthetic datasets with NumPy

Apply Logistic Regression for:

Binary Classification (Pass/Fail)

Multi-class Classification (Fruit types)

Train/Test split for model evaluation

Performance metrics: Accuracy, Precision, Recall, F1-score, Confusion Matrix


📊 Datasets

1️⃣ Student Performance (Binary Classification)

Features:

Hours studied (hours)

Sleep hours (sleep)

Target: Pass or Fail

np.random.seed(42)   
n = 200  
hours = np.random.normal(5, 2, n)  
sleep = np.random.normal(7, 1, n)  
pass_fail = (0.5*hours + 0.3*sleep + np.random.randn(n)) > 5  

2️⃣ Fruit Classification (Multi-class)

Features:

Sweetness

Crunchiness

Target: Fruit type → Apple, Banana, Orange

np.random.seed(42)  
n = 300  
sweetness = np.random.normal(5, 2, n)  
crunchiness = np.random.normal(3, 1, n)  
labels = np.random.choice(["Apple", "Banana", "Orange"], size=n)  

🚀 Tech Stack

Python 3.x

NumPy & Pandas

Matplotlib / Seaborn (visualization)

Scikit-learn (Logistic Regression, metrics)


📈 Results

Binary (Pass/Fail):

Accuracy: 75%

Recall/Precision: Reported in classification report

Confusion Matrix: Visualized

Multi-class (Fruits):

Accuracy: 35%

Multinomial classification report


🔧 Future Improvements


Use real-world datasets (Titanic, Iris, Student dataset)


👩‍🎓 Author

Sonia Firdous
