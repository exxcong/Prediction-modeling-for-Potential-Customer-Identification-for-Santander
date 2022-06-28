# Prediction-modeling-for-Potential-Customer-Identification-for-Santander

## Video Presentation
https://www.youtube.com/watch?v=EL_jXirPkFk


## Background and Problem Statement
Santander is a Spanish multinational corporation bank and financial-based company operating in Europe, Asia, and North and South America. Santander continually helps its customers understand their financial health, and discern products and services helpful for achieving their monetary goals. In this scenario, they want to identify customers who will make a transaction in the future, irrespective of the amount of money transacted.
This project is aimed to help Santander build prediction models to identify potential customers.

## Data Acquisition
https://www.kaggle.com/competitions/santander-customer-transaction-prediction/data

## Method Used
Generally, we used 5 techniques: boosting, neural network, stacking, ensemble 200 models and ensemble 200 stacking models. Ensemble 200 stacking models worked best with an AUC score of 0.91611 while CNN got the worst score with a long-running time. 

We built 200 models, and for each model, we only used two features -- one original feature and its unique or not flag feature. But within each model, instead of only using one boosting model, we used stacking to ensemble different boosting models which gave us pretty good results before. After trying several combinations, we got our best model by stacking CatBoost, XGBoost, and LightGBM and the best score on Kaggle is 0.91611.

## Business Implication
By implementing our model, Santander will be able to correctly rank a true purchasing customer ahead of a customer that will not actually purchase 91.4% of the time.
As a next business step, Santander can devise different strategies for different types of customers using our predictive model. For customers that are predicted to make a purchase, Santander does not need to offer discounts and give away margin on a product they know will be purchased anyway. Instead, they can focus on driving additional value on the transaction through upgrades or related products. On the other hand, for customers who are predicted not to make a purchase, Santander can focus on offering discounts or other incentives to boost customer retention and increase the probability of a purchase.
