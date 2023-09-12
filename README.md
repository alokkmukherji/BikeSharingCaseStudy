# Bike Sharing Case Study 

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
  3. Visualising the data - univariate, bivariate analysis
  4. Data preparation for Modeling
  5. Splitting data into Training and Test sets
  6. Rescaling features
  7. Building a linear model
  8. Resudual analysis of the training data
  9. Making prediction using final model
  10. Model evaluation
 10. Summary

 - The no. of rows and columns reduced to 37398 and 21 respectively, This reduced dataset was used for further analysis
   
 

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
-  After univariate, segmented univariate and bivariate analysis, the list of drivers for loan default mentioned below were identified: 
  1. Interest rate - Higher the interest rate, the chance of loan default is more
  2. Anual income  - Lower the income, the chance of loan default is more
  3. Loan grade    - Chance of loan default is more for loan grade F
  4. Loan sub grade - Chance of loan default is more for loan sub grade F5
  5. Loan term      - Higher chance of loan default for loan term 60
  6. Purpose of loan - Higher chance of loan default if loan is taken for small business
  7. Loan amount      - Higher chance of loan default if loan amount is high
  8. No. of installment - Higher chance of loan default if no. of installment is more 
  9. The length of employment - Higher chance of loan default is for fresher

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- Python 3.0 (Python lib used - numpy, pandas, seaborn, matplotlib)
- Jupyter notebook
- Exploratory Data Anlysis (EDA) Concept

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements

- IIIT Bangalore
- Upgrad 


## Contact
Created by alokkmukherji@gmail.com / akshaykachroo2050@gmail.com


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
