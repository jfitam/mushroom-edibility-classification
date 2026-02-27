# Mushroom Poisonous Classification

This project implements a **binary classification model** to identify whether a mushroom is **poisonous or edible** based on its physical characteristics.

The dataset comes from a **synthetic version of the classic mushroom dataset available on Kaggle**, prepared for machine learning classification tasks.

The goal of the project is to demonstrate a **complete classification workflow**, from data preparation to model interpretation.

---

# Project Goal

Correctly identifying poisonous mushrooms is a **safety-critical classification problem**.  
For this reason, the model prioritizes **maximizing recall for the poisonous class**, ensuring that poisonous mushrooms are not misclassified as edible.

---

# Dataset

The dataset contains categorical features describing mushroom characteristics such as:

- cap shape
- cap color
- odor
- gill size
- stalk characteristics
- habitat

Each sample is labeled as:

- **edible**
- **poisonous**

The dataset used in this project is a **synthetic version derived from the original Kaggle dataset**, commonly used for classification practice.

---

# Methodology

The project follows a simple machine learning workflow:

1. Data loading
2. Data cleaning and preprocessing
3. Feature encoding
4. Model training using **Logistic Regression**
5. Model evaluation
6. Feature importance analysis

Categorical features are transformed into numerical representations before training the model.

---

# Model

The classification model used is:

**Logistic Regression**

Logistic regression was chosen because it:

- is interpretable
- works well for binary classification
- allows direct inspection of **feature coefficients**

---

# Evaluation

The model is evaluated using standard classification metrics:

- Accuracy
- Precision
- Recall
- Confusion Matrix

The model achieves:

Recall = 1.0

This means the model **successfully identifies all poisonous mushrooms**, eliminating false negatives.

This behavior is particularly desirable in safety-critical scenarios.

Confusion matrix:

<img width="253" height="216" alt="image" src="https://github.com/user-attachments/assets/27b9f4f8-5471-4419-9902-8b03def96f06" />

---

# Feature Importance

One of the advantages of logistic regression is that model coefficients can be interpreted.

The project analyzes the **weight of each feature in the prediction**, allowing identification of the mushroom characteristics that contribute most strongly to predicting toxicity.

This provides a basic level of **model interpretability**.

<img width="542" height="181" alt="image" src="https://github.com/user-attachments/assets/cc4a8523-6340-415e-a1d0-d8ded9d022f0" />


---

# Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib

---

# Possible Improvements

Future extensions could include:

- testing additional models (Random Forest, Gradient Boosting, SVM)
- performing hyperparameter tuning
- applying cross-validation
- adding SHAP or permutation importance for deeper interpretability
- building a simple prediction interface

---

# License

This project was created for educational and portfolio purposes.
