# NYC-Taxi-Trip-Time-Prediction
Predicting NYC Taxi Trip Duration 

The competition dataset is based on the 2016 NYC Yellow Cab trip record data made available in Big Query on Google Cloud Platform. The data was originally published by the NYC Taxi and Limousine Commission (TLC). The data was sampled and cleaned for the purposes of this playground competition. Based on individual trip attributes, participants should predict the duration of each trip in the test set.

Data fields

id - a unique identifier for each trip

**vendor_id **- a code indicating the provider associated with the trip record

pickup_datetime - date and time when the meter was engaged

dropoff_datetime - date and time when the meter was disengaged

passenger_count - the number of passengers in the vehicle (driver entered value)

pickup_longitude - the longitude where the meter was engaged

pickup_latitude - the latitude where the meter was engaged

dropoff_longitude - the longitude where the meter was disengaged

dropoff_latitude - the latitude where the meter was disengaged

store_and_fwd_flag - This flag indicates whether the trip record was held in vehicle memory before sending to the vendor because the vehicle did not have a connection to the

server - Y=store and forward; N=not a store and forward trip

trip_duration - duration of the trip in seconds

FAQ

Q: Why remove the outliers in the train data? Trips that are outside of the 99th quantile for trip length will unduly skew all of our numbers and results. Let's remove them. This will remove only 14593 out of the nearly 1.5 million trips from the train dataset.

Some of the trips might have a high extremely trip duration. When we check those points, some of the passengers are traveling into the Atlantic ocean. Not only are these points outliers, they also probably don’t correspond to real travel information. By cutting out extremal values, we can train a regressor that is a better fit for most values.

Q: Why is dropoff_datetime present in the train data but not in the test data? According to the Kaggle website:

The decision was made to not remove dropoff coordinates from the dataset order to provide an expanded set of variables to use in Kernels.

Since the dropoff_datetime was not present in the test dataset, we removed it. It also doesn’t make sense to use it since a taxi driver wouldn’t necessarily know how long a trip when picking someone up.

Q: What is drop_contains? It is a list of strings which will tell DFS to drop any features which match the strings.

Q: Why is trips.test_data in drop_contains? We don't want any features to be generated on the test_data column. The column is simply there to differentiate between train and test data. By putting the entity, followed by a dot, and the column name, it tell DFS to drop any aggregation features of test_data. If we had put just test_data in drop_contains, then it would have dropped the test_data column and the aggregation features of test_data.

Q: What is the model being used? XGBoost, which stands for eXtreme Gradient Boosting, is the model used. It is a very popular machine learning algorithm in Kaggle competitions for structured or tabular data. More infromation can be found here.
