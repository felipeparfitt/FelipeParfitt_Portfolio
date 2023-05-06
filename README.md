# Felipe Parfitt Portfolio
Data Science portfolio

<style>body {text-align: justify}</style>

## [Project 1: Clustering Countries with Unsupervised Learning for HELP International](https://github.com/felipeparfitt/FelipeParfitt_Portfolio/blob/main/Data%20projects/CountryData_Clustering/clustering-country-data-kaggle.ipynb)

- This is a kaggle dataset for clustering the countries by using Unsupervised Learning for HELP International.
- The quality of the features was improved using normalization techniques. 
- K-means model and PCA were applied to data in order to solve the problem.
- By dividing the data into three clusters, it is possible to identify three groups of countries: those in green with good indices that do not require assistance (North America, Western Europe, and some parts of Oceania); those in yellow with moderate indices that may require assistance (South America, most of Asia, North and South Africa); and those in red with low indices that require assistance (Central Africa and some countries in the Middle East).

<img src="./Data%20projects/CountryData_Clustering/color_map_att.jpg" alt="drawing" width="650"/>

And following a dashboard made in Power BI with different colors representing each cluster:

<img src="./Data%20projects/CountryData_Clustering/color_map_att.png" alt="drawing" width="650"/>

## [Project 2: Supervised Learning Classification of Spaceship Titanic Passengers](https://github.com/felipeparfitt/FelipeParfitt_Portfolio/blob/main/Data%20projects/SpaceshipTitanic%20project/spaceshiptitanic-kagglecompetition.ipynb)

- This Kaggle competition involves using supervised learning to predict which passengers were transported to an alternate dimension.
- Some features were created to fill NaNs by grouping passengers based on their close relationships. For example, passengers with the same cabin or last name are likely to exhibit similar behavior. Basically, categorical features were filled first by the mode of each group defined by the new column 'Group', then by the mode of each group defined by the new column 'LastName', and lastly by the mode of the entire column.
- NaN values in numerical features have been filled with the mode, which is basically zero, implying that the passenger has not spent anything.
- The prediction was made by a soft voting ensemble of models, using Logistic Regression, KNeighbors, Gradient Boosting, XGB, and StackingCV.

<img src="./Data%20projects/SpaceshipTitanic%20project/corr_image.png" alt="drawing" width="650"/>

## [Project 3: House Prices - Advanced Regression Techniques](https://github.com/felipeparfitt/FelipeParfitt_Portfolio/blob/main/Data%20projects/House%20project/house-price-kaggle.ipynb)

- This is a Kaggle competition to estimate house prices using supervised learning.
- NaN values in the features were filled with the mode, median, or another suitable categorical value such as 'None'. Categorical features were converted into dummy variables, taking into account the dependent variable SalePrice. One-hot encoding was applied.
- All features with non-Gaussian distributions were transformed using the boxcox1p transformation.
- An ensemble of models was used to estimate house prices, including linear regression models such as Lasso and Ridge, decision tree models such as GradientBoostingRegressor and XGBRegressor, and also the StackingCVRegressor.

<img src="./Data%20projects/House%20project/SalePrice_var.png" alt="drawing" width="650"/>
