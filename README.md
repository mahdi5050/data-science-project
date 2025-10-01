# Wine Quality Prediction Project

This repository contains a Jupyter Notebook for predicting the quality of Portuguese "Vinho Verde" wines using machine learning.

## Contents

- Exploratory Data Analysis (EDA)
- Feature engineering
- Model training and evaluation (classification and regression)
- Visualizations
- Conclusions

## Tech Stack

- Python 3.8+
- Jupyter Notebook
- pandas
- numpy
- seaborn
- scikit-learn
- imbalanced-learn

## Key Visualizations

### Wine Quality Distribution

Red and white wine quality scores are imbalanced, with most samples rated 5 or 6.

![Red wine quality distribution](figures/red_quality_distribution.png)
![White wine quality distribution](figures/white_quality_distribution.png)

### Correlation Heatmaps

Chemical properties show strong correlations, e.g., free/total sulfur dioxide and residual sugar/density.

![Red wine correlation heatmap](figures/red_correlation_heatmap.png)
![White wine correlation heatmap](figures/white_correlation_heatmap.png)

### Quality by Alcohol Category

Alcohol content is discretized into low, mid, and high. Most wines with mid alcohol content are rated 5 or 6.

![Red wine quality by alcohol](figures/red_quality_by_alcohol.png)
![White wine quality by alcohol](figures/white_quality_by_alcohol.png)

### Quality by Sweetness

Sweetness (dry/sweet) is associated with quality. Sweet wines tend to have higher quality scores.

![Red wine quality by sweetness](figures/red_quality_by_sweetness.png)
![White wine quality by sweetness](figures/white_quality_by_sweetness.png)

### Model Performance

Confusion matrices for classification models and regression error distributions show model accuracy and error spread.

![Red wine confusion matrix](figures/red_confusion_matrix.png)
![White wine confusion matrix](figures/white_confusion_matrix.png)
![Red wine regression error](figures/red_regression_error.png)
![White wine regression error](figures/white_regression_error.png)

## Conclusions

- Alcohol and sweetness are moderately correlated with wine quality.
- Highly correlated features (e.g., free/total sulfur dioxide, residual sugar/density) can be dropped to improve model interpretability.
- Logistic Regression and SVM models achieve good accuracy for binary classification of wine quality.
- Linear Regression models provide reasonable predictions for continuous quality scores.
- Hyperparameter tuning and cross-validation help prevent overfitting and improve model reliability.

## Usage

1. Clone the repository.
2. Open the notebook in Jupyter.
3. Run all cells to reproduce the analysis and results.

## Dataset

The notebook uses the publicly available "Vinho Verde" wine quality datasets (red and white) from the UCI Machine Learning Repository.

## License

This project is for educational purposes.
