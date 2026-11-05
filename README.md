# Earthquake Damage Prediction Using Machine Learning

## Project Overview

This project uses machine learning to predict earthquake-induced building damage based on geographical, structural, and construction-related characteristics. The dataset contains approximately **260,000 building records** from the 2015 Gorkha earthquake in Nepal.

The original dataset categorizes damage into three levels:

- **Grade 1:** Low Damage
- **Grade 2:** Medium Damage
- **Grade 3:** High Damage

The current implementation focuses on binary classification, distinguishing Grade 3 damage from Grades 1 and 2 combined.

## Project Objectives

- Analyze building characteristics and earthquake damage patterns.
- Perform exploratory data analysis and feature engineering.
- Develop and compare multiple machine learning classification models.
- Improve predictive performance through hyperparameter tuning and ensemble learning.
- Predict damage severity for new building records.

## Dataset

**Source:** DrivenData — Richter's Predictor: Modeling Earthquake Damage

The dataset contains building-level information, including geographical identifiers, building age, floor count, height, area, foundation type, roof type, superstructure materials, and secondary usage.

## Project Workflow

1. Problem Definition and Data Understanding
2. Data Cleaning and Exploratory Data Analysis
3. Feature Engineering and Data Preprocessing
4. Stratified Train-Test Split (80:20)
5. Model Building and Training
6. Model Evaluation and Comparison
7. Hyperparameter Tuning
8. Ensemble Learning
9. New Building Damage Prediction
10. Results and Conclusions

## Machine Learning Models

The following algorithms were implemented and compared:

- Logistic Regression
- Decision Tree
- Random Forest
- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)
- Histogram-based Gradient Boosting
- XGBoost
- LightGBM
- Soft-Voting Ensemble

## Model Evaluation

Because the dataset has an imbalanced class distribution, the **F1-score** was prioritized alongside accuracy, precision, recall, confusion matrix, and ROC-AUC.

### Best Recorded Model: Soft-Voting Ensemble

The ensemble combines **LightGBM, Gradient Boosting, and Random Forest**.

| Evaluation Metric | Result |
|---|---|
| Test Accuracy | 81.66% |
| Weighted F1-Score | 0.8119 |
| ROC-AUC | 0.8758 |

These results correspond to the binary classification experiment. Further independent validation is required before real-world deployment.

## Technologies Used

- **Programming Language:** Python
- **Data Analysis:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn
- **Machine Learning:** Scikit-learn, XGBoost, LightGBM
- **Development Environment:** Jupyter Notebook / Google Colab
- **Version Control:** Git and GitHub

## Project Structure

```text
Earthquake_damage_prediction/
├── Backend/
├── Dataset/
├── Images/
├── Output/
├── Earthquake_Damage_Project_Report.pptx
├── Modeling Earthquake Damage.docx
└── README.md
```

## Applications

This project demonstrates how predictive modeling can support:

- Building vulnerability assessment
- Disaster risk analysis
- Structural inspection prioritization
- Earthquake preparedness and planning

## Conclusion

The project demonstrates an end-to-end machine learning workflow for earthquake damage prediction. Comparative model evaluation, feature engineering, and ensemble learning helped identify an effective predictive approach.

The Soft-Voting Ensemble achieved the highest recorded test accuracy of **81.66%** on the binary classification task.

## Author

**Iswarya Gudi**

GitHub: [IswaryaGudi](https://github.com/IswaryaGudi)
