# House-Sale-Price-Penalized-Regression-XGBRegressor

***Name:*** Ziyad Maknojia

***Contact Information:*** zam@gwu.edu

***Kaggle Name:*** Ziyad

***Kaggle Leaderboard Score:*** 0.125

***Kaggle Rank:*** 681

### Basic Information

* **Model date**: May, 2021
* **Model version**: 1.0
* **License**: MIT
* **Model implementation code**: [penalized-regression-and-xgbregressor.ipynb](penalized-regression-and-xgbregressor.ipynb)

### Intended Use
* **Primary intended uses:** This model is to predict the Boston Housing Prices
* **Primary intended users:** This model can be used by students, professors
* **Model Applications:** This model can be used to conduct Elastic Net regression analysis on any similar data with high number of predictors

### Training Data
* **Source of training and test data:** https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data
* **How training data was divided into training and validation data: 50% training, 50% test**
* **Data Dictionary:** https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data
* **Number of rows in training and validation data:**
  * Training rows: 1,460
  * Validation rows: 1,460

### Model Details
* ***Columns used in model as inputs:*** BedroomAbvGr,GarageType,FireplaceQu,Fireplaces,Functional,TotRmsAbvGrd,KitchenQual,KitchenAbvGr,HalfBath         
GarageFinish,FullBath,BsmtHalfBath,BsmtFullBath,GrLivArea,LowQualFinSF,2ndFlrSF,1stFlrSF,GarageYrBlt,GarageCars,CentralAir,PoolArea,SaleType,        
YrSold,MoSold,MiscVal,MiscFeature,Fence,PoolQC,ScreenPorch,GarageArea,3SsnPorch,EnclosedPorch,OpenPorchSF,WoodDeckSF,PavedDrive,GarageCond      
GarageQual,Electrical,HeatingQC,MSSubClass,LandSlope,OverallCond,OverallQual,HouseStyle,BldgType,Condition2,Condition1,Neighborhood,LotConfig,YearRemodAdd
LandContour,LotShape,Alley,Street,LotArea,LotFrontage,MSZoning,YearBuilt,RoofStyle,Heating,BsmtCond,TotalBsmtSF,BsmtUnfSF,BsmtFinSF2,BsmtFinType2     
BsmtFinSF1,BsmtFinType1,BsmtExposure,BsmtQual,RoofMatl,Foundation,ExterCond,ExterQual,MasVnrArea,MasVnrType,Exterior2nd,Exterior1st,SaleCondition 
* **Column(s) used as target(s) in the final model:*** SalePrice
* **Type of model:*** Elastic Net with RMSE = 0.125
* **Software used to implement the model:** Python
* **Version of the modeling software**: 3.7.12
* **Hyperparameters or other settings of the model**: n_folds = 5, alpha = 0.0005, l1_ratio = 0.5

### Abbreviations
* **RMSE:** Root Mean Squared Error

### Quantitative analysis:
* **Metrics used to evaluate the final model**:
* **Root Mean Squared Error(RMSE)**
* **Training Data**
* RMSE = 0.11
* **Validation Data**
* RMSE = 0.125

### Graphs 
* **Distplot:** The plot provides the distribution of the target variable 
* **Probability Plot:** The plot provides information whether the target variable follows normal distribution
* **Regression Plot:** The plot highlightes the relationship between target varibale and one of the prominent independent variable i.e. Living Area
* **Box Plot:** The box plot gives the Sale prices of the houses over the years as well as with respect to different Neighborhood
* **Correlation HeatMap:** The correaltion heatmap gives the correlation between all the numerical features, we are interested correlation between dependent
variable and independent variables 
* **Bar Graph:** The bar graph provides the missing data percentage for the top 20 independent variables

### Ethical considerations:
* **Math issues**:*** Few input columns have been transformed based on their contribution to the model and the categorical variables are subjected to Label Encoding. Hence, interpretation can be a hard. Also, the concept of red-lining can cause bias with respect to Neighborhood
* **Real World Risks**:
* If this model is used to make business decisions, it might not be accurate due to the variable importance measure and can severly impact the outcome



