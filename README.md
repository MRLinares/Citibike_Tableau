# NYC Citibike Analysis

## Overview

Using csv files on NYC Citibike data, perform analysis on data for the month of August 2019 to inform whether a Citibike program in Iowa may be feasible.
<br>
<br>
> ## ***Resources:***
>
> **Software:** Tableau Public, Python 3.7, Jupyter Notebook, Pandas
>
> **Datasource:** NYC Citibike Website: *[201908-citibike-tripdata.csv](https://s3.amazonaws.com/tripdata/index.html)*

## Results

Below are snapshots of the Tableau workbook that I created while performing analysis on the 201908-citibike-tripdata.csv file I downloaded from the NYC Citibike website.  I had to transform the tripduration column into datetime type from an object type in order to perform accurate analyses on it so I used jupyter notebooks and pandas to perform that transformation. Access to the actual Tableau Public workbook page by clicking the link here: [Citibike Tableau Story](https://public.tableau.com/app/profile/manny.linares/viz/Module_14_16666441765060/CitibikeStory)
 
 
![NYC_Citibike_Analysis_dash](https://user-images.githubusercontent.com/108758105/202524519-581e04e9-cfbb-41cb-ac39-1c218cade5af.png)
The image above shows the overall ride count for the month of August 2019, a pie chart showing the breakdown of users by customer and subscriber, and a heat map showing the most active start/end destinations for Citibike users (which can be zoomed in and out for viewer comprehension).<br><br>


![peakHours](https://user-images.githubusercontent.com/108758105/202525107-a8833338-f0cb-46d1-81d2-3cddfebec1eb.png)
This visualization depicts the most active hours of the day in August 2019 in descending order which reveals that the end of the average workday (for those working 9-5) is the most active time for Citibike rides.<br><br>
 

![duration](https://user-images.githubusercontent.com/108758105/202596401-47debb31-675a-486a-9ee2-941ec1e3eb02.png)
This graph shows that the majority of all trips in August 2019 lasted less than 20 minutes.<br><br>

![weekdayByHour](https://user-images.githubusercontent.com/108758105/202597292-b477df36-97f1-4f03-9b2a-4d1da783be48.png)\
This heatmap highlights the heaviest hours of utilization for each weekday.  The busiest hours during the work week were between 7am-9am and between 4pm and 7pm. For the weekend there seems to be an even distribution of utilization throughout the day between the hours of 9am and 7pm. It further emphasizes that 5pm-6pm and 8am are the highest hours of utilization given their dark red hue in comparison to the yellows and oranges throughout the rest of the map.<br><br>

![genderDash](https://user-images.githubusercontent.com/108758105/202597639-5a1f59db-2ef6-457f-af55-38383e74e349.png)
This visualization shows the breakdown of the prior metrics by gender.   There is far greater utilization by indivduals that identify as male in every metric.<br><br>

![userTripsByGenderWkday](https://user-images.githubusercontent.com/108758105/202770059-07725719-fc7a-4c59-9060-e11dfbe38359.png)\
The blue heatmap further divides by user type (customer vs subscriber). It appears that majority of subscribers identify as male and there is fairly even distribution of utilization throughout the week for each respective gender.<br><br>

![story_maintenance](https://user-images.githubusercontent.com/108758105/202599093-1d5182b3-df19-44fa-8fbc-b25c1037697f.png)
Finally, this visualization shows the utilization of each bicycle in such a way that it makes it easy to plan for preventitive maintenance and/or repairs.  The overall screenshot including, text boxes above, is an example of how a Tableau Story would look on the website if one were to navigate to the link at the beginning of this "Results" section. 

## Summary

The month of August, 2019, yielded:

* Total of 2,344,224 rides
* 1,900,359 (***81.1%***) subscriber vs. 443,865 (***18.9%***) non-subscriber
* Top Location: Grand Central Terminal (Mid-Town Manhattan) with 16,564 trip starts and 16,455 drop-offs.
* Peak Utilizaion hours for August: <br> 
&emsp; • 5pm - 224,566 total rides (***9.6%***) <br>
&emsp; • 6pm - 215,783 total rides (***9.2%***) <br>
&emsp; • 8am - 170,730 total rides (***7.3%***) <br>
* Rides up to 20 minutes account for 1,815,032 (***77.4%***) of total rides
* Rides up to 30 minutes account for 2,140,447 (***91.3%***) of total rides
* Gender breakdown: <br>
&emsp; • Out of total rides: <br> 
&emsp;&emsp;&emsp; • 1,530,272 (***65.3%***) reported as Male <br>
&emsp;&emsp;&emsp; • 588,431 (***25%***) reported as Female <br>
&emsp;&emsp;&emsp; • 225,521 (***9.6%***) Gender not reported <br>
&emsp; • Of the total rides up to 30 minutes (which accounted for 91.3% of total rides) 1,426,693 reported as Male (***61%***)<br>
&emsp; • 1,249,092 (***53%***) reported as Male for rides up to 20 minutes. <br>
&emsp; • Subscriber: <br>
&emsp;&emsp;&emsp; • Male: 1,372,601 (***58.6%***) <br>
&emsp;&emsp;&emsp; • Female: 493,752 (***21%***) <br>
&emsp;&emsp;&emsp; • Not Reported: 34,006 (***1.5%***) <br>
&emsp; • Non-Subscriber  <br>
&emsp;&emsp;&emsp; • Male: 157,671 (***6.7%***) <br>
&emsp;&emsp;&emsp; • Female: 94,679 (***4%***) <br>
&emsp;&emsp;&emsp; • Not Reported: 191,515 (***8.2%***) <br>

&emsp;&emsp; Given that the highest starting and ending location is the Grand Central Terminal and that most ustilization occurs during the morning and evening work commute, it is safe to assume that most rides occur for the purpose of commuting to work.  The New York Water Taxi location at the Lincoln Tunnel accounts for 13,435 starts and 14,018 drop-offs.  The Battery Park City/Vesey St. Ferry station accounts for 13,875 starts and 14,730 drop-offs.  It appears that people travelling to the city from non-NYC Subway routes (e.g. MTA North, LIRR, Water Taxi/Ferry) prefer to ride a bicycle from their stop to work as an alternative to transferring to NYC Subway/MTA Bus. 

Another analysis I would run would be the distances traveled. While duration could help understand how long someone had the bike, it doesn't show how far someone rode. 
