# Felipe Parfitt Portfolio
Data Science portfolio

<style>body {text-align: justify}</style>

## [Project 1: Disease Detection](https://github.com/felipeparfitt/FelipeParfitt_Portfolio/blob/e4d570ca440c79ce9812abfc6a7f3a1bae72a411/Data%20projects/Disease%20Detection%20Project/Disease%20Detection%20-%20ICR%20Competition.ipynb)

- An exploratory data analysis (EDA) was conducted to investigate all aspects of the data, including: (a) Data balance, (b) Descriptive statistics, (c) Identification of missing values, (d) Detection of outliers, (e) Identification of clusters, (f) Assessment of skewness, (g) Identification of trends, and (h) Analysis of correlations.
- The mean of the target class grouped by meanand  trend correlation were cheked in order to see to relationship with the target clas and also trend correlation bewtwen an train/test split sample;
- The data's skewness was addressed using the Yeo-Johnson method, utilizing the PowerTransformer. Additionally, an anomaly detection process was executed, and its results were incorporated into a new feature.
- Numerous feature selection techniques were experimented with, including Mutual Information (MI), Boruta, Minimum Redundancy Maximum Relevance (MRMR), and Recursive Feature Elimination (RFE). The RFE method, utilizing Shapley values as the criteria for feature elimination, was chosen to eliminate several noisy features from the dataset.
- A Nested Cross-validation scheme was implemented, consisting of four outer cross-validation folds and five inner cross-validation folds. Within the inner cross-validation, hyperparameter optimization was conducted using OPTUNA, while the models were tested on the outer cross-validation folds. As a result, four distinct models were obtained from this process.
- Four distinct models were trained using different subsets of the data, and subsequently combined through an ensemble approach to effectively address the issue of overfitting.

<img src="./Data%20projects/Disease%20Detection%20Project/Time%20by%20bins.png" alt="drawing" width="650"/>

## [Project 2: Credit Card Fraud Detection](https://github.com/felipeparfitt/FelipeParfitt_Portfolio/blob/2a52d143d19e7a6beacb957b02825cceadb15535/Data%20projects/Fraud%20Detection%20Project/Fraud%20Detection%20in%20Credit%20Card%20Dataset.ipynb)

- An exploratory data analysis was conducted to examine the skewness and correlation of the dataset.
- Average precision, recall, precision, and F1-score are all metrics used to evaluate the model's performance. Another metric that could be utilized is the F-beta score, which allows for giving slightly more weight to recall and reducing false negatives.
- To address the issue of imbalanced data, such as in the case of fraud detection, undersampling methods (Random Undersampling, Nearest Neighbors) and oversampling method (SMOTE) were employed to enhance the model's results.
- In relation to the original dataset, the train, validation, and test sets were split based on chronological order, with a gap of 5% of the data (using a prequential approach with a delay). This approach was adopted to ensure that the model always predicts future transactions using past data.
- To improve the hyperparameters of the models, optimization was performed using the Optuna library with the TPE optimizer. The metric used for optimization was the average precision, aiming to maximize it and select the best model configuration.
- After selecting the best model, the optimal threshold was chosen to maximize the F1-score metric, achieving a good and balanced trade-off between recall and precision.
- Shapley values were utilized to determine the importance of each feature in the model. These values allowed us to examine why the model correctly predicted instances (both true positives and true negatives) and which feature contributed to those predictions. Additionally, Shapley values provided insights into the reasons behind incorrect predictions (both false positives and false negatives) and the corresponding features responsible for those errors.
- What else could be done? The features with near-zero Shapley values should be either removed or combined with others.
 
<img src="./Data%20projects/Fraud%20Detection%20Project/Shapley%20values.png" alt="drawing" width="650"/>

## [Project 3: Clustering Countries with Unsupervised Learning for HELP International](https://github.com/felipeparfitt/FelipeParfitt_Portfolio/blob/main/Data%20projects/CountryData_Clustering/clustering-country-data-kaggle.ipynb)

- This is a kaggle dataset for clustering the countries by using Unsupervised Learning for HELP International.
- The quality of the features was improved using normalization techniques. 
- K-means model and PCA were applied to data in order to solve the problem.
- By dividing the data into three clusters, it is possible to identify three groups of countries: those in green with good indices that do not require assistance (North America, Western Europe, and some parts of Oceania); those in yellow with moderate indices that may require assistance (South America, most of Asia, North and South Africa); and those in red with low indices that require assistance (Central Africa and some countries in the Middle East).

<img src="./Data%20projects/CountryData_Clustering/color_map_att.png" alt="drawing" width="650"/>

And following a dashboard made in Power BI with different colors representing each cluster:

<img src="./Data%20projects/CountryData_Clustering/CountryCluster.png" alt="drawing" width="650"/>

## [Project 4: Supervised Learning Classification of Spaceship Titanic Passengers](https://github.com/felipeparfitt/FelipeParfitt_Portfolio/blob/main/Data%20projects/SpaceshipTitanic%20project/spaceshiptitanic-kagglecompetition.ipynb)

- This Kaggle competition involves using supervised learning to predict which passengers were transported to an alternate dimension.
- Some features were created to fill NaNs by grouping passengers based on their close relationships. For example, passengers with the same cabin or last name are likely to exhibit similar behavior. Basically, categorical features were filled first by the mode of each group defined by the new column 'Group', then by the mode of each group defined by the new column 'LastName', and lastly by the mode of the entire column.
- NaN values in numerical features have been filled with the mode, which is basically zero, implying that the passenger has not spent anything.
- The prediction was made by a soft voting ensemble of models, using Logistic Regression, KNeighbors, Gradient Boosting, XGB, and StackingCV.

<img src="./Data%20projects/SpaceshipTitanic%20project/corr_image.png" alt="drawing" width="650"/>

## [Project 5: House Prices - Advanced Regression Techniques](https://github.com/felipeparfitt/FelipeParfitt_Portfolio/blob/main/Data%20projects/House%20project/house-price-kaggle.ipynb)

- This is a Kaggle competition to estimate house prices using supervised learning.
- NaN values in the features were filled with the mode, median, or another suitable categorical value such as 'None'. Categorical features were converted into dummy variables, taking into account the dependent variable SalePrice. One-hot encoding was applied.
- All features with non-Gaussian distributions were transformed using the boxcox1p transformation.
- An ensemble of models was used to estimate house prices, including linear regression models such as Lasso and Ridge, decision tree models such as GradientBoostingRegressor and XGBRegressor, and also the StackingCVRegressor.

<img src="./Data%20projects/House%20project/SalePrice_var.png" alt="drawing" width="650"/>


## Project 6: Power BI Dashboards

### [Sales Dashboard Example](https://github.com/felipeparfitt/FelipeParfitt_Portfolio/blob/7af446acd4738d169c5af9c6b1367c29a1b6d039/Data%20projects/ContosoSales%20Project/MS%20data.png)

- The data has been imported into Power BI by SQL Server.

<img src="./Data%20projects/ContosoSales%20Project/MS%20DATA%20NOVO.png" alt="drawing" width="650"/>

### [Web Scraping With Python - Brasileirão 2022](https://github.com/felipeparfitt/FelipeParfitt_Portfolio/blob/739405704ea7dd4d41582503c49f1351e0881fcc/Data%20projects/Brasileirao%20Project/WebScraping_Brasileirao.ipynb)

- This is a project to extract game information data from the [cbf website](https://www.cbf.com.br/futebol-brasileiro/competicoes/campeonato-brasileiro-serie-a/2022) using the Requests and BeautifulSoup libraries in Python.

<img src="./Data%20projects/Brasileirao%20Project/Brasileir%C3%A3oS%C3%A9rie_A_2022_BI.png" alt="drawing" width="650"/>
