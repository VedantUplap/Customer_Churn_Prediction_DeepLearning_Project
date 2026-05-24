# Customer Churn Prediction using Deep Learning

A Deep Learning based Customer Churn Prediction System built using TensorFlow, Keras, Streamlit, and Scikit-learn.

This project predicts whether a customer is likely to leave (churn) based on customer information such as credit score, geography, age, balance, salary, and account activity.

---

# Features

- Customer churn prediction using ANN (Artificial Neural Network)
- Deep Learning model built using TensorFlow/Keras
- Data preprocessing and feature engineering
- One-hot encoding and label encoding
- Feature scaling using StandardScaler
- Interactive Streamlit web application
- TensorBoard visualization support
- Model saving and loading using Pickle and H5

---

# Technologies Used

- Python
- TensorFlow
- Keras
- Scikit-learn
- Pandas
- NumPy
- Streamlit
- Matplotlib
- TensorBoard

---

# Project Structure

```bash
Customer_Churn_Prediction_DeepLearning_Project/
│
├── Data/
│   └── Churn_Modelling.csv
│
├── Notebook/
│   └── churn_DeepLearning.ipynb
│
├── app.py
├── model.h5
├── scaler.pkl
├── label_encoder_gender.pkl
├── onehot_encoder_geo.pkl
├── requirements.txt
├── .gitignore
└── README.md
```

---

# Dataset

Dataset used: Churn Modelling Dataset

Features include:
- Credit Score
- Geography
- Gender
- Age
- Tenure
- Balance
- Number of Products
- Has Credit Card
- Is Active Member
- Estimated Salary

Target:
- Exited (1 = Churn, 0 = No Churn)

---

# ANN Architecture

The Artificial Neural Network consists of:

- Input Layer
- Hidden Layer 1 → 64 neurons (ReLU)
- Hidden Layer 2 → 32 neurons (ReLU)
- Output Layer → 1 neuron (Sigmoid)

Loss Function:
- Binary Crossentropy

Optimizer:
- Adam

---

# Model Performance

The model predicts customer churn probability and classifies customers as:

- Likely to Churn
- Not Likely to Churn

---

# Installation

Clone the repository:

```bash
git clone https://github.com/VedantUplap/Customer_Churn_Prediction_DeepLearning_Project.git
```

Move into the project directory:

```bash
cd Customer_Churn_Prediction_DeepLearning_Project
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

# Run the Streamlit App

```bash
streamlit run app.py
```

---

# TensorBoard Visualization

Run TensorBoard:

```bash
tensorboard --logdir logs/fit
```

---

# Example Prediction

Input:
- Credit Score: 750
- Geography: Germany
- Age: 55
- Balance: 120000
- Active Member: No

Output:
```bash
Churn Probability: 0.82
The customer is likely to churn.
```

---
# Author

Vedant Uplap

GitHub:
https://github.com/VedantUplap

---
