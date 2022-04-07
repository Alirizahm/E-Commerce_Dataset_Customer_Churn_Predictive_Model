# E-Commerce Dataset Customer Churn Predictive Model
Author's : Aliriza Hamonangan Matondang
## Purpose
- To predict the datasets by using machine learning models
- To understand important features in order to be able to be evaluated for reducing churn value
## Data Information
The data consists of 5630 rows and 20 features

- CustomerID : Unique customer ID
- Churn : Churn Flag
- Tenure : Tenure of customer in organization
- PreferredLoginDevice : Preferred login device of customer
- CityTier : City tier
- WarehouseToHome : Distance in between warehouse to home of customer
- PreferredPaymentMode : Preferred payment method of customer
- Gender : Gender of customer
- HourSpendOnApp : Number of hours spend on mobile application or website
- NumberOfDeviceRegistered : Total number of deceives is registered on particular customer
- PreferedOrderCat : Preferred order category of customer in last month
- SatisfactionScore : Satisfactory score of customer on service
- MaritalStatus : Marital status of customer
- NumberOfAddress : Total number of added on particular customer
- Complain : Any complaint has been raised in last month
- OrderAmountHikeFromlastYear : ercentage increases in order from last year
- CouponUsed : Total number of coupon has been used in last month
- OrderCount : Total number of orders has been places in last month
- DaySinceLastOrder : Day Since last order by customer
- CashbackAmount : Average cashback in last month

## Steps
- Data Cleaning (fill the NA with median)
- Change some features data types & drop features
- Feature Engineering
- One Hot Encoding
- Remove Outliers
- Features Selection
- Oversampling using SMOTE
- Checking the overfitting and underfitting
- Standardization 
- Modeling & Evaluation
- Feature Importance

## The Results
1. Model Conclusion

- The best model produced is the XGBoost with an accuracy of 97%
- The right model to use is the XGBoost
- When viewed from each evaluation carried out both from the test and train data, there is no significant difference
- So, the model is appropriate and not overfitting

2. Feature Importance based on the best model

Feature Importance by XGBoost

![download (4)](https://user-images.githubusercontent.com/92624520/162217983-d191afad-80a8-4073-9c67-8ca04819adff.png)


Findings :

- The features Importance use XGBoost plot importance and the features Importance of the best model can be used as a reference to reduce churn
- It should be noted that the best model obtained and the feature importance obtained can serve as a reference for evaluation in order to reduce the churn value
- The Number of Address feature or the total number of registered houses have an average value of users who churn higher than compared to customers who continue to use the app with an average value of 3-6
- This indicates that customers have many different home addresses and it appears that users who churn have a higher warehouse-to-home value compared to users who continue to use the app with an average value of 12-22
- The Warehouse To Home feature has a dominant value and is a very important feature of this model
- The distance from the warehouse to the house that is far away affects user churn so that an evaluation can be carried out related to shipping costs with that distance
- Based on the previous EDA, users who churn have an average score of 2-6 which indicates that new users churn very quickly
- Customers who Churn also often complain when compared to the previous EDA, users who churn and complain are far more than users who churn but do not complain
- The amount of cashback and the average cashback per order of churn users also tend to be lower than customer churn

Feature Importance by Shapley Value

![download (5)](https://user-images.githubusercontent.com/92624520/162218098-a1b1c79b-0f59-42a1-831b-1768a6ed3596.png)


Findings :

- Based on checking using the best feature importance model with shape, it can also be used as a reference to reduce churn
- There needs to be improvements in terms of service or good customer service, even though users complain but handling can be fast so that customers feel comfortable
- Tenure can also be a focus especially on new users, good promos with high or frequent cashbacks can make users stay and create habit patterns in users
- Improvements to product categories can be made to grocery, others, as well as laptops and accessories
- City tier 2 and 3 can be targetsmarket due to customers in City tier 2 and 3 is relatively small so it can reduce the value ofchurn on City tier 2 and 3

Notes :

- Red indicates high feature value (churn)
- Blue indicates low feature value (no churn)

## Conclusion
- The best model that can be used is the Random Forest Classifier with a prediction accuracy of 97%
- There needs to be improvements according to the importance of features based on the best model in order to reduce the churn value
- The model can be used as a reference and prediction to determine the development of churn after improvement

## Recommendation
- The e-commerece needs to create promotion at new users, because customers churn very quickly in tenure
- For long-standing customers,if that is certainly a concernbefore, so it's better for old customersgiven a program that makes customers comfortable or feel appreciated (exp: platinum service loyalty)
- There are need to be an improvement in the distance of the delivery of goods so that the delivery of goods become easier and cheaper, such as making a delivery checkpoint
