# Predicting Diabetes Using Machine Learning

Classification of diabetes risk on the Pima Indians Diabetes Dataset, comparing four ML models in R. Data Mining Principles project, Bucharest University of Economic Studies (2025).

## Key Findings

- **Logistic Regression** gave the best overall performance.
- **Glucose** and **BMI** were the strongest predictors.
- The dataset contains class imbalance across several variables.

## Methods

- Target encoded as factor (pos/neg); 70/30 train/test split
- Missing-value and outlier handling
- Univariate/bivariate analysis and correlation matrix (`corrplot`)
- Models: Random Forest, XGBoost, KNN, Logistic Regression
- Evaluation: sensitivity, specificity, precision, recall, F1, ROC/AUC, confusion matrix

## Setup

```r
install.packages(c("caret", "tidyverse", "MASS", "mlbench", "summarytools",
                   "corrplot", "gridExtra", "timeDate", "pROC", "caTools",
                   "rpart.plot", "e1071", "graphics"))
source("cod.R")
```

Dataset: [Pima Indians Diabetes (Kaggle)](https://www.kaggle.com/uciml/pima-indians-diabetes-database) — place in the working directory before running.

## Authors

Ariton Alexandru, Bucur Alexia-Gabriela, Coman Alex, Cojocaru Florin
