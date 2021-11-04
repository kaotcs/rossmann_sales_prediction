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

* Stores with closest competitors sells are higher. It may indicates there is no direct competitors fighting for the same customers in the same area.

* Stores with extended promo (promo2) does not have a better performance comparing with regular promo.

## 0 MACHINE LEARNING MODEL APPLIED

## 0 MACHINE LEARNING MODEL PERFORMANCE

## 0 CONCLUSIONS

## 0 LESSONS LEARNED

## 1 NEXT STEPS AND IMPROVEMENTS
