# Ford GO exploration
## by Juan Daniel Alonso Fernández


## Dataset

We have worked with 2019's data from Bay Wheels, (formerly Ford GO) extracted from [here](https://s3.amazonaws.com/baywheels-data/index.html)

We manually downloaded all 12 files for 2019 into our computer and then concatenated them into a DataFrame in Jupyter.

The dataset contains around, 2.5 million observations for which 15 different variables had been collected (Station information, travel duration, etc) on which we performed some cleaning before working with them (dropped unneeded columns, investigated missing values and changed datatypes)



## Summary of Findings


We have discovered that Bay Wheels rides tend to be short (95% of travels take less than 30 minutes) but the duration depends on the time of the year (longer rides in summer than in winter), the service offered (longer if stationless e-bikes are used) and the user type that rides (casual customers tend to have longer rides than Bay Wheels' members)

We saw as well that the year ended with bad results for the company and opened the question to analyze 2020's dataset in the future.


## Key Insights for Presentation

Our exploration first based on the search of a reason for the big number of Null values existing in station_id and station_name variables in July and August, once we realized that it was due to the introduction of stationless e-bikes and not due to an error, we started investigating the effect that business decisions had on the customer's bike usage.
The number of trips by subscribers is disproportionate on weekdays while customers seem to travel the same on weekdays as on weekends (72% is as well the number of workdays in the week)
