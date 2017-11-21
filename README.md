# Project *Weather Phenomena of Stuttgart, Baden-Württemberg Region, Germany*

## Comparision of Temperature, Precipitation and Snow Depth of Six Cities near the latitude of 48°47′N (where Stuttgart lies)

### Introduction

As a citizen of Stuttgart, I would like to compare the weather data of cities which lie at the similar latitudes of Stuttgart. 

On the plots, groups of data under comparisons are

* Average daily temperatures in Celsius
* Average aggregated monthly precipitation (mm)
* Average daily snow depth (mm)


Cities under comparison are: 

City | Latitude | Altitude | Elevation (m) | Populoation | Country
-----|---------:|---------:|----------:|-----------:|-----------|
Stuttgart | 48°47′N  | 9°11′E | 332.50 | 623,738 | Germany
Vienna | 48°12′N | 16°22′E | 199.00  | 1,867,960 | Austria
Qiqihar | 47°21′N | 123°55′E |  148.00  | 5,357,003 | China
Bellingham | 48°45′1″N | 122°28′30″W | 79.82  | 80,885 | USA
Quebec City | 46°49′N | 71°13′W | 89.64   | 531,902 | Canada
Paris | 48°51′24″N | 2°21′03″E |  81.85  |  2,229,621 | France


* Source of the data in the table above: Wikipedia, National Centers for Environmental Information (NCEI) [Daily Global Historical Climatology Network](https://www1.ncdc.noaa.gov/pub/data/ghcn/daily/readme.txt) (GHCN-Daily).
 
* Source of the weather data: NCEI.

### Comment on the data downloaded from NCEI

I chose the unit of "Metric" when I downloaded the data. So that the values of temperatures, precipitation and snow depth in the tables are all in millimetre, not tenth of millimetre.  


### Comment on the choice of plot types for each subplot

Subplot  | Plot Type | Reason
---------|-----------|--------
average daily temperatures | line plot | Intuitive choice for a sequence that only has mild difference between consecutive two days
average aggregated monthly precipitation | bar plot | Tried line plot, but, when six cities are plotted on the same chart, this line plot is ugly and difficult to read because of many wild intersections between the lines. So I chose bar plot at the end. 
average daily snow depth | line plot | Similar to the "average daily temperatures plot". The trick here is, snows depth is very different from precipitation. Because snow depth doesn't reset to zero when a day ends, while precipitation can be measured from zero on a new measure time point. So the snow depth has much more continuity over days than the amount of daily rain water. Aggregating daily value over a month for snow depth does not make sense. 

* This is the assignment project of the Online Course *Applied Plotting, Charting & Data Representation in Python*