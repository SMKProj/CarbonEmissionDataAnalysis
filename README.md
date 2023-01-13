# CarbonEmissionDataAnalysis
 Comparison of Linear Regression, Decision Trees and Support Vector Machines in Predicting Carbon Emission 

Abstract— The deteriorating climatic conditions over the time has alarmed the world forums to take the problem seriously and to focus on development and revision of projects that are more environment friendly and sustainable. The ever-expanding industrialization has caused smog formation over the cities and great emission of carbon dioxide from usage of greenhouse gases. It is an hour of need to identify the factors that contribute to release of smog and CO2 to reduce the adverse effects caused by economic development. With the emergence of idea of making transportation systems smart, it is important to understand and be aware of the factors which are contributing to vehicles emissions to cope up with rapidly increasing threat to the environment thus predicting effects of greenhouse gases and particularly CO2 is also very important. This study presents a comparative analysis of machine learning models in predicting carbon emission by analyzing dataset collected from Kaggle. The research findings confirm machine learning efficacy in predicting carbon emission, which can be prove useful in improving the adverse effects of transportation sector on climatic conditions.

The industrialization and economic development have entirely transformed our ways of living. It has made human life easy in so many ways however, we are paying great price for the comfort which it offers in terms of damage that it caused to the environment. According to fifth assessment report of intergovernmental panel on climate change (IPCC) in last one hundred years, the world temperature has soared by 0.89 degree centigrade and in last 50 years over 90% of global warming is due to rapid usage of greenhouse gases from fuels used and burned. The discharge from greenhouse gases remains in atmosphere for over one hundred years and layers around the world like a blanket that entrapped energies causing rise in atmosphere temperature. CO2 accounts to 80% of total greenhouse gases emitted by different human activities. Every year carbon dioxide emissions are increasing causing rapid increase in global surface temperature as well as increase in sea levels.

Many environmental challenges are introduced due to massive transportation caused by urbanization. According to Environmental Protection Agency (EPA), transportation comes first in a survey of economic sectors contributing higher greenhouse gas emissions with 29% of greenhouse gas emissions in US in year 2019 and 25% of emissions are only related to CO2. In Europe also transportation is causing one fourth of greenhouse gas emissions and with count more than 70%. Road transport is considered the biggest emitter of greenhouse gases in year 2014 in Europe. As per European commission, light commercial vehicles and passenger cars contribute to 2.5% and 12% of CO2 emissions in EU. In Jan 2020, new performance standard regulations were passed by European commission for CO2 emission for new passenger cars and light commercial vehicles which has caused reduction in CO2 emission by 12%.

For any country’s economic and social development, transportation is an indispensable industry and is commonly used as a tool for measuring development. Often transportation systems are associated with greater development. However, these highly functional and ever-expanding transportation systems are a great threat to world’s climatic conditions and if the global surface temperature keeps on increasing it will lead to more natural catastrophes and cause significant risk and damage to survival and development of humanity.

To mitigate the adverse effects of greenhouse gas emission particularly CO2  it is essential to understand what factors are contributing to higher CO2. The study is an effort to exploit machine learning algorithms to predict carbon emission caused by vehicles.

Data: The data for the proposed research is collected from Kaggle which constitutes data related to fuel consumption and CO2 emission for year 2022 for new light duty vehicles for retail sale in Canada. The dataset constitutes of nearly 1000 records and 12 columns namely Model Year, Make, Model, Vehicle Class, Engine Size, Cylinders, Transmission, Fuel Type, Fuel Consumption (City (L/100 Km)), Fuel Consumption (Highway (L/100 km)), Fuel Consumption Combine (L/100 Km), Fuel Consumption Combine (mpg), CO2 emission (g/km), CO2 ratings and Smog Ratings. The CO2 and Smog ratings are scaled from 1(worst) to 10 (best). Fuel consumption for city and highway individually are shown in liters per 100 km and combined ratings are given in liters per 100 km and miles per imperial gallon (mpg). CO2 emissions gives the tailpipe emission of carbon dioxide for both city and highway driving. CO2 ratings and Smog ratings gives a scale from 1-10 for CO2 emission and smog forming pollutants.

Tools and Libraries: The proposed research is developed in Python programming language and the used python libraries for data analysis are: scikit-learn, pandas, numpy, matplotlib, and dython.

Machine Learning Models: The proposed study comes under supervised machine learning where we made the model learn from labelled training data to help predict results for unseen test data. The machine models that are developed for predicting carbon emission are linear regression, decision tree, and support vector classifier (SVC).

Data Sampling and Descriptive Statistics: In given dataset we have five categorical variables namely Make, Model, Vehicle Class, Transmission and Fuel while rest of the variables are numeric. For analysis we are going to drop Year variable from the given dataset which only holds single value i.e., 2022.
For convenience purpose, the column names of given dataset are renamed to Make, Model, Vehicle, Engine, Cylinders, Transmission, Fuel, FC_City, FC_Hwy, FC_Comb_L, FC_COMB_Mpg, Emission, CO2 and Smog. Figure below shows the first five records of given dataset.

![image](https://user-images.githubusercontent.com/85155952/212294997-8fc9c3d8-94cf-4623-979a-a4db90ede606.png)

The descriptive information of the given dataset is given in Table below. The correlation between variables is shown as a heat map is a figure below.

![image](https://user-images.githubusercontent.com/85155952/212295377-099b2344-431d-4f7a-9a45-18d2a4fa93e5.png)

![image](https://user-images.githubusercontent.com/85155952/212301928-5b48423d-a61a-403b-ae6c-28ff0076f0ae.png)

Data Preperation: For the analysis, rightnow only numerical values are considered whcih showed positive and negative correlation with the response variable i.e. emission. This step involves creation of training and test data using Python sklearn. For the purpose 70% data is used for training and 30% is set for testing purpose.

Data Representation: Below figure plots original data without any preprocessing to gives a better idea or understanding of relationship between response and predictor variables for our analysis.
![VisualRepresentationofData](https://user-images.githubusercontent.com/85155952/212297196-7b462933-8089-4db0-829c-3f7bbc792a74.png)

Predicting Emission: Below are the figure that plots actual test values for response variable (emission) and predicted values using linear regression, decision trees and support vector classifer

![LinearRegressionDataModeling](https://user-images.githubusercontent.com/85155952/212299445-0b37473b-6178-43c4-89d1-64eee86ec283.png)

MSE:  106.78343778516974, 
R squared score: 0.97

![DecisionTreesDataModeling](https://user-images.githubusercontent.com/85155952/212300082-58dae5e6-0588-470a-8276-40ae4373f7df.png)

MSE:  144.42957746478874, 
R squared score: 0.96

![SVMDataModeling](https://user-images.githubusercontent.com/85155952/212300023-1177f860-ff0f-43cc-917c-b5aaa6409b81.png)

RMSE:  163.90140845070422, 
R squared score: 0.95

Conclusion: The main purpose of this study is to investigate how the machine learning can be utilized to lessen the adverse effects of greenhouse gases emission caused by transportation sector. The developed model’s performance for predicting carbon dioxide emission ratings confirms machine learning utility which is very advantageous for limiting the worsening climatic conditions.





