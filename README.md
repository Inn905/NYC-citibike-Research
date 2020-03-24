# NYC-citibike-Research
All HTML files are data analysis export files using jupyter notebook (python)
## [BaiduAPI.html](https://inn905.github.io/NYC-citibike-Research/HTML/BaiduAPI.html)
* Using Baidu API, using his own road planning, calculate the distance and time of walking, driving, and public transportation from the start to the end.  
* problem:  
The distance calculated using the Baidu API will obviously be more scientific, and the starting point and end point are the same although we use different methods, which can be mapped.
However, due to the quota limit of Baidu API, foreign route planning can only do 400 data a day, obviously not enough.  
Therefore, the following calculations are temporarily performed using Euclidean distance.  

## carbon dioxide.html
* Method for calculating carbon emissions of bicycles.  
The program only uses gasoline for the time being, which means that all bicycles are replaced with car-type carbon emission factors.  
* problem:  
The calculation method is this. It is still being studied how to solve the problem of the proportion of bicycles replacing different types of vehicles. Different types have different carbon emission factors, and the carbon emissions saved are different.  
Thinking, this ratio will be affected by factors such as weather and weekends. For example, it rains, fewer people choose to walk, more people drive, and the replacement ratio should be different.  

## citibike.html
* Some basic data analysis of citibike, morning and evening peaks, weekends, gender ratio and the like.  

## Mobike.html
* Analysis of some basic data of Mobike, morning and evening peaks, weekends and the like.  
* problem:  
Mobike's data was later found, only for 2017.  
If Mobike data can be used, the Baidu API can be used to calculate the distance and time. The domestic limit is 30,000, which is enough.  
But , Mobike's data looks like Shanghai's, but the overall coordinates are not accurate, as if the collective deviation.  
I haven’t thought about processing this data yet, first do the data for New York.  

## weather.html
* Regarding the correlation between weather and the frequency of bicycle use and the average riding distance, the temperature is bound to affect, and precipitation and snowfall are still under investigation. The problem is the data is insufficient.  
Then I found that the correlation between the weather is quite strong. I plan to use multiple linear regression to create something like "weather coefficient", which represents the impact of weather on the frequency of bicycle use and different types of replacement ratios.  
* problem:  
The weather data is from March 2013 to March 2019, some are missing in the middle and have not been processed yet.  
The experiment was done in March 2017.  
