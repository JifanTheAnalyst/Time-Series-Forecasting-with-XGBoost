# Time-Series-Forecasting-with-XGBoost

# Business Background and Objectives

Product demand forecasting has always been critical to decide how much inventory to buy, especially for brick-and-mortar grocery stores. More accurate forecasting with machine learning could prevent overstock of perishable goods or stockout of popular items.

This study aims for forecasting store sales for Corporación Favorita, a large Ecuadorian-based grocery retailer.

# Data Source and Understanding

## Data Source

https://www.kaggle.com/competitions/store-sales-time-series-forecasting/data

## Data Understanding

**store data:**
- store_nbr: the store at which the products are sold
- family: the type of product sold
- sales: the total sales for a product family at a particular store at a given date
- onpromotion: the total number of items in a product family that were being promoted at a store at a given date.
- cluster: a grouping of similar stores

**holiday data:**
- type: holiday type
- locale: scope of the holiday

**macro indicator:**
- oil price: Ecuador is an oil-dependent country and it's economical health is highly vulnerable to shocks in oil prices.

# Framework and Method

1. Data merging and cleaning (filling in missing values)
2. Data visualisation
3. Feature engineering (transforming categorical features)
4. Modelling and prediction
- Multivariate Time Series model
- XGBoost algorithm

# Result

- The Normalised Root Mean Square Error (RMSE)for XGBoost is 0.005 which indicate that the simulated and observed data are close to each other showing a better accuracy.
- Sales are predicted for test dataset (outof-sample)


![newplot](https://user-images.githubusercontent.com/93923656/164966254-a8135f17-d688-4a5b-9873-910fda85aa04.png)

![newplot-2](https://user-images.githubusercontent.com/93923656/164966289-d17f61a1-1d1e-4a06-a717-65523d2d579c.png)

Most sales are made on Sunday:

![day of week](https://user-images.githubusercontent.com/93923656/164966316-a8a34f63-02f2-4119-b471-00bf2bc64197.png)

Most sales are made in quarter 2:

![quarter](https://user-images.githubusercontent.com/93923656/164966353-1afd0f8d-5b8f-424a-9a0b-94105a323f37.png)

**Refrence:**
Big thanks to Kashish Rastogi: for the data visualisation dashboard.
