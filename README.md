# MiniProject- Wine Quality Prediction
This project aim to analyze and create a prediction model based on different chemical properties that effect wine quality. The dataset used in this model is WINEQT.csv and is from the following kaggle: https://www.kaggle.com/datasets/yasserh/wine-quality-dataset.

In order to run this project the following libraries are required python 3, pandas, numpy, seaborn, matplotlib, scikit-learn.

The structure of the project includes data loading and preparation, exploratory data analysis, model training and evaluation and model comparison. 

Data Description
The dataset contains the following: fixed acidity, volatile acidity, citric acid, residual sugar, chlorides, free sulfur dioxide, total sulfur dioxide, density, pH, sulfates, alcohol and quality.

Data loading and preparation
- The dataset is loaded using pandas and described using .info and .describe
- Log Transformation is used to reduce skewness effect of outliers.
- Robust scaler

Exploratory Data Analysis
- Heatmap shows the relationships between fixed features for each notebook.
- Boxplot, scatterplots and violin plots are used to visualize these chemical properties and their relationship with quality of the wine.

Model Comparison  
- Decision Tree
- Random Forest
- Linear Regression

Model analysis
- Mean squared error
- Goodness of fit
- R^2 Score

Link to power point: https://docs.google.com/presentation/d/1mzXFIEh3CIzrWwn4ftEVO_lcgcq6BlHc7FC3yBKqyrE/edit?fbclid=IwZXh0bgNhZW0CMTAAAR3wZZW5P6VNuic79ET_MRV6__ikmLmZLWkKUOXEvhwg2L60Qzyok-Mi5zI_aem_9eGi1rKv6rDFSWDxSOYRJA#slide=id.g313982179b3_0_352
