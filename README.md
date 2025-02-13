# Diamonds price analysis

The analysis is intented to give the answer **what factors affect the price of diamonds the most**.

## Motivation

In this study the exploratory data analysis (**EDA**) with visualizations of diamond specifications of **56000 diamonds** have been performed to make a relevant predictions.
In main I have used different **linear regression models** with strong accent on the common ones like **Ridge, Lasso, ElasticNet** and other ones like **Random Forest, Gradient Descent and XGBoost** to resolve the issue.


#### The project is created with Python libraries:

 -  scikit-learn/pandas/numpy.

### Recap

In this project I have used several linear regression algorithms for diamonds price prediction, mainly the most popular ones like **Ridge, Lasso, ElasticNet** and other ones like **Random Forest, Gradient Descsent and XGBoosts**. The **best model** turned out to be a **Random Forest one**. I achieved **the smallest RMSE (605,57)** and **the highest R-Squared (0.97)**. I have also used **GridSearch** to find the **best hyperparameters of Random Forest model** and to check if that result can be improved. By virtue of the GridSearch method I did not manage to improve the result since I got slightly worse one - the **RMSE (790,41)** and the **R-Squared (0.96)**. Additionally **the most significance variable** in my analysis is **"volume"**.

Model | R-Squared | RMSE
------------ | ------------- | -------------
Random Forest | 0.971 | 605.57
XGBoost Classifier | 0.972 | 666.28
Ridge Regression | 0.925 | 1092.79
Stochastic Gradient Descent | 0.924 | 1098.35
Elastic Net | 0.923 | 1104.25
Lasso Regression | 0.90 | 1218.24




#### Running the project:

* To run this project use Jupyter Notebook or Google Colab.

## Files in this repository

1. The **diamonds.ipynb** file contains all the codes, plots and relevant descriptions of conducted analysis.

## The dataset origin

The dataset can be found at Kaggle (https://www.kaggle.com/shivam2503/diamonds) and contains data about diamond specifications of **56000 diamonds** which have been widely used for analysis.

## Relevant information

The dataset consists of the following features:

- **price** - given in US dollars ($326--$18,823);
- **carat** - weight of the diamond (0.2--5.01);
- **cut** - quality of the cut (Fair, Good, Very Good, Premium, Ideal);
- **color** - diamond colour, from J (worst) to D (best);
- **clarity** - a measurement of how clear the diamond is (I1 (worst), SI2, SI1, VS2, VS1, VVS2, VVS1, IF (best));
- **x** - length in mm (0--10.74);
- **y** - width in mm (0--58.9);
- **z** - depth in mm (0--31.8);
- **depth** - total depth percentage = z / mean(x, y) = 2 * z / (x + y) (43--79);
- **table** - width of top of diamond relative to widest point (43--95).


