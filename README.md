# Air-quality-analysis-from 2010-2014
## Impact of Weather Conditions on Air Quality
![](https://github.com/bellaTHEanalyst/powerbi-report-weather-quality-analysis-/blob/main/environmental%20and%20air%20agency%20picture.jpeg) 


## Introduction
I’m Isabella Martins, and I’m excited to share some insights about your business. This is a power project on predictive analysis of air quality using regression. Thank you for providing the guiding questions. It was helpful to see what types of insights you are looking to gain from the data. I hope you find the analysis compelling and helpful as you make decisions regarding future business opportunities.

## Problem Objective
This project is on a company in the environmental consulting industry that is seeking to analyze the air quality in a specific city during hot and cold weather, during high-wind conditions in air quality, analyze and derive insights to help make recommendations to give the government and business in the region on how to mitigate the impact of weather conditions on air quality.

## Problem statement
1. What is air quality?

2. What does PM 2.5 mean in air quality?

3. What weather factors influenced the PM 2.5 value?

4. What years recorded the highest and lowest PM 2.5 value?

5. What is the predictions on PM2.5 value in air quality in the next 4 years?
## Data Source
Song Xi Chen, csx '@' gsm.pku.edu.cn, Guanghua School of Management, Center for Statistical Science, Peking University
[clickhere](https://archive.ics.uci.edu/ml/datasets/Beijing+PM2.5+Data)

## Data Set Information

- Number of attributes: 13

- Missing values : Yes 

- Duplicate values : No

## SKILLS/CONCEPTS DEMONSTRATED
- Power Query
- Dax
- Modeling
- Quick measure

## MODELLING
I tried to create a relationship using date tabels,though it wasn’t necessary as we have just  one fact table and no dimension table, but a relationship was created between tables using the dates.
![](https://github.com/bellaTHEanalyst/powerbi-report-weather-quality-analysis-/blob/main/weather%20model.jpg)

## Data Preparation/Cleaning
- The dataset contained 13 columns and 41,757 rows.
1. I made first rows as headers
2. I filtered out all null values
3. I changed datatype from 'TEXT" to 'WHOLE NUMBER'
![](https://github.com/bellaTHEanalyst/powerbi-report-weather-quality-analysis-/blob/main/powerquery%20table.jpg)
4. I created a new measure for month as “short_month” 
![](https://github.com/bellaTHEanalyst/powerbi-report-weather-quality-analysis-/blob/main/short_month.jpg)

 ## SOLUTION
 ## What is air quality?
Air quality refers to the degree to which the air is suitable or clean enough for humans or the environment

 ## What is PM2.5 with concentration (ug/m^3)
 
Pm2.5 is used when describing pollutant levels both outdoors and indoors, where health impact from exposure considers the amount of pm2.5 over a 24-hour period.PM2. 5 at or below 12 μg/m3 is considered healthy with little to no risk from exposure. If the level goes to or above 35 μg/m3 during a 24-hour period, the air is considered unhealthy and can cause issues for people with existing breathing issues such as asthma.

## What does PM 2.5 mean in air quality?
Fine particulate matter (PM2.5) is an air pollutant that is a concern for people's health when levels in the air are high. PM2.5 are tiny particles in the air that reduce visibility and cause the air to appear hazy when levels are elevated

# **NOTE** : pm2.5 in this dataset is given in(ug/m^3)
 ## Analyzation 1: What weather factors influenced the PM 2.5 value?
Weather factors that affect the PM2.5 value include the dewpoint, temperature, combined wind direction, hours of rainfall, hours of snow, and hours of the day
- Visual 1:
Dew point:  The points in the scatterplot can be seen rising from left to right with all points nearby and we see a high positive correlation here; the dew point is positively correlated with the PM 2.5 values. As the dew point increased, so did the PM 2.5 value except for a few cases of outliers. The highest PM 2.5 value was experienced at -24(â„ƒ) 
![](https://github.com/bellaTHEanalyst/powerbi-report-weather-quality-analysis-/blob/main/visual%201%20weather.jpg)

- Visual 2
Temperature:  This shows that as temperature increases PM 2.5 decreases. The PM 2.5 value can be seen to have a low negative correlation with temperature. This probably explains why its value is highest at midnight when the temperatures are usually lowest then it decreases in the afternoon when the temperature is around its peak. A few cases of outliers were observed

![](https://github.com/bellaTHEanalyst/powerbi-report-weather-quality-analysis-/blob/main/visual%202%20weather.jpg)

- Visual3
 Hours of snowfall:  The points in the scatterplots can be seen falling while moving from left to right with the points in scattered forms. The PM 2.5 value can be seen to have a low negative with hours of snowfall. The hours of snowfall were seen to consequentially affect the PM 2.5 values. As the hours of snowfall increased, the PM 2.5 values decreased.
![](https://github.com/bellaTHEanalyst/powerbi-report-weather-quality-analysis-/blob/main/visual%203%20weather.jpg)

- Visual 4
Hours of the day:   I observed a few cases of outliers and there was no cluster in the scatterplot. The PM 2.5 recorded its highest value 994ug/m³   which was an outlier around 1:oo am
![](https://github.com/bellaTHEanalyst/powerbi-report-weather-quality-analysis-/blob/main/visual%204%20weather.jpg)

- Visual 5
Combined wind direction: I used a column chart to analyze the relationship between the combined wind direction and the average pm2.5 value, I see a perfect negative correlation which forms almost a straight line.  Wind direction can be seen to negatively correlate with the average PM 2.5 values. Days with calm/variable recorded the highest average PM2.5 values and north wind recorded the lowest average PM 2.5 value.
![](https://github.com/bellaTHEanalyst/powerbi-report-weather-quality-analysis-/blob/main/visual%205%20weather.jpg)

- Visual 6.
 Hours of rainfall: The results showed that the PM 2.5 value has a low negative correlation with rainfall as points can be seen falling from left to right. The lower the hours of rainfall, the higher the concentration of PM 2.5 and vice versa. The PM 2.5 value was at its highest when there was no rainfall and its value decreased as the hours of rainfall increased.
![](https://github.com/bellaTHEanalyst/powerbi-report-weather-quality-analysis-/blob/main/visual%206%20weather.jpg)

## Analyzation 2: Which month and year recorded the highest and lowest PM 2.5 value?
I used a line chart to create a trend analysis to analyze the pm2.5 values over across the years and months.
![](https://github.com/bellaTHEanalyst/powerbi-report-weather-quality-analysis-/blob/main/analysis%202.jpg)
- I noticed that in January 2013, the average PM 2.5 value recorded its highest value of 193.27 ug/m³ while its lowest value of 60.00 ug/m³ was recorded in December 2012

## Analyzation 3: What is your forecast projection of the average pm2.5 value in the next 4 years?
I used a line chart to forecast the average pm2.5 value in the next 4 years as shown below:

![](https://github.com/bellaTHEanalyst/powerbi-report-weather-quality-analysis-/blob/main/analysis%203.jpg)

I discovered   that after 2014, the PM 2.5 value values will most likely increase  from 97.73 ug/m³ in 2014 to about 101.71ug/m³ in 2015 and declined to 90.55 ug/m³ and rised to 101.71 ug/m³ in 2018.

## Recommendations
1.	  More volunteers to be recruited into the SDGS(sustainable development goals) organization  to help support and promote  the 
     SDG goal 13:CLIMATE CHANGE .

2.	The government should Integrate weather and air quality change measures into   national policies, strategies, and planning to help monitor and regulate     PM 2.5 value

3.	 Government should promote  mechanisms for raising capacity for effective weather change-related planning and management in  rural communities, least-       developed countries, and small island developing States, including focusing on women, youth, and local and marginalized communities
 
4. Awareness campaigns should be organized to sensitize the members of the public about PM 2.5  ( the meaning, safe and hazardous levels, and the causes      and effects it has in the environment)

5. Wild fires, bush burning, burning of gas in motorized vehicles, industrial processes, power generators, stoves, fireplaces, smoking tobacco, etc. all       of these activities should be discouraged.

6.	People should  be sensitized about the effects of high pollution  on their health, awareness campaigns to help people see how dangerous high pm 2.5         levels can cause health problems 
 
 








 









 



