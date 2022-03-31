# JC_bikesharing
Module 14: NY Citibike with Tableau

# Overview of the analysis:

The following analysis aims to show the length of time that bikes are checked out for all riders and genders, to show the number of bike trips for all riders and genders for each hour of each day of the week and to show the number of bike trips for each type of user and gender for each day of the week.

3 parts are accomplished and can be explored following this [link]( https://public.tableau.com/app/profile/juanita.camargo/viz/JC_bikesharing_challenge/NYCCitiBikeStory?publish=yes):

- D1: Change Trip Duration to a Datetime Format
- D2: Create Visualizations for the Trip Analysis
- D3: Create a Story and Report for the Final Presentation

Furthermore, a story was created to gather all the Dashboards and Worksheets produced during the analysis of this Challenge:

![NYC CitiBike Story](/__Resources/TableauNYCCitiBikeStory.gif)

The following dashboard (included as introduction in the story presented above) shows a summary of the Number of Rides, Type of Users distribution and the August Peak Hours per Gender.

![NYC CitiBike Dashboard](/__Resources/NYCCitiBikeDashboard.jpg)

# Resources:
 
  **Data source** Large csv files have been used in this analyses and are not available in the repo. 

  **Software** Pandas, Tableau Desktop, Jupyter Notebook, Excel.

# Results:

Once the Trip Duration datetime was edited through Pandas, the code is available in [NYC_Citibike_Challenge.ipynb](https://github.com/juanitacosmica/JC_bikesharing/NYC_Citibike_Challenge.ipynb) we were able to export the new data, and upon plugging it to Tableau the following analysis was made:

1. Checkout Time for Users:

![Checkout Time for Users](/__Resources/CheckoutTimesForUsers.jpg)

The chart above shows the count of bike IDs (number of trips) on the y-axis and the trip duration on the x-axis, this trip duration is split in hours and minutes. 

- Conclusion: It can be appreciated that the most frequent trip duration is between 3 hours to 9 hours (around 1,101,425 trips), followed by longer trip duration of 9 to 24 hours (around 1,021,670 trips). The shorter trip duration was between few minutes to 3 hours (around 236,526 trips).

2. Checkout Time for Users By Gender:

![Checkout Time for Users by Gender](/__Resources/CheckoutTimesByGender.jpg)

The chart above shows the count of bike IDs (number of trips) on the y-axis and the trip duration on the x-axis, this last is split in hours and minutes. The 3 colors represent the classification of gender, as seen in the legend.

- Conclusion: It can be appreciated that the checkout times for male is much higher than for female and unknown gender, mostly between 1 hour to 10 hours checkout time trip duration.

3. Trips by Weekday per Hour:

![Trips by Weekday per Hour](/__Resources/TripsByWeekdayPerHour.jpg)

The chart above shows the total trips per hour and per weekday. The y-axis is the hours and the x-axis contain the weekdays; while the color shows the total of trips. The darker the color represents more trips, whereas the lighter the color means a smaller number of trips. 

- Conclusion: It can be appreciated that the greatest number of trips occur in the morning during weekdays between 6 am and 9 am, and, in the evening during weekdays between 5 pm and 7 pm. For the weekends, the greatest number of trips occur mid-day around 10 am and 6 pm.

4. Trips by Gender, Weekday per Hour:

![Trips by Gender Weekday per Hour)](/__Resources/TripsByGenderWeekdayPerHour.jpg)

The chart above shows the total trips per hour and per weekday. The y-axis is the hours and the x-axis contain the weekdays; while the color shows the total of trips. The darker the color represents more trips, whereas the lighter the color means a smaller number of trips. Plus, there is a differentiation between genders: male, female and unknown. 

- Conclusion: It can be appreciated that the distribution of the checkout times for all genders is quite alike, it gets busier in the morning during the weekdays from 6am to 9am and in the evening during weekdays from 5 pm to 7 pm. Whereas the weekends gets busier mid day around 10 am and 6 pm. But also, the males have significant higher number of trips to those taken by the females and unknown gender.

5. User Trips by Gender by Weekday

![User Trips by Gender by Weekday](/__Resources/TripsByGenderByWeekday.jpg)

The chart above shows the total number of trips by weekday, by user type (subscribers and customers) and by gender. The x-axis is the gender and the y-axis is the weekdays. 

- Conclusion: It can be appreciated that from the subscribers, the male have the largest number of trips especially on Thursdays and Fridays, followed by trips on Monday and Tuesdays; the female have similar distribution of trips, with significant lower number of trips than the male; and, the unknown gender have uniform distribution of trips along the week. For the customers’ data it can be seen that significant less trips happen for all genders with a slight increase in the unknown gender on Saturdays and Sundays.

6. Bike Utilization

![Bike Utilization](/__Resources/BikeUtilization.jpg)

The chart above shows all the bikes and the accumulated trip utilization (datatype for the time used is used as integer for easier calculations).
- Conclusion: It can be appreciated from 4 groups: Small bubble shows around 200,000 time units, Medium-small bubble shows around 300,000 time units, Medium bubble shows around 1,000,000 time units and Large bubble shows around 2,000,000 time unit. Therefore, this can be used to classify the bikes into groups to build a maintenance plan, rotation and distribution according to the stations (shown in the coming point).

7. Top Starting Locations & Top Ending Locations

![Top Starting Locations & Top Ending Locations](/__Resources/TopStartingLocations.jpg)
![Top Starting Locations & Top Ending Locations](/__Resources/TopEndingLocations.jpg)

The charts above let us appreciated the most popular starting and ending locations, the legend shows the colors per type of users. Larger bubbles are locations with the greatest number of trips, and smaller bubbles are the ones with a smaller number of trips. 
- Conclusion: It can be appreciated which stations are more popular between the subscribers and customers, furthermore, what areas are the most popular compared to others. Downtown appears to be more popular than other areas.

All Tableau screenshots results are available for viewing in the [Resources Folder](https://github.com/juanitacosmica/JC_bikesharing/__Resources).

# Summary:

Tableau is a powerful tool that allows to plug the data and get visualization easier for the users to read and understand. The results above permitted a good at glance of the bike trips and bike users in NYC, the distribution by gender and the peak times. From that another two things to bear in mind for a bike business are the two following: 

1. Bike maintenance

![PopUp Markers](/__Resources/BikeRepairs.jpg)

Heat maps are great visualization for large amount of data and provides a clear story of the data. The conclusion is that the Peak Hours per Gender, Trips by Weekday per Hour and Trips by Gender (Weekday per Hour) have the less busy from 11pm and 5am, which suggests it can be a good time for bike maintenance. And along with the Bike Utilization, shown in #6 above, a stagger plan can be created for rotation type of maintenance of the bikes from popular stations to less popular stations as seen in #7 above.

2. Average Trip Duration

![Average Trip Duration](/__Resources/AverageTripDuration.jpg)

Area charts are a great visualization for Averages, this can be used when analyzing the bike maintenance required.

People call me JC, the short for [Juanita C. Nunez](https://www.linkedin.com/in/juanitacamargonunez/). Contact me for any questions! I love networking, so here you go  my [LinkedIn] (https://www.linkedin.com/in/juanitacamargonunez/) :)

