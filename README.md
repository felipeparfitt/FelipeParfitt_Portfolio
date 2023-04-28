# Felipe Parfitt Portfolio
Data Science portfolio

<style>body {text-align: justify}</style>

## [Project 1: Clustering Countries with Unsupervised Learning for HELP International](https://github.com/felipeparfitt/FelipeParfitt_Portfolio/blob/main/Data%20projects/CountryData_Clustering/clustering-country-data-kaggle.ipynb)

- This is a kaggle dataset for clustering the Countries by using Unsupervised Learning for HELP International.
- The quality of the features was improved using normalization techniques. 
- K-means model and PCA were applyed to data solve the problem.
- By dividing the data into three clusters, it is possible to identify three groups of countries: those in green with good indices that do not require assistance (North America, Western Europe, and some parts of Oceania); those in yellow with moderate indices that may require assistance (South America, most of Asia, North and South Africa); and those in red with low indices that require assistance (Central Africa and some countries in the Middle East).

<img src="./Data%20projects/CountryData_Clustering/color_map.jpg" alt="drawing" width="650"/>

## [Project 2: House Prices - Advanced Regression Techniques](https://github.com/felipeparfitt/FelipeParfitt_Portfolio/blob/main/Data%20projects/House%20project/house-price-kaggle.ipynb)

- This is a Kaggle competition to estimate house prices using supervised learning.
- NaN values in the features were filled with the mode, median, or another suitable categorical value such as 'None'. Categorical features were converted into dummy variables, taking into account the dependent variable SalePrice. One-hot encoding was applied.
- All features with non-Gaussian distributions were transformed using the boxcox1p transformation.
- An ensemble of models was used to estimate house prices, including linear regression models such as Lasso and Ridge, decision tree models such as GradientBoostingRegressor and XGBRegressor, and also the StackingCVRegressor.

<img src="./Data%20projects/House%20project/SalePrice_var.png" alt="drawing" width="650"/>
