
# Flu Shot Learning: Predicting Vaccination Behavior

## Project Overview

This project uses data analysis and machine learning to predict whether individuals received the H1N1 flu vaccine and the seasonal flu vaccine.

The goal is to build a practical classification workflow, covering data exploration, preprocessing, model training, evaluation, and prediction generation.

## Objectives

- Explore the dataset and investigate missing values.
- Prepare numerical and categorical features for modeling.
- Build and compare machine learning classification models.
- Evaluate model performance using ROC AUC.
- Generate prediction probabilities for the test dataset.

## Tools & Technologies

- **Python** — Data analysis and machine learning
- **Pandas & NumPy** — Data manipulation
- **Scikit-learn** — Preprocessing, classification, and evaluation
- **Jupyter Notebook** — Interactive analysis
- **Git & GitHub** — Version control

## Project Workflow

### 1. Data Exploration
Examined the training features, target labels, data types, and missing values to understand the dataset.

### 2. Data Preprocessing
Built a preprocessing pipeline using `ColumnTransformer`:

- Numerical features: missing-value imputation and standardization.
- Categorical features: missing-value imputation and one-hot encoding.
- Unseen categories: handled with `handle_unknown="ignore"`.

### 3. Model Development
Experimented with two classification approaches:

- **Logistic Regression** — A baseline classification model.
- **HistGradientBoostingClassifier** — A tree-based boosting model for capturing more complex patterns.

Used `MultiOutputClassifier` to predict both vaccination targets.

### 4. Model Evaluation
Split the training data into training and validation sets and evaluated each target using ROC AUC.

### 5. Prediction Generation
Retrained the final model on the full training dataset and generated prediction probabilities for the competition test data.

## Repository Structure

```text
flu_project/
├── flu_notebook.ipynb
├── README.md
├── .gitignore
└── my_submission.csv
```

The raw competition datasets are stored locally and excluded from version control.

## Key Learnings

- Data cleaning and missing-value handling
- Numerical and categorical feature preprocessing
- Scikit-learn pipelines and `ColumnTransformer`
- Multi-output classification
- Model evaluation using ROC AUC
- Generating predictions for machine learning competitions

## How to Run

1. Clone this repository.
2. Install the required dependencies.
3. Place the competition datasets in the expected local data directory.
4. Open `flu_notebook.ipynb` in Jupyter Notebook or VS Code.
5. Run the notebook cells in order.

Install the main dependencies:

```bash
pip install pandas numpy scikit-learn jupyter
```

## Project Status

**Status:** Exploratory machine learning project.

This project demonstrates a practical approach to preparing data, training classification models, evaluating performance, and generating predictions.

## Author

**Emirhan Morkoc**

[GitHub Profile](https://github.com/emirhanmorkoc)
