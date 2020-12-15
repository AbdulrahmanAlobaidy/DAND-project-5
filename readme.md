# (Data Analysis and Visualization)
## by (Abdulrahman Mohammed Alobaidy)


## Dataset

This data set contains information about the **Ford Go** bike-sharing system, the dataset contains data points a little more than 180,000 data points for the month of February of the year 2019.

### Dataset Features

The dataset consists of the following 16 features:
* `duration_sec`: Duration of the trip.
* `start_time`: Timestamp of the start of the trip.
* `end_time`: Timestamp of the start of the trip.
* `start_station_id`: ID of the start station.
* `start_station_name`: Name of the start station.
* `start_station_latitude`, `start_station_longitude`: Coordinates  of the start station.
* `end_station_id`: ID of the end station.
* `end_station_name`: Name of the end station.
* `end_station_latitude`, `end_station_longitude`: Coordinates  of the end station.
* `bike_id`: ID of the bike used.
* `user_type`: Type of user, Subscriber or Customer.
* `member_birth_year`: Year of birth of user.
* `member_gender`: Gender of the user.
* `bike_share_for_all_trip`: Whether the bike was part of the **Bike Share For All** program.

The cleaned version of the dataset contains these 6 additional engineered features:
* `duration_hour`: `duration_sec` converted to hour-format.
* `duration_min`: `duration_sec` converted to minute-format.
* `hour-of-day`: Extracted from `start_time`.
* `user_age`: Extracted from the `member_birth_year` column, i.e. current year minus the year in the `member_birht_year`.
* `age_range`: `user_age` categorized into age bins of 10 using this format [start, end).
* `route`: Route of trip, (`start_station_name` -> `end_station_name`).


### Features of Interest

The following is a list of the features of interest, i.e. the features that we will be focusing on and analyzing, along with extracted and enigneered ones which are present in the cleaned dataset, classified into either **Quantitative** or **Qualitative**:
1. **Quantitative**:
    * `duration_min`
    * `hour_of_day`
    * `user_age`
2. **Qualitative**:
    * `start_station_name`
    * `end_station_name`
    * `route`
    * `user_type`
    * `age_range`
    * `member_gender`
    * `bike_share_for_all_trip`


## Summary of Findings

The following points are the results of the exploration process:

* The bulk of the time spent was in the 5 to 10-minute range.

* We notice that the heighest usage hour was in the 8 o'clock in the morning as well as the 5 o'clock in the afternoon, which suggests that probably most of the users are using the service to commute to work.

* We notice that the bulk of our users are in the age range of 20 to 40 years of age.

* **91%** of the users are **Subscribers** and **9%** are **Customers**.

* Males constitute three quarters of the dataset, while females constitute 23% and 2% for Others.

* **90%** of the bikes are **not** part of a bike sharing program, while **10%** are.

* The 20 most used start stations make up about **25%** of the total trips count.

* The 20 most used end stations make up about **27%** of the total trips count.

* The 20 most used routes make up about **3%** of the total trips count.

* We notice that most of the data points are concentrated in the duration of 5 to 15 minutes for users within age range of 20 to 40 years old.

* Males have a higher median than females when it comes to user ages, but not by too much.

* Females have a higher median than males when it comes to ride duration by not much.

* Users of both types, Subscribers and Customers, both have about the same median when it comes to age, but customers have a higher median when it comes to duration.

* Gender count for subscribers is obviously higher for all genders than for customers, which makes sense since **91%** of users are Subscribers.

* As for the bike-sharing program, the majority of the gender count goes to the **No** criteria, this makes sense since **90%** of the bikes are not enrolled in such program.

* The highest average duration taken by a male age group was that of age range 60-70 with 12 minutes, followed by 10-20 and 70-80 years with about 11 minutes.

* As for females, the age group with the highest duration was the group with age range 10-20 with an average duration of about 15 minutes, followed by the 60-70 age group with a duration of about 12 minutes, with no female datapoints for ages greater than 90.

* There are no users of type customers with bike-share programs.

* Gender count was almost the same with users that are subscribers using bikes that are part of bike-sharing program and users that are customers using bikes that are not a part of bike-sharing program.

* The bulk of the gender counts where users that are subscribers and not using a bike-sharing program bike.

* For the facet grid that subsets the heatmaps of age versus duration by gender and user type, we notice that the data is concentrated in about the same place, but with small shifts for the center, for example, we notice that duration for females who are customers is higher than for females .who are subscribers, we also notice that males who are subscribers take the age range of about 25 to 35 years, while those who are customers take the age range of 30 to 35 years.



## Key Insights for Presentation

The main points that where passed on to presentation where the following:

* The bulk of the time spent was in the 5 to 10-minute range.

* We notice that the heighest usage hour was in the 8 o'clock in the morning as well as the 5 o'clock in the afternoon, which suggests that probably most of the users are using the service to commute to work.

* We notice that the bulk of our users are in the age range of 20 to 40 years of age.

* **91%** of the users are **Subscribers** and **9%** are **Customers**.

* Males constitute three quarters of the dataset, while females constitute 23% and 2% for Others.

* **90%** of the bikes are **not** part of a bike sharing program, while **10%** are.

* The 20 most used start stations make up about **25%** of the total trips count.

* The 20 most used end stations make up about **27%** of the total trips count.

* The 20 most used routes make up about **3%** of the total trips count.

* We notice that most of the data points are concentrated in the duration of 5 to 15 minutes for users within age range of 20 to 40 years old.

* Males have a higher median than females when it comes to user ages, but not by too much.

* Females have a higher median than males when it comes to ride duration by not much.

* Users of both types, Subscribers and Customers, both have about the same median when it comes to age, but customers have a higher median when it comes to duration.