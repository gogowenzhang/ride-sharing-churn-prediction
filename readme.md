## Ride Sharing Churn Prediction

A ride-sharing company (Company X) is interested in predicting rider retention.
A cohort of users who signed up for an account in January 2014 were included. 
The data was pulled on July 1, 2014; a user were considered retained if they were “active” (i.e. took a trip) in the preceding 30 days (from the day the data was pulled). In other words, a
user is "active" if they have taken a trip since June 1, 2014. The data,
`churn.csv`, is in the [data](data) folder.  The data are split into train and
test sets.  


### Description of the data:

- `city`: city this user signed up in phone: primary device for this user
- `signup_date`: date of account registration; in the form `YYYYMMDD`
- `last_trip_date`: the last time this user completed a trip; in the form `YYYYMMDD`
- `avg_dist`: the average distance (in miles) per trip taken in the first 30 days after signup
- `avg_rating_by_driver`: the rider’s average rating over all of their trips 
- `avg_rating_of_driver`: the rider’s average rating of their drivers over all of their trips 
- `surge_pct`: the percent of trips taken with surge multiplier > 1 
- `avg_surge`: The average surge multiplier over all of this user’s trips 
- `trips_in_first_30_days`: the number of trips this user took in the first 30 days after signing up 
- `luxury_car_user`: TRUE if the user took a luxury car in their first 30 days; FALSE otherwise 
- `weekday_pct`: the percent of the user’s trips occurring during a weekday


### Workflow:
1. Perform any cleaning, exploratory analysis, and/or visualizations to use the provided data for this analysis.
2. Build a predictive model to help determine the probability that a rider will be retained.
3. Evaluate the model. Focus on metrics that are important for the statistical model.
4. Identify / interpret features that are the most influential in affecting the predictions.
5. Discuss the validity of the model. Issues such as leakage. For more on leakage, see this essay on Kaggle, and this paper: Leakage in Data Mining: Formulation, Detection, and Avoidance.
6. Repeat 2 - 5 until find the best model.
7. Consider business decisions that the model may indicate are appropriate. Evaluate possible decisions with metrics that are appropriate for decision rules.
