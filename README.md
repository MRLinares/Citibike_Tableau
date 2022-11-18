# NYC Citibike Analysis

## Overview

Using csv files on NYC Citibike data, perform analysis on data for the month of August 2019.
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
The image above shows the overall ride count for the month of August 2019, a pie chart showing the breakdown of users by customer and subscriber, and a heat map showing the most active star/end destinations for Citibike users (which can be zoomed in and out for viewer comprehension).<br><br>


![peakHours](https://user-images.githubusercontent.com/108758105/202525107-a8833338-f0cb-46d1-81d2-3cddfebec1eb.png)
This visualization depicts the most active hours of the day in August 2019 in descending order which reveals that the end of the average workday (for those working 9-5) is the most active time for Citibike rides.<br><br>
 

![duration](https://user-images.githubusercontent.com/108758105/202596401-47debb31-675a-486a-9ee2-941ec1e3eb02.png)
This graph shows that the majority of all trips in August 2019 lasted less than 20 minutes.<br><br>

![weekdayByHour](https://user-images.githubusercontent.com/108758105/202597292-b477df36-97f1-4f03-9b2a-4d1da783be48.png)\
This heatmap highlights the heaviest hours of utilization for each weekday.<br><br>

![genderDash](https://user-images.githubusercontent.com/108758105/202597639-5a1f59db-2ef6-457f-af55-38383e74e349.png)
This visualization shows the breakdown of the prior metrics by gender with the blue heatmap further dividing by user type (customer vs subscriber).<br><br>

![story_maintenance](https://user-images.githubusercontent.com/108758105/202599093-1d5182b3-df19-44fa-8fbc-b25c1037697f.png)
Finally, this visualization shows the utilization of each bicycle in such a way that it makes it easy to plan for preventitive maintenance and/or repairs.  The overall screenshot including, text boxes above, is an example of how a Tableau Story would look on the website if one were to navigate to the link at the beginning of this "Results" section. 

## Summary

