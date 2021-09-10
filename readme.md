# Bike Sharing Analysis with Ford GoBike Data
## Nima Afshar

## Dataset

Bay wheels was primarily a public bicycle sharing system in California which started working in 2013 as "Bay Area Bike Share". After 5 years in 2018 it had over 2,600 bicycles in 262 stations around San Fransisco, East Bay and San Jose. From 2017, Ford Motor company took partnership and company been renamed to Ford GoBike. After Motivate's acquisition by Lyft, the system was renamed to Bay Wheels in June 2021.

#### Data wrangling process:
- fix multiple fields that are not in the correct dtype, i.e. `start_time`, `end_time` should be datetime type, `user_type` and `member_gender` should be categorical data type, etc
- add new columns for trip duration in minute, trip start date in yyyy-mm-dd format, trip start hour of the day, day of week and month
- add a new column calculating riders' age from 'member_birth_year'
- filter out outlier ages from visual examination of the member age distribution and statistical percentile
- cast 'member_age' to integer instead of float type
- cast 'start_dayofweek' to category dtype
- cast 'start_month' to category dtype for easy plotting
- filter out outlier trip records where the duration was very long


## Summary of Findings

people use system more around 8-9 AM and 4 to 6 PM. more trips been done during the week days. Perhaps since the weather is better more bike were used during the summer. 
number of male user are almost 3 times the number of female users. Most members age are around 25 to 40. Subscribers are way more than casual users. Subscribers use the bike more in the morning during the week in
order to get to work and casual users use bike more during the weekends.



## Key Insights for Presentation

Different usage pattern/habit between the two type of riders are seen from the exploration. 