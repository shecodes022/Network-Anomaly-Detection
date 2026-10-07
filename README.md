# About this Repository 📌

This repository contains the mini project I did as a part of the coursework for the module Applications of AI. The project builds an anomaly detection system for healthcare cloud database systems, using a Random Forest classifier on the NSL-KDD network intrusion dataset and SHAP to explain the model's predictions.


# Key Takeaways 🔍

1. Data Preparation: Loaded the KDDTrain+ and KDDTest+ datasets, checked for duplicates and missing values, removed the non-feature `difficulty` column and encoded the categorical features.

2. Label Engineering: Converted the multi-class attack labels into a binary attack vs normal problem and examined the class imbalance in both datasets.

3. Exploratory Data Analysis: Visualised class balance, the distribution of protocol type, flag and service, and a correlation heatmap of the numerical features.

4. Model Development: Trained a Random Forest classifier with balanced class weights on a stratified 80/20 train and validation split.

5. Evaluation: Assessed the model using accuracy, precision, recall, F1, ROC and PR curves, confusion matrix, false positive and false negative rates, MCC and balanced accuracy.

6. Explainable AI: Used SHAP to identify the features that most influence the model's attack predictions.


# Stack 🛠️

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)


# Environment 👩🏻‍💻
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)


# Libraries ⚙️

![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=for-the-badge&logo=python&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-4C8CBF?style=for-the-badge&logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![SHAP](https://img.shields.io/badge/SHAP-FF0051?style=for-the-badge&logo=python&logoColor=white)


# Repository Structure 🌲
```text
├──.gitattributes
├── KDDTest+.txt
├── KDDTrain+.txt
├── Mini_Project.ipynb
└── README.md
```

# Reflection 🪞
This project showed how machine learning can support security in sensitive environments such as healthcare databases, where missing an attack is far more costly than raising a false alarm. Looking beyond accuracy to metrics like FPR, FNR, MCC and balanced accuracy gave a more honest picture of how the model performs on imbalanced intrusion data.

Using SHAP also highlighted the value of explainability, since being able to see which network features drive a prediction makes the model easier to trust and act on.
