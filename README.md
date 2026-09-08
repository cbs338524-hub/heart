# Heart Disease Prediction Using Machine Learning

## Project Overview

This project uses machine learning classification algorithms to predict the presence of heart disease based on patient health-related features.

Three machine learning algorithms are implemented and compared:

* Logistic Regression
* Decision Tree
* Random Forest

The models are evaluated using Accuracy, Precision, Recall, and F1 Score. The best-performing model is selected based on the highest F1 Score.

## Objectives

The main objectives of this project are:

1. Load and explore the heart disease dataset.
2. Clean and preprocess the data.
3. Handle missing values and duplicate records.
4. Convert categorical variables into numerical features.
5. Split the dataset into training and testing sets.
6. Train multiple machine learning classification models.
7. Evaluate model performance.
8. Visualize model results and feature importance.
9. Identify the best-performing algorithm.
10. Export model results for further analysis.

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

## Machine Learning Algorithms

### 1. Logistic Regression

Logistic Regression is a classification algorithm used to predict the probability of a target class.

In this project, the input features are standardized before training the Logistic Regression model.

### 2. Decision Tree

Decision Tree is a supervised learning algorithm that makes predictions using a tree-like structure of decision rules.

The Decision Tree is also visualized to understand how the model makes predictions.

### 3. Random Forest

Random Forest is an ensemble learning algorithm that combines multiple decision trees to improve prediction performance and reduce overfitting.

Feature importance from the Random Forest model is also calculated to identify the most influential features.

## Dataset

The project uses a CSV dataset named:

```text
heart-disease.csv
```

The dataset contains patient-related health information and a target variable indicating the presence or absence of heart disease.

The notebook automatically searches for common target-column names such as:

```text
target
condition
heartdisease
heart_disease
output
label
class
num
```

## Data Preprocessing

The following preprocessing steps are performed:

* Remove unnecessary whitespace from column names.
* Convert column names to lowercase.
* Remove duplicate records.
* Check for missing values.
* Remove patient ID columns when present.
* Convert categorical variables using one-hot encoding.
* Handle missing numerical values using median imputation.
* Convert the target variable into numerical form when necessary.
* Standardize features for Logistic Regression.

## Train-Test Split

The dataset is divided into:

* 80% Training Data
* 20% Testing Data

A random state of `42` is used to make the results reproducible.

Stratified splitting is used to maintain the target-class distribution between training and testing datasets.

## Model Evaluation

The models are evaluated using the following metrics:

### Accuracy

Measures the overall percentage of correct predictions.

### Precision

Measures how many of the observations predicted as positive are actually positive.

### Recall

Measures how many of the actual positive observations were correctly identified.

### F1 Score

The F1 Score is the harmonic mean of Precision and Recall.

The model with the highest F1 Score is selected as the best-performing model.

## Visualizations

The project includes several visualizations:

* Heart Disease Target Distribution
* Age Distribution
* Age vs Heart Disease
* Correlation Heatmap
* Confusion Matrix for each model
* Decision Tree Visualization
* Random Forest Feature Importance
* Accuracy Comparison
* Overall Model Performance Comparison

## Project Workflow

```text
Dataset
   ↓
Data Loading
   ↓
Data Exploration
   ↓
Data Cleaning
   ↓
Missing Value Handling
   ↓
Feature Engineering
   ↓
Train-Test Split
   ↓
Feature Scaling
   ↓
Model Training
   ↓
Model Evaluation
   ↓
Model Comparison
   ↓
Feature Importance
   ↓
Best Model Selection
```

## Project Files

A typical repository structure is:

```text
Heart-Disease-Prediction/
│
├── heart-disease.csv
├── heart_disease_prediction.ipynb
├── heart_disease_model_results.csv
├── random_forest_feature_importance.csv
└── README.md
```

## Output Files

The notebook generates two CSV files:

### `heart_disease_model_results.csv`

Contains the performance results of the three machine learning algorithms.

The results include:

* Accuracy
* Precision
* Recall
* F1 Score

### `random_forest_feature_importance.csv`

Contains the feature importance values calculated by the Random Forest model.

## How to Run the Project

### 1. Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### 2. Open the project folder

```bash
cd Heart-Disease-Prediction
```

### 3. Install the required libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### 4. Start Jupyter Notebook

```bash
jupyter notebook
```

### 5. Open the notebook

Open:

```text
heart_disease_prediction.ipynb
```

### 6. Make sure the dataset is available

Place:

```text
heart-disease.csv
```

in the same directory as the notebook.

### 7. Run the notebook

Run the cells from top to bottom.

## Results

The project compares the three classification algorithms using Accuracy, Precision, Recall, and F1 Score.

The final notebook automatically identifies the best-performing algorithm based on F1 Score.
```

The actual values depend on the dataset used and the resulting train-test split.

## Feature Importance

Random Forest feature importance is used to identify which patient features contribute most to the model's predictions.

The feature importance results are saved in:

```text
random_forest_feature_importance.csv
```

## Limitations

This project is intended for educational and machine learning practice purposes.

The model should **not be used as a medical diagnostic system**. Real-world medical prediction requires clinically validated datasets, appropriate evaluation, external validation, and professional medical oversight.

## Future Improvements

Possible improvements include:

* Hyperparameter tuning using GridSearchCV or RandomizedSearchCV.
* Cross-validation.
* Comparing additional algorithms such as SVM, KNN, and Gradient Boosting.
* Handling class imbalance when necessary.
* Using ROC-AUC and Precision-Recall curves.
* Performing feature selection.
* Improving model interpretability.
* Testing the models on an independent external dataset.
* Deploying the best model as a web application.

## Conclusion

This project demonstrates the application of machine learning classification techniques to heart disease prediction.

Logistic Regression, Decision Tree, and Random Forest models are trained and evaluated using multiple performance metrics.

The best-performing model is selected based on F1 Score, while feature importance and visualizations provide additional insight into the model's predictions.

---

## Author

**Your Name**

[GitHub: `https://github.com/YourUsername`](https://github.com/cbs338524-hub/heart.git)

