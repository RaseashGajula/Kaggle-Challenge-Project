

https://github.com/user-attachments/assets/c32950e5-def3-4109-9ba7-e1111300ca78

![IMG_5002](https://github.com/user-attachments/assets/b8d33f1d-566a-4d67-a434-602b29eb4838)
# Kaggle-Challenge-Project: Mushroom Classification Challenge

## Overview

The **Mushroom Classification Challenge** involves predicting whether a mushroom is **edible** (labeled as 'e') or **poisonous** (labeled as 'p') based on various characteristics. The goal is to develop a model that can accurately determine a mushroom's edibility, which is a critical task that could potentially save lives.

## Problem Description

The challenge aims to create a reliable model that can classify mushrooms as either **edible** or **poisonous**. The dataset contains 23 features describing different mushroom characteristics, such as **color**, **texture**, **odor**, **gill size**, and **habitat**. These features help build a system capable of identifying mushrooms and preventing potential poisoning from wild mushrooms.

### Importance

This challenge is essential for creating a safe and reliable system that can accurately identify mushrooms, ultimately protecting public safety and preventing poisoning from wild mushrooms.

---

## Summary of Performance

The task was to predict whether a mushroom is **edible** or **poisonous**.

- The **Random Forest model** successfully predicted the correct classification with high accuracy.
- The **Naive Bayes model** achieved an impressive **99% accuracy**, making it a strong model for predicting the categories.

---

## Summary of Work Done

### Data Details:
- **Rows**: 8,124
- **Columns**: 23

### Preprocessing / Clean-Up:
- Checked for and addressed missing values.
- **Categorical Encoding**: Used **Label Encoding** and **One-Hot Encoding** for features like `gill-size`, `odor`, etc.
- Removed irrelevant columns (e.g., ID columns) to enhance model efficiency.
- Split the dataset into **training** and **validation** sets.
- Scaled the features where necessary to improve model accuracy.

### Data Visualization:
- **Bar Plot**: Shows the distribution of **edible** vs **poisonous** mushrooms in the dataset.
- **Heatmap**: Visualizes the correlation between numerical features. Identifying strong correlations helps with feature selection, which can improve model efficiency.

---

## Problem Formulation

To classify mushrooms as either **edible** or **poisonous**, various models were tested. The **hyperparameters** were tuned to optimize the models' performance. **Cross-validation** was used to assess model generalization. **Random Forest** and **SVM** performed well due to their robustness and ability to handle complex data.

---

## Training Process

The training process was straightforward for simpler models like **Naive Bayes** and **Logistic Regression**, but **Random Forest** and **SVM** required more effort for fine-tuning due to their complexity. 

- Issues like **overfitting** and **class imbalance** were managed using:
  - **Cross-validation**
  - **Early stopping**
  - **Hyperparameter tuning**

Fortunately, there were no significant difficulties in the process.

---

## Performance Comparison

The **ROC Curve** illustrates the trade-off between **sensitivity** (True Positive Rate) and **specificity** (False Positive Rate). A model with an **AUC** close to **1** is considered to perform well, as it indicates the model's ability to differentiate between edible and poisonous mushrooms.

- **Random Forest** achieved the highest **AUC**, indicating its superior ability to distinguish between the two classes.

---

## Conclusion

The **Random Forest model** emerged as the most reliable, providing the best balance between **accuracy** and **generalization**.

---

## Future Work

The next steps could include:
1. **Hyperparameter Tuning**: Further optimization to enhance model performance.
2. **Feature Engineering**: Creating new features or combining existing ones to improve predictions.
3. **Advanced Machine Learning Techniques**: Exploring more advanced methods, such as deep learning or ensemble methods.

---

## Results

The models achieved good performance, with **Random Forest** and **Naive Bayes** performing particularly well in predicting mushroom edibility.

---

## Software Setup

To reproduce the results, the following libraries are required:

- **Pandas**: Data manipulation (`pip install pandas`)
- **NumPy**: Numerical operations (`pip install numpy`)
- **Scikit-learn**: Machine learning models and utilities (`pip install scikit-learn`)
- **Matplotlib**: Plotting and visualizations (`pip install matplotlib`)
- **Seaborn**: Enhanced visualizations (`pip install seaborn`)

You can set up these libraries in your local environment or use **Google Colab**, which has them pre-installed.

---

## Data

You can download the dataset from Kaggle:

- **Dataset**: [Mushroom Classification Dataset](https://www.kaggle.com/datasets/uciml/mushroom-classification/data)

---

## Citations

- **Mushroom Classification.** (2016, December 1). Kaggle. [Mushroom Classification Dataset on Kaggle](https://www.kaggle.com/datasets/uciml/mushroom-classification/data)

---

By following these steps, you can reproduce the results or apply the models to new data for your own study.
