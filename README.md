# MiniProject- Wine Quality Prediction Repository

About

This project aim to analyze and create a prediction model based on different chemical properties that effect wine quality. The dataset used in this model is WINEQT.csv and is from the following kaggle: https://www.kaggle.com/datasets/yasserh/wine-quality-dataset.

In order to run this project the following libraries are required python 3, pandas, numpy, seaborn, matplotlib, scikit-learn.

Problem Definition:  To determine which features are most important in predicting wine quality and to build an effective classification model based on these properties.

Project Structure: 
The structure of the project includes data loading and preparation, exploratory data analysis, model training and evaluation and model comparison. The mini project is divided into three separate python notebooks for better modularity. The projects key takeways and a evalution is highlighted as well as which contributator worked on which notebook and the notebooks content. 

1. Data Description
2. Data loading and preparation
3. Exploratory Data Analysis
4. Model comparision
5. Model analysis
6. Evaluation
7. Key Takeaways
8. Notebooks
9. Contributions
____________________________________________________________________

1. Data Description
The dataset contains the following: fixed acidity, volatile acidity, citric acid, residual sugar, chlorides, free sulfur dioxide, total sulfur dioxide, density, pH, sulfates, alcohol and quality.

2. Data loading and preparation
- The dataset is loaded using pandas and described using .info and .describe
- Log Transformation is used to reduce skewness effect of outliers.
- Robust scaler

3. Exploratory Data Analysis
- Heatmap shows the relationships between fixed features for each notebook.
- Boxplot, scatterplots and violin plots are used to visualize these chemical properties and their relationship with quality of the wine.

4. Model Comparison  
- Decision Tree
- Random Forest
- Linear Regression

5. Model analysis
- Mean squared error
- Goodness of fit
- R^2 Score
- Confusion Matrix

6. Evaluation
- The project showcases data science fundamentals, from data exploration to model evaluation. Each notebook is well-organized around key chemical properties, with logical progression from exploratory data analysis to modeling. The final results underline that while logistic regression offers a straightforward approach, the neural network captures more complex patterns, resulting in higher accuracy. The project shows a correlation bewtten for example alchol content and volatile acidity effecting the overal wine quality score, however the result also shows that wine quilty can't just be simplified to a few key factors. In order to understand wine quality better, the relationship between each chemical properity should be explored furthur. 

7. Key Takeaways
- Alcohol content and volatile acidity show the strongest correlations with wine quality, with values of 0.48 (alcohol) and -0.41 (volatile acidity), respectively.
Most attributes have weak correlations with quality, suggesting that no single feature dominates in determining wine quality.Wine quality is multifactorial, likely requiring a combination of attributes rather than relying on a single predictor.

- Data cleaning involved handling precision issues, like rounding excessive decimal places (e.g.,0.7200000000000001) to maintain consistency across features. Visualizations highlighted skewness and outliers in many attributes, but removing them wasn’t ideal, as they could contain valuable information. Scaling techniques (log transformations, robust scaling) had limited effect on model improvement,showing the challenge of addressing skewed distributions effectively.
  
- Linear regression was ineffective due to non-linear relationships and the ordinal nature of the quality ratings. Decision trees and random forest classifiers improved predictive power slightly, as they better handle non-linear data and feature interactions.
  
- Grouping features by chemical similarity (e.g., acidity types, sulfur compounds) helped in capturing interactions but didn’t significantly boost model accuracy. Purely chemical-based models struggle with high predictive accuracy, suggesting wine quality may involve complex interactions not reflected in chemical data alone.

8. Notebooks
- fixedacidity-volatileacidity-citricacidity-residualsugar
- chlorides-fsd-tsd-sulphates
- density-ph-alchol

9. Contributions
-  @ersulxx fixedacidity-volatileacidity-citricacidity-residualsugar
-  @acao-57  chlorides-fsd-tsd-sulphates
-   Jiahuiyue  density-ph-alchol

Link to power point: https://docs.google.com/presentation/d/1mzXFIEh3CIzrWwn4ftEVO_lcgcq6BlHc7FC3yBKqyrE/edit?fbclid=IwZXh0bgNhZW0CMTAAAR3wZZW5P6VNuic79ET_MRV6__ikmLmZLWkKUOXEvhwg2L60Qzyok-Mi5zI_aem_9eGi1rKv6rDFSWDxSOYRJA#slide=id.g313982179b3_0_352

Link to video:https://drive.google.com/file/d/1zxHNvUr4m2K-qMpyZ6p__Pn-8fp0TqyZ/view?usp=sharing
