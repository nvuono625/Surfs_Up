# Surfs Up Analysis
## Overview
An investor is presented the oppurtunity to back a business plan in Oahu, Hawaii. The idea is to create a shop called "Waves and Ice Cream", a shop that would sell surfboards and ice cream to locals and tourists. It is our job to conduct an analysis on a weather dataset from Oahu, Hawaii to determine whether it is in the best interest to open this shop.

## Results
It is understood in this analysis that the business' success depends on the weather and the location may be the advantage this business has for it's success. Weather data, both temperature and precipitation, in Oahu, Hawaii, was gathered. 

Employing Jupyter notebook, Pandas functions and a Python SQL toolkit, SQLAlchemy, was used to create an engine to connect to the SQLite Database (hawaii.sqlite). the data was then reflected into a new model in order to retrieve the temperature and precipitation data between the months of 08.23.2016 and 07-10-2017. Once the data was retrieved, the data was converted to a list and from there, converted into a DataFrame. At this point, the statistics could then be generated into visualizations.

### Temperature Vs Frequency (Year)
- A histogram was created to show the frequency distribution of all the various temperatures throughout the year using data from just one station. This station was of the most active of the nine stations.
	 - The results show that temperature between 75°F-77°F occurred most throughout the year.
	 
![/Resources/Temperature_vs_Frequency.png](/Resources/Temperature_vs_Frequency.png)

### Precipitation (Year)
- A simple vertical line chart was ceated to show precipitation for one year, specifically between 08.23.2016 and 07-10-2017.
	- These results show how often storms generally come and go throughout the year. You can see that major storms (outliers) occur not in the months of June or Decemeber and for this reason we will analyze them to show data that will not be skewed by outliers.
	
![/Resources/Precipitation_Troughout_The_Year.png](/Resources/Precipitation_Troughout_The_Year.png)

### June Vs December Temperature
- Now from all nine stations, temperature data from June and December was converted into a DataFrame that showed basic summary statistics (Count, Mean, Standard Deviation, etc.).
	- There are more counts in June (1700.00) than in December (1517.00).
	- The highest temperature only varies by ~2°F, with June having the high of 85°F & December having the high of 83°F.
	- The lowest temperature varies more than the high, by ~8°F. June's low is 64°F & December's low is 56°F).
	- The mean (average) temperature for June is 74.944118°F and for December, 71.041529°F. The average pnly varies by 3.902589°F
	
June Temperature           |  December Temperature
:-------------------------:|:-------------------------:
![/Resources/June_Temperature.png](/Resources/June_Temperature.png)  |  ![/Resources/December_Temperature.png](/Resources/December_Temperature.png)

### June Vs December Precipitation
- Also from all nine stations, precipitation data from June and December was converted into a DataFrame that showed basic summary statistics (Count, Mean, Standard Deviation, etc.).
	- There are more counts in June (1574.00) than in December (1405.00).
	- The highest precipitation varies by 1.99, (June's reading is 4.43 & December's reading is 6.42, the high).
	- The lowest precipitation varies the same, with June and December both reading a minimum of 0.00.
	- The mean (average) precipitation for June is 0.136360 and for December, 0.216819. 
	- December has the higher precipitation but only varies by 0.080459.

June Precipitation          |  December Precipitation
:-------------------------:|:-------------------------:
![/Resources/June_Precipitation.png](/Resources/June_Precipitation.png)  |  ![/Resources/December_Precipitation.png](/Resources/December_Precipitation.png)

## Summary
Now, with all this information, it is safe to say that the "Waves and Ice Cream" shop could be open year round with Decembers weather only varying by 3.902589°F less than June and a precipitation of 0.080459 more than June. There might be a few days in December where the shop may need to close but overall the temperature doesnt change all that much. Further analysis may be necessary to account for the major storms, which according to our year long precipitation vertical line chart, the store may need to close a handful of times throughout the year.
