# Cyclistic-Bike-Share-Analysis - 2023
Google Analytics Case study: How does a bike-share navigate speedy success? The objective is to identify key insights that will inform the development of a targeted marketing strategy focused on converting casual riders into annual members. By understanding these distinctions, develop a data-driven marketing strategy to maximize the number of annual members, thus leading the way to the company's future success.
## Dashboard Link - 
https://public.tableau.com/views/CyclisticBikeShareAnalysis-2023/CyclisticBikeSales?:language=en-US&:sid=&:display_count=n&:origin=viz_share_link
## Data Analysis Phases Steps: Ask, Prepare, Process, Analyze, Share and Act
### ASK PHASE - 
#### 1. Define the Problem - 
  Define a marketing Strategy focusing on converting casual riders to annual riders by maximizing the number of annual members, thus leading the way for the company's future success
#### 2. Consider key stakeholders - 
  1. Lily Moreno: Director of marketing team
  2. Cyclistic marketing analytics team: Data analysts team who are responsible for collecting, analyzing, and reporting data that helps to guide Cyclistic marketing strategy
  3. Cyclistic executive team: Detail-oriented executive team will decide whether to approve the recommended marketing program.
#### 3. Question - 
  How do annual members and casual riders use Cyclistic bikes differently?
### PREPARE PHASE - 
#### Dataset Link - 
https://divvy-tripdata.s3.amazonaws.com/index.html
#### Dataset Description - 
The dataset contains historical ride data from Cyclistic, a bike-share service operating in Chicago. The data provides insights into how customers utilize the bike-share service, including ride_id, rideable_types, starting and ending time, start and end locations, user type (casual or member). I focused on using 2023 data for this case study. The data has been made available by Motivate International Inc. under license. For more details, you may refer to https://divvybikes.com/data-license-agreement. 
#### Variables:
1. ride_id: Unique identifier for each ride, consisting 16 characters - Example: 'F96D5A74A3E41399'
2. rideable_type - Types of bikes: electric_bike, classic_bike and docked_bike
3. Start Time: Date and time when the ride began in format of MM/DD/YYYY HH:MM:SS AM/PM
4. End Time: Date and time when the ride ended in format of MM/DD/YYYY HH:MM:SS AM/PM
5. Start Station ID: Identifier for the station where the ride originated.
6. Start Station Name: Name of the station where the ride originated.
7. End Station ID: Identifier for the station where the ride ended.
8. End Station Name: Name of the station where the ride ended.
9. start_lat - Latitude of starting station
10. start_lng - Longitude of starting station
11. end_lat - Latitude of ending station
12. end_lng - Longitude of ending station
13. member_casual - Indicates whether the rider is a casual user or an annual member.
### PROCESS PHASE - 
The Cyclistic bike share data will undergo thorough preprocessing to ensure its suitability for analysis. This will involve tasks such as handling missing values, standardizing data formats, and encoding categorical variables. Additionally, data exploration techniques may be employed to gain a deeper understanding of the dataset's structure and identify any initial patterns or trends that could inform subsequent analysis strategies.
Here, I used SQL WORKBENCH for the data preprocessing as Microsoft Excel is unable to accomplish due to its limitations with large datasets.

1. Data Combining: https://github.com/Jyosna059/Cyclistic-Bike-Share-Analyisis-2023/blob/8318c44ad0942838a58ddf0041b56d7e7e146572/Data%20Combining  
   
2. Data Exploration: https://github.com/Jyosna059/Cyclistic-Bike-Share-Analyisis-2023/blob/8318c44ad0942838a58ddf0041b56d7e7e146572/Data%20Exploration
   
3. Data Cleaning: https://github.com/Jyosna059/Cyclistic-Bike-Share-Analyisis-2023/blob/8318c44ad0942838a58ddf0041b56d7e7e146572/Data%20Cleaning

### ANALYZE PHASE - 
The Cyclistic's bike share data will be subjected to various statistical and analytical techniques to extract actionable insights. this will involve identifying correlations between different variables, conducting trend analysis to understand patterns over time, and possibly employing predictive modeling to forecast future trends. 
1. Data Analyzing - Data analysis involves applying statistical and analytical techniques to uncover patterns, trends, and relationships within the dataset. By interpreting the data, can extract meaningful insights that inform decision-making and drive strategic actions.
https://github.com/Jyosna059/Cyclistic-Bike-Share-Analyisis-2023/blob/8318c44ad0942838a58ddf0041b56d7e7e146572/Data%20Analysis

### SHARE PHASE - 
After performed analysis and gained some insights into data, created visualizations to share your findings of the follwing question "How do annual members and casual riders use Cyclistic bikes differently?" that mentioned earlier, I have created 5 dashboard visualizations to answer this question by using a software such as 'TABLEAU'.
1. This visualization shows bikes types used by riders in 2023 by two groups of users.
   https://public.tableau.com/views/CyclisticBikeShareAnalysisBikeTypes/Biketypesin2023?:language=en-US&:sid=&:display_count=n&:origin=viz_share_link
   ![Bike types in 2023](https://github.com/Jyosna059/Cyclistic-Bike-Sales-Analyisis/assets/111238384/48619c73-c557-4dd0-a985-23b58dd7a06a)
  The outcome reveals that there are currently 1,03,014 active members, representing nearly 75.53% of the total user base, while the remaining 24.47% (77805) consists of casual riders. Classic bike with 47.01% (48,426) has the most popularity among users and followed by the electric bike with 25.52% (29,379). However, only 1.69% of users use docked bikes.
  
2. This Visualization shows the total number of trips in 2023 by month, weekday and hour.
   https://public.tableau.com/views/CyclisticBikeShareAnalysisNumberofTrips/Total_tripsin2023?:language=en-US&:sid=&:display_count=n&:origin=viz_share_link
   ![Total_trips in 2023](https://github.com/Jyosna059/Cyclistic-Bike-Sales-Analyisis/assets/111238384/a61b0633-265a-4e65-91ac-470b0157bbc0)
   For monthly data, both casual and member users demonstrate comparable patterns, showing increased travel during the starting of month (January) and decreased activity in the winter at the month of end (DECEMBER). Looking at the graph that indicates number of trips by day, casual and member riders shows opposite patterns. Members tend to make their ride on Tuesday and casual users prefer to make their journey on weekends. When examining hourly data, a clear trend emerges: both types of users overwhelmingly prefer riding during the morning at 8am and in the evening at 5pm.
   
3. This Visualization shows average ride duration per minutes by month, weekday, hour in 2023.
   https://public.tableau.com/views/CyclisticBikeShareAnalysisAverageRideDuration/AverageRideDurationin2023?:language=en-US&:sid=&:display_count=n&:origin=viz_share_link
   ![Average Ride Duration in 2023](https://github.com/Jyosna059/Cyclistic-Bike-Sales-Analyisis/assets/111238384/a0a7aa90-aedd-4641-b3eb-80f9fb8d0b5e)
    This visualization shows the ride activity for both types of users during the spring and summer months but for month june member users increased the activity. This trend extends to the average ride duration by month (Above 20 minutes), with a substantial increase observed over the same period. And when we look at average ride duration by day, we can observe that both casual and member riders will spend more time for riding. For hourly data, between 10 am and 2 pm and night 11pm, users tend to embark on longer journeys during the day. Conversely, from five to eight in the morning, their trips are typically shorter in duration.

4. This visualization map shows the total trips at starting stations in 2023 by type of users.
   https://public.tableau.com/views/CyclisticBikeShareAnalysisStartingStations/StartingStationsin2023?:language=en-US&:sid=&:display_count=n&:origin=viz_share_link
   ![Starting Stations in 2023](https://github.com/Jyosna059/Cyclistic-Bike-Sales-Analyisis/assets/111238384/d17b1534-0eb7-4116-8597-ffcd0af421ab)
    'Desplaines St & Kinzie St' & 'Clinton St & Madison St' sees the highest volume of riders starting their rides at user annual members. 'Desplaines St & Kinzie St' & 'Clinton St & Madison St' is situated nearby to Jane Addams Memorial Park and the apartment building Lake Point Tower. Casual riders predominantly kick-start their trips from stations adjacent to museums, parks, beaches, harbors, and aquariums, while members opt to commence their journeys from stations proximate to universities, residential areas and commercial districts.

5. This visualization map shows the total trips at ending stations in 2023 by type of users.
   https://public.tableau.com/views/CyclisticBikeShareAnalysisEndingStations/Ending_Stationsin2023?:language=en-US&:sid=&:display_count=n&:origin=viz_share_link
   ![Ending_Stations in 2023](https://github.com/Jyosna059/Cyclistic-Bike-Sales-Analyisis/assets/111238384/9798ffae-b45d-4dfc-bd2d-c8f14e17c188)
    Most of the Member riders chose to end their journey at 'Kingsbury St & Kinzie St' & 'Clinton St & Madison St'. Casual riders of 'Streeter Dr & Grand Ave' and also often conclude their journeys near parks, museums, and recreational areas, while members tend to end their trips in proximity to residential areas and commercial districts.

### ACT PHASE
Recommendations for marketing strategy based on my analysis:
1. Highlight Membership Benefits: Highlight membership perks like exclusive features and discounts to attract casual riders to become annual members.
2. Promote Bike Types Preferred by Members: Promote classic and electric bikes favored by members in marketing campaigns targeting casual riders.
3. Seasonal Promotions: Offer seasonal discounts during peak biking months to encourage annual membership sign-ups.
4. Day and Hour Preferences: Emphasize the convenience of weekend and evening rides for annual members.
5. Strategic Station Placement: Place bike stations strategically in popular casual rider areas and showcase their accessibility with annual membership.
6. Personalized Recommendations: Leverage data analysis to provide personalized recommendations to casual riders, highlighting stations, bike types, and ride times that align with their preferences and behavior patterns.
7. Testimonials and Success Stories: Share success stories from existing members to illustrate the benefits of annual membership and inspire casual riders to join. Highlight how annual membership has transformed the biking experience for others and encourage casual riders to join the community.
