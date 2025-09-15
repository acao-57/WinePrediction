# Wine Quality Prediction

This project aims to analyze and build a predictive model for wine quality based on its chemical properties. The work involves data exploration, preprocessing, and the evaluation of multiple machine learning models to identify the most significant factors influencing wine quality.

## Project Overview

**Problem Definition:** To determine the most important features for predicting wine quality and to build an effective classification model based on these chemical properties.

The project is structured into three modular Jupyter notebooks, each focusing on a distinct group of chemical attributes. The workflow encompasses data loading, exploratory data analysis (EDA), feature engineering, model training, and evaluation.

## Dataset

The model is built using the `WineQT.csv` dataset from Kaggle:
[Wine Quality Dataset](https://www.kaggle.com/datasets/yasserh/wine-quality-dataset)

**Features:**
*   fixed acidity
*   volatile acidity
*   citric acid
*   residual sugar
*   chlorides
*   free sulfur dioxide
*   total sulfur dioxide
*   density
*   pH
*   sulfates
*   alcohol
*   quality (target)

## Project Structure and Contributions

The repository is organized into three main notebooks, each analyzing a specific subset of features:

1.  @ersulxx: `fixedacidity-volatileacidity-citricacidity-residualsugar.ipynb`
2.  @acao-57: `chlorides-fsd-tsd-sulphates.ipynb`
3.  Jiahuiyue `density-ph-alcohol.ipynb`

## Methodology

1.  **Data Preparation & Cleaning:**
    *   Loaded and inspected data using `pandas`.
    *   Addressed precision issues by rounding excessive decimal places.
    *   Applied log transformation to reduce skewness from outliers.
    *   Scaled features using `RobustScaler` to handle outliers in the data distribution.

2.  **Exploratory Data Analysis (EDA):**
    *   Utilized correlation heatmaps, boxplots, scatterplots, and violin plots to visualize relationships between chemical properties and wine quality.
    *   Identified initial correlations and data distributions.

3.  **Modeling & Evaluation:**
    *   **Models Implemented:** Decision Tree, Random Forest, Linear Regression.
    *   **Evaluation Metrics:** Mean Squared Error (MSE), R² Score, Goodness of Fit, and Confusion Matrix.
    *   Trained and compared models to assess predictive performance.

## Results & Evaluation

The project demonstrates a full data science pipeline, from initial exploration to final model evaluation. Our analysis reveals:

*   **Alcohol content** and **volatile acidity** showed the strongest correlations with wine quality (0.48 and -0.41, respectively).
*   Most attributes had weak individual correlations, indicating that wine quality is a multifactorial outcome.
*   Linear regression proved ineffective due to non-linear relationships and the nature of the quality ratings.
*   Tree-based models (Decision Tree, Random Forest) performed better at capturing non-linear patterns and feature interactions.
*   Grouping features by chemical similarity provided interpretability but did not significantly boost model accuracy, suggesting that complex interactions beyond basic chemistry may influence quality.

## Key Takeaways

*   **Dominant Factors:** Alcohol (positive correlation) and volatile acidity (negative correlation) are the most significant single predictors of quality.
*   **Model Performance:** Tree-based ensemble methods outperformed linear models, though predictive accuracy remains a challenge, highlighting the complexity of the problem.
*   **Data Challenges:** Skewness and outliers were present in many attributes. Scaling and transformations had a limited impact on final model performance.
*   **Conclusion:** Wine quality cannot be simplified to a few key factors; it likely emerges from complex, non-linear interactions between all chemical properties.

## Installation & Usage

**Requirements:**
To run this project, ensure you have the following Python libraries installed:
```bash
pip install pandas numpy seaborn matplotlib scikit-learn jupyter
