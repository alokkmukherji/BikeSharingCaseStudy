# Bike Sharing Business Case Study 

US bike-sharing provider BoomBikes has observed dip in revenue due to Covid-19. So, the company wants to understand the demand for shared bikes among the people after ongoing quarantine situation ends across the nation due to Covid-19 so that they can regain the market. So, they contacted a consulting company to understand the factors on which the demand for these shared bikes depends. Specifically the company wants to know which variables are significant in predicting the demand for shared bikes and how well those variables describe the bike demands so that they apply the same knowledge in their business strategy:

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

## General Information
- The main objective of this analysis is to create a linear regression model to understand which independent variables/attributes (predictor) are mostly impacting outcome variable "cnt" (count of total rental bikes)
- Steps followed for this analysis: 
  1. Reading and cleaning the Data
     - Input dataset used for this analysis had 730 rows and 16 columns
     - The data cleaning step included
        1. Rounding up digit after decimal  by 3 
        2. Converting integer values to corresponding categorical values 
        3. Checking columns have same values or not
        4. Remove columns which are not required for analysis
  2. Visualising the data - 
     -  Created different plots to understand the relationship (specifically to understand linear relationship) between different sets of variables 
  3. Data preparation for Modeling
        1. Converting categorical variables to dummy variables - so that they become suitable for model building 
        2. Splitting data into Training and Test sets at 70% (for training data) and 30% (for evaluating data) ratio respectively
        3. Rescaling features so that variables can have comparable scale using Min-Max scaling technique
  4. Building a linear model
      - Linear model was build using statsmodels 
      - Started with 10 variables using sklearn RFE technique and dropped unnecessary variables having high VIF (>5), high p (>0.05) one by one after checking p and VIF everytime.
      - Dropped variables having very low magnitude one by one after checking p, VIF and Adjusted R2
      - FInal model having 81% as R2 and 1.999 as Durbin-Watson
  5. Resudual analysis of the training data
      - Applied model validated on training dataset
      - Residual analysis done to validate residuals are normally distributed with mean at 0
      - Checked y_predict vs y based on the training database to validate linear distribution (homoscedasticity) between the two 
  6. Making prediction using final model
      - Final model applied on test dataset
  7. Model evaluation
      - Model is evaluated based on test data using sklearn r2_score which gave R2 value which is within 5% of R2 generated based on training dataset
      - Checked y_predict vs y based on the test database to validate linear distribution (homoscedasticity) between the two
      - Did residual analysis on test dataset to validate residuals are normally distributed with mean at 0
  8. Summary
      - Created final linear regression equation 


   
 

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
 -  Increase in temp causes an increase in bike rent when all other predictors are not changing
 -  Bike rent increases with increase in year when all other predictors are not changing
-   Increase in Light Snow/Light Rain + Thunderstorm + Scattered clouds/Light Rain + Scattered clouds causes a decrease in bike rent when all other predictors are not changing
-   Increase in windspeed causes a decrease in bike rent when all other predictors not not changing
-   During spring, there is a decrease in bike rent when all other predictor is not changing
-   During Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, there is a decrease in bike rent when all other predictor is not changing

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- Python 3.0 (Python lib used - numpy, pandas, seaborn, matplotlib, sklearn, statsmodels)
- Jupyter notebook
- Exploratory Data Anlysis (EDA) Concept
- Linear regression (single and multiple) Concept
- Inferential Statistics Concept

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements

- IIIT Bangalore
- Upgrad 


## Contact
Created by alokkmukherji@gmail.com 


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
