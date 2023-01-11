## Bike-Sharing demand analysis 
A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.
A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state. 



## Table of Contents
- [Problem Description](#general-information)
- [Technologies Used](#technologies-used)
- [Conclusions](#conclusions)
- [Acknowledgements](#acknowledgements)

## Problem Description
To build a model that explain demand for shared bikes with the available independent variables. 
To understand how exactly the demands vary with different features. 
They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. 
Model should be a good way for management to understand the demand dynamics of a new market. 

## Conclusions
- Temprature, weathersit, season, year, month are the most important factor to predict demand
- Year:
    - Year is important since every year there will be some improvement, development and advertizing in company which will increase its demand.
- Season:
    - Demand changes with spring,summer,fall, winter:
        - In spring demand is lowest
        - In summer demand is good 
        - In fall demand is at peak
        - In winter demand is good
- Month:
    - Month give more information about demand
- Temprature: It have positive correlation with demand
- Weathersit:
    - Demand changes with weather:
        - 1: Clear, Few clouds, Partly cloudy, Partly cloudy
            - Demand is at peak in clear weather
        - 2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
            - Demand is good
		- 3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
            - Demand is at lowest
		- 4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
            - No demand at all

## Technologies Used
- Python
	- numpy
	- pandas
	- matplotlib
	- statsmodels
	- seaborn

## Dataset characteristics
day.csv have the following fields:	
	- instant: record index
	- dteday : date
	- season : season (1:spring, 2:summer, 3:fall, 4:winter)
	- yr : year (0: 2018, 1:2019)
	- mnth : month ( 1 to 12)
	- holiday : weather day is a holiday or not (extracted from http://dchr.dc.gov/page/holiday-schedule)
	- weekday : day of the week
	- workingday : if day is neither weekend nor holiday is 1, otherwise is 0.
	+ weathersit : 
		- 1: Clear, Few clouds, Partly cloudy, Partly cloudy
		- 2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
		- 3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
		- 4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
	- temp : temperature in Celsius
	- atemp: feeling temperature in Celsius
	- hum: humidity
	- windspeed: wind speed
	- casual: count of casual users
	- registered: count of registered users
	- cnt: count of total rental bikes including both casual and registered
	
## License
Use of this dataset in publications must be cited to the following publication:

[1] Fanaee-T, Hadi, and Gama, Joao, "Event labeling combining ensemble detectors and background knowledge", Progress in Artificial Intelligence (2013): pp. 1-15, Springer Berlin Heidelberg, doi:10.1007/s13748-013-0040-3.

@article{
	year={2013},
	issn={2192-6352},
	journal={Progress in Artificial Intelligence},
	doi={10.1007/s13748-013-0040-3},
	title={Event labeling combining ensemble detectors and background knowledge},
	url={http://dx.doi.org/10.1007/s13748-013-0040-3},
	publisher={Springer Berlin Heidelberg},
	keywords={Event labeling; Event detection; Ensemble learning; Background knowledge},
	author={Fanaee-T, Hadi and Gama, Joao},
	pages={1-15}
}
