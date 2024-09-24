# Linear Regression Bike Sharing Assignment
> A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the system.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state.

In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine end across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around ans stand out from other service providers and make huge profits.

They have contracted a consulting company to understand the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market. The company wants to know:

- Which variables are significant in predicting the demand for shared bikes.
- How well those variables describe the bike demands.

Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the American market based on some factors.

Business Goal:
- Model development for shared bikes demand based on available independent variables.
- This model will be used by the management to understand how exactly the demands vary with different features.
- Management can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations.
- Further, the model will be a good way for management to understand the demand dynamics of a new market.

What is the dataset that is being used?

Description of all the columns in the dataset

- instant: record index
- dteday : date
- season : season (1:spring, 2:summer, 3:fall, 4:winter)
- yr : year (0: 2018, 1:2019)
- mnth : month ( 1 to 12)
- holiday : weather day is a holiday or not
- weekday : day of the week
- workingday : if day is neither weekend nor holiday is 1, otherwise is 0.
- weathersit :
   1: Clear, Few clouds, Partly cloudy, Partly cloudy
   2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
   3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
   4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
- temp : temperature in Celsius
- atemp: feeling temperature in Celsius
- hum: humidity
- windspeed: wind speed
- casual: count of casual users
- registered: count of registered users
- cnt: count of total rental bikes including both casual and registered


<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- With high R-squared (0.815) for train set and test set (0.834), this model explains the variability of the dependent variable i.e. cnt suggesting that the model fits the data quite well.
- yr (Year) has positive coefficient indicating that the demand is increasing over the time. So, demand is more in 2019 compared to 2018.
- holiday has negative coefficient indicating that the demand decreases on holidays.
- temp (Temperature) as positive coefficient indicating that there are higher demands when there's increase in temprature.
- hum (Humidity) has negative coefficient indicating that the higher humidity gradually decreases the demand for bikes.
- windspeed has negative coefficient which indicates that the higher wind speed decreases the demand.
- season_spring has negative coefficient indicating negative impact on the demand while season_winter has positive coefficient indicating positive impact on the demand.
- mnth_Jul, mnth_Nov and weathersit_Good have negative coefficients indicating negative impact on the demand.

- We can conclude that the above mentioned variables are some of the different variables which affect bike demand dynamics and we can say that the analysis of seasonal trends can really help in planning and forecasting bike demands precisely.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- Numpy - version 1.26.4
- Pandas - version 2.2.2
- Matplotlib - 3.8.4
- Seaborn - 0.13.2
- Sklearn - 1.4.2
- Statsmodel - 0.14.2


<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Contact
Created by @AjtMishra


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
