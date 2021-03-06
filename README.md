# Rossmann Sales Prediction

Sales projection for a retail chain to predict the total amount of sales for the next 6 weeks.

<img src="https://github.com/kaotcs/rossmann_sales_prediction/blob/main/img/rossmann_.jpg" alt="Rossmann Store"
	title="Rossmann"  width="100%" height="500" />

## 01 BUSINESS PROBLEM
Rossmann operates over 3,000 drug stores in 7 European countries. Currently, Rossmann store managers are tasked with predicting their daily sales for up to six weeks in advance. Store sales are influenced by many factors, including promotions, competition, school and state holidays, seasonality, and locality. With thousands of individual managers predicting sales based on their unique circumstances, the accuracy of results can be quite varied.

The main goal for this project is to predict with a level of certainty the projections of sales for the next 6 weeks, since the retail chain wish to annalyze how to improve the performance of stores by figuring out which one have a better performance or not. This project aims to indicate the health of retail chain and its future.

## 02 BUSINESS ASSUMPTIONS
<ul>
<li>Stores marked as opened and with no results were removed from the analyzes.</li>
<li>Most of stores are closed on Sundays, reducing the total amount of sales during the week. For this project, it was kept all open and unopen stores to indicates this nuance for training the algorithm. </li>
<li>One semester of 180 stores are missing on records of sales. This inconsistency was kept since there were records of previous year.</li>
</ul>

## 03 SOLUTION STRATEGY
The strategy adopted was the following:

<b>Step 01.</b> Data Description: Searching for missing values, checking data types and preliminary statistical description.

<b>Step 02.</b> Feature Engineering: Looked for elaborate the hypotheses mindmap to understand how this bussiness work and derivate some new features the dig into the problem.

<b>Step 03.</b> Data Filtering: Data with no information or containing inputs which does not match to the scope of the project were removed.

<b>Step 04.</b> Exploratory Data Analysis: This crucial steps aims to answer the main questions indicated on hypotheses map, by analyzing the data on univariate, bivariate and multivariate analysis. The main insights are summarized by the end of that step.

<b>Step 05.</b> Data Preparation: Transforming the data for inputing to machine learning model. Most of jobs were rescaling and transforming the features values.

<b>Step 06.</b> Feature selection: Verifying which feature is important to input to the machine learning model. Some algorithms were used to assess the best ones.

<b>Step 07.</b> Machine learning modelling: Training and predicting results with machine algorithms. Cross-validation were used to assess the best performance model.

<b>Step 08.</b> Model-to-business: Convert the results for business managers.

<b>Step 09.</b> Deploy Model to Production: Deploying the model to be reachable to all retail chain managers.

## 04 TOP 3 DATA INSIGHTS

* The mean sales by day of extended assortment is higher than the others assortment types. In the other hand, 'basic' assortment have 15% more stores and it doesn't show a better performance.

* Stores sells are higher with closest competitors. It may indicates there is no direct competitors fighting for the same customers in the same area.

* Stores with extended promo (promo2) does not have a better performance comparing with regular promo.

## 05 MACHINE LEARNING MODEL APPLIED

The following machine learning algorithms were used to predict sales:

* Linear Regression;
* Regularized Linear Regression - Lasso;
* Random Forest Regressor;
* XGBoost Regressor.

Every model were cross-validated and its performance were compared against a model using the mean sales by stores.

## 06 MACHINE LEARNING MODEL PERFORMANCE

The result of running the machine learning algorithms as showed bellow. Since the RMSE standard deviation is lower for XGBoost Regressor, it was used for fine tunning of the model. Random Forest Regressor performed better, but this models has a higher computer performance cost and the result was close to XGBoost.

<img src="https://raw.githubusercontent.com/kaotcs/rossmann_sales_prediction/main/img/ml_performance.jpg" alt="ML peformance"
	title="Rossmann"/>

## 07 CONCLUSIONS
Deploying this model to production, the managers will be informed with an accurated prediction of sales in 6 weeks window. The projection of sales is important to assess the real performance of each stores and predict the next steps for retail chain.

## 08 LESSONS LEARNED
For this initial cicle of exploring the data with machine learning, XGBoost can perform better than the average model by 11%. Since the retail chain didn??t have previous method to predict sells, this model can help the managers to assess the performance of each stores and make decisions about the future by expanding or closing stores.

## 09 NEXT STEPS AND IMPROVEMENTS
By analyzing the residuals of the final model, it is important to indicate the model have room for improvement. For this initial aprouch, it was used several features that could be worked together by using correspondence analysis since there are many categorical features or making a clustering analyzis. This two methods can be used for the next cicle of the CRISP in this project.
