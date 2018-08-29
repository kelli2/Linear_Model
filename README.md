# Linear Model of Housing Prices

Analysis was done in R and the complete html readout of the rmd file can be viewed here: 

## https://kelli2.github.io/LinearRegressionModel_KelliDv5.html

In this analysis project, I developed a linear regression model to predict housing prices from the Ames data set. An exploratory data analysis identified variables that are associated with price and described the effects of log transformations on variable distributions and correlation with price. Models were selected with AIC, BIC, and Bayesian model selection and evaluated with residual plots and RMSE values for train and test sets. A simple model consisting of only 6 variables resulted in strong price predictions and had an AdjR2 of over 0.84. After analysis of anomalies in home prices from non-normal sales, the model performance was improved by modeling normal sales only. A larger model with 17 explanatory variables had an AdjR2 of over 0.92 with improved RMSE scores and the model exhibited slightly less than true coverage probability (0.947 vs 0.950).

Contents: <br/>

Part 1. EDA <br/>
1.1 The Ames dataset contains few missing values <br/>
1.2 The price distribution is more normally distributed with log transformation <br/>
1.3 Area metrics are more normally distributed with log transformation <br/>
1.4 Area and Price exhibit the best correlation when log tranformed<br/>
1.5 Year.Sold is associated with modest differences in price<br/>
1.6 Quality, but not Condition, is strongly associated with house price<br/>
1.7 Location is associated with price and quality differences<br/>
1.8 Correlation matrix identifies additional numerical variables associated with price<br/>

Part 2. Initial Model <br/>
2.1 Simple linear regression model with 6 explanatory variables<br/>
2.2 Model selection and feature analysis with BIC, AIC, and BMA produce similar models<br/>
2.3 Residual Plots of AIC Selected Model and Identification of Outliers<br/>
2.4 Relative Model Performance w/ RMSE: AIC selected model performs best<br/>
2.5 Analysis of Sale.Condition: Modeling normal sales only improves overall model<br/>

Part 3. Final Model <br/>
3.1 Feature Engineering and Linear Regression Model with 21 Explanatory Variables<br/>
3.2 BIC and AIC selection methods produce different models<br/>
3.3 Residual Plots of AIC Selected Model<br/>
3.4 Relative Model Performance w/ RMSE: AIC selected model again performs best<br/>
3.5 Based on coverage probability, the model correctly reflects uncertainty<br/>
3.6 Conclusions<br/>
