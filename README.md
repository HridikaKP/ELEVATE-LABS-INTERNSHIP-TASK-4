🧪 Logistic Regression - Breast Cancer Classification
This project implements a binary classification model using Logistic Regression to classify tumors as malignant (M) or benign (B) using the Breast Cancer Wisconsin dataset.

📂 Dataset
Source: Breast Cancer Wisconsin Diagnostic Dataset

Total samples: 569

Features: 30 numeric features describing cell nuclei characteristics

Target: diagnosis (M = Malignant, B = Benign)

🛠 Tools & Libraries
Python

Pandas

NumPy

Matplotlib

Scikit-learn

🚀 Tasks Performed
Data Preprocessing

Dropped irrelevant columns (id, Unnamed: 32)

Converted diagnosis labels from M/B to binary 1/0

Split data into training and test sets

Standardized feature values

Model Building

Trained a Logistic Regression model using scikit-learn

Predicted class labels and probabilities on the test set

Model Evaluation

Used metrics:

Confusion Matrix

Precision, Recall, F1-Score

ROC-AUC Score

Plotted ROC Curve

Threshold Tuning

Adjusted classification threshold (e.g., from 0.5 to 0.3) to observe performance impact

Understanding the Sigmoid Function

Visualized the sigmoid function used in logistic regression to map inputs to probabilities

📊 Results Snapshot
ROC-AUC Score: ~0.99 (very high)

Model performed well in identifying malignant and benign tumors with proper tuning.

📌 How to Run
Ensure you have Python installed with the required libraries:

bash
Copy
Edit
pip install pandas numpy matplotlib scikit-learn
Place the breast cancer data.csv in the same directory.

Run the script:

bash
Copy
Edit
python logistic_regression_breast_cancer.py
🧠 Sigmoid Function Intuition
The sigmoid function converts real-valued inputs into a probability range between 0 and 1:

python
Copy
Edit
def sigmoid(z):
    return 1 / (1 + np.exp(-z))
It's what powers the output of logistic regression for binary decisions.

