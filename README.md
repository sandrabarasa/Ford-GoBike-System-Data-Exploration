# Ford-GoBike-System-Data-Exploration
This data visualisation project involves exploration of individual rides made in a bike-sharing system covering the greater San Francisco Bay area.

## Dataset

This data set includes information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area. The data has a total of 183,412 rows and 16 columns with data showing:

* Duration of the trip in seconds.
* Start and end time of the trips.
* Start- and end-station names, IDs, latitudes and longitudes.
* Bike IDs.
* User Type ie Subscriber or Customer.
* Members' birth year and gender.
* Whether the bike was used for the whole trip or not.

### Pre-Wrangling
Before analysis of the data began, it was vital to assess and clean the data. Quality issues that were identified and cleaned included:
* Incorrect data type for columns 'start_time' and 'end_time' - should be datetime
* Missing values in columns: start_station_id, start_station_name, end_station_id, end_station_name, member_birth_year, member_gender
* Incorrect data type for columns 'user_type', 'member_gender' and 'bike_share_for_all_trip' - should be categorical data
* New column to show the day of the week when bikes were used
* Incorrect data type for the column 'member_birth_year' -Should be int; Add a column that shows member ages.

The wrangling resulted in a new dataset with 174,952 rows and 18 columns.

## Summary of Findings
My main focus of analysis was on duration, user type, members' age, members' gender, start day and bike-share-for-all-trip.

The key findings established include:
* There are more males than females and 'other' genders.
* There are more subscribers than there are customers, yet customers ride for a longer duration than subscribers.
* Thursday is the most popular day for starting the rides, followed by Tuesday and Wednesday.
* Most members cycle between 0 and 20,000 seconds (0 - 5.5 hours), with a majority not using the bikes for the whole trip.
* There is a higher cycling duration from people between the age 20 and 50 years old. 
* Saturday and Sunday record the highest average duration of rides.
* 'Other' gender category have longer durations than females and males, despite being the minority. The opposite is true for the males. i.e. Despite showing significantly high numbers, they on average rode for the shortest duration of time.
* The age groups with the most active bike riders are: Male: 41 - 50 years, Female: 51 - 60 years, Other: 31 - 40 years

## Key Insights for Presentation

* Distribution of gender
* Duration of trips per gender, plotted according to days of the week
* Distribution of user type
* Duration of trips per user type, plotted according to days of the week
* Duration of trips against age, when plotted according to days of the week
