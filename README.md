# Time-Series-Forecasting-using-Pycaret

This repository helps us in predicting daily sales of a particular product in a particular store.

## Source
 
 This is store sales challenge on kaggle.
 https://www.kaggle.com/c/store-sales-time-series-forecasting
 
 ## Goal
 
To forecast store sales on data from Corporación Favorita, a large Ecuadorian-based grocery retailer using time series forecasting.
Specifically, you'll build a model that more accurately predicts the unit sales for thousands of items sold at different Favorita stores. You'll practice your machine learning skills with an approachable training dataset of dates, store, and item information, promotions, and unit sales.
![image](https://user-images.githubusercontent.com/45202209/163094220-04a51df9-1cdc-4df8-948b-d0d9ddb08f59.png)

 
## Context
 
Forecasts aren’t just for meteorologists. Governments forecast economic growth. Scientists attempt to predict the future population. And businesses forecast product demand—a common task of professional data scientists. Forecasts are especially relevant to brick-and-mortar grocery stores, which must dance delicately with how much inventory to buy. Predict a little over, and grocers are stuck with overstocked, perishable goods. Guess a little under, and popular items quickly sell out, leading to lost revenue and upset customers. More accurate forecasting, thanks to machine learning, could help ensure retailers please customers by having just enough of the right products at the right time.

Current subjective forecasting methods for retail have little data to back them up and are unlikely to be automated. The problem becomes even more complex as retailers add new locations with unique needs, new products, ever-transitioning seasonal tastes, and unpredictable product marketing.


## Potential Impact

If successful, you'll have flexed some new skills in a real world example. For grocery stores, more accurate forecasting can decrease food waste related to overstocking and improve customer satisfaction. The results of this ongoing competition, over time, might even ensure your local store has exactly what you need the next time you shop.


## datasets

https://www.kaggle.com/competitions/store-sales-time-series-forecasting/data

### File Descriptions and Data Field Information
#### train.csv
The training data, comprising time series of features store_nbr, family, and onpromotion as well as the target sales.
- store_nbr identifies the store at which the products are sold.
- family identifies the type of product sold.
- sales gives the total sales for a product family at a particular store at a given date. Fractional values are possible since products can be sold in fractional units (1.5 kg of cheese, for instance, as opposed to 1 bag of chips).
- onpromotion gives the total number of items in a product family that were being promoted at a store at a given date.

#### test.csv
The test data, having the same features as the training data. You will predict the target sales for the dates in this file.
- The dates in the test data are for the 15 days after the last date in the training data.

#### stores.csv
Store metadata, including city, state, type, and cluster.
- cluster is a grouping of similar stores.

#### oil.csv
Daily oil price. Includes values during both the train and test data timeframes. (Ecuador is an oil-dependent country and it's economical health is highly vulnerable to shocks in oil prices.)

#### holidays_events.csv
-Holidays and Events, with metadata

- NOTE: Pay special attention to the transferred column. A holiday that is transferred officially falls on that calendar day, but was moved to another date by the government. A transferred day is more like a normal day than a holiday. To find the day that it was actually celebrated, look for the corresponding row where type is Transfer. For example, the holiday Independencia de Guayaquil was transferred from 2012-10-09 to 2012-10-12, which means it was celebrated on 2012-10-12. Days that are type Bridge are extra days that are added to a holiday (e.g., to extend the break across a long weekend). These are frequently made up by the type Work Day which is a day not normally scheduled for work (e.g., Saturday) that is meant to payback the Bridge.
- Additional holidays are days added a regular calendar holiday, for example, as typically happens around Christmas (making Christmas Eve a holiday).

#### Additional Notes
- Wages in the public sector are paid every two weeks on the 15 th and on the last day of the month. Supermarket sales could be affected by this.
- A magnitude 7.8 earthquake struck Ecuador on April 16, 2016. People rallied in relief efforts donating water and other first need products which greatly affected supermarket sales for several weeks after the earthquake.

All these datasets will help us building the ML model to capture trend, seasonality and cycles in the time series data.


## PyCaret
![image](https://user-images.githubusercontent.com/45202209/163095073-b6b2597c-28f1-4e8b-bf0a-68d1b4cf4569.png)
- I have used a new python library "PyCaret" to forecast sales of 3 products in store number 44. 
- This procedure can be extended to all the stores and products combination.


## Resources
- Find the PyCaret references in https://pycaret.gitbook.io/docs/
- Find PyCaret tutorials on youtube in https://www.youtube.com/channel/UCxA1YTYJ9BEeo50lxyI_B3g

## Licesnce

Copyright 2022 Ramya S

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.


## Credits
This project would have been impossible without "PyCaret" library, its references and tutorials.


