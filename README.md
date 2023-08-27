# Bike-Sharing-Linear-Regression

This assignment is for building a multiple linear regression model for the prediction of demand for shared bikes.

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)


## General Information
- A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.
- A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state. 
- In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.
They have contracted a consulting company to understand the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market. The company wants to know:
Which variables are significant in predicting the demand for shared bikes.
How well those variables describe the bike demand
- Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the American market based on some factors.
- Business Goal:
You are required to model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market.

## Dataset and Data Dictionary
- day.csv (dataset)
- Readme.txt (data dictionary)

## Conclusions
We used Recursive Feature Elimination for selecting the variables :
Then we removed based on below criteria.
High p-value and high VIF - remove the variable
High p-value and low VIF - remove next
Low p-value and high VIF - remove after the 1st 2 steps
Low p-value and low VIF - Keep the variables
After following the above steps of elimination our model gave us an R-Square value of 85 percent.
Variables Significance
cnt = 0.2889 + (0.2272)yr + (0.0510)workingday + (-0.1162)windspeed +(-0.1082)spring+(0.0612)winter+(-0.0443)Dec+(-0.0456)Jan+(0.0670)Saturday+(-0.1825)Light Rain/Thunderstorm+(-0.1683)hum+(0.4272)temp+(0.0542)Sep+(0.0664)Saturday
considering variables 'temp','hum','windspeed' and 'cnt' are normalized using min-max scaler b/w the values 0-1.
Statistically significant and important predictor variables are as follows:
1 yr
2 workingday
3 temp
4 hum
5 windspeed
6 spring
7 winter
8 Dec
9 Jan
10 Sep
11 Saturday
12 Light Rain/Thunderstorm

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->






## Contact
Created by mahalakshmibhatk@gmail.com - feel free to contact me!

