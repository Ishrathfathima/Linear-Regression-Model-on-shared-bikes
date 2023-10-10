# Linear Regression Model on bike sharing
> A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.


A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state. 


In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.


They have contracted a consulting company to understand the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market. The company wants to know:

Which variables are significant in predicting the demand for shared bikes.
How well those variables describe the bike demands
Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the American market based on some factors. 

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
  

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- Business Goal:
You are required to model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market. 


- Data Preparation:

You can observe in the dataset that some of the variables like 'weathersit' and 'season' have values as 1, 2, 3, 4 which have specific labels associated with them (as can be seen in the data dictionary). These numeric values associated with the labels may indicate that there is some order to them - which is actually not the case (Check the data dictionary and think why). So, it is advisable to convert such feature values into categorical string values before proceeding with model building. Please refer the data dictionary to get a better understanding of all the independent variables.
 
You might notice the column 'yr' with two values 0 and 1 indicating the years 2018 and 2019 respectively. At the first instinct, you might think it is a good idea to drop this column as it only has two values so it might not be a value-add to the model. But in reality, since these bike-sharing systems are slowly gaining popularity, the demand for these bikes is increasing every year proving that the column 'yr' might be a good variable for prediction. So think twice before dropping it. 
 

- Model Building

In the dataset provided, you will notice that there are three columns named 'casual', 'registered', and 'cnt'. The variable 'casual' indicates the number casual users who have made a rental. The variable 'registered' on the other hand shows the total number of registered users who have made a booking on a given day. Finally, the 'cnt' variable indicates the total number of bike rentals, including both casual and registered. The model should be built taking this 'cnt' as the target variable.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- Final Result Comparison
  rain R^2 :0.818
  rain Adjusted R^2 :0.815
  Test R^2 :0.801
  Test Adjusted R^2 :0.793
This seems to be a really good model that can very well 'Generalize' various datasets.

- FINAL REPORT
As per our final Model, the top 3 predictor variables that influences the bike booking are:
  
<li><b>Temperature (temp) -</b> A coefficient value of ‘0.5733’ indicated that a unit increase in 
temp variable increases the bike hire numbers by 0.5733 units.</li>
<li><b>Weather Situation 3 (weathersit_3) -</b> A coefficient value of ‘-0.30773’ indicated that, w.r.t Weathersit1, 
a unit increase in Weathersit3 variable decreases the bike hire numbers by 0.30773 units.</li>
<li><b>Year (yr) -</b> A coefficient value of ‘0.2305’ indicated that a unit increase in 
yr variable increases the bike hire numbers by 0.2305 units.</li>
So, it's suggested to consider these variables utmost importance while planning, to achive maximum Booking


<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- jupyter notebook
- librarys used are:<br>
  numpy<br>
  panda<br>
  matplotlib<br>
  seaborn<br>
  feature_selection<br> 
  linear_model <br>
  variance_inflation_factor<br>
  statsmodels

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->



## Contact
Created by [@IshrathFathima] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
