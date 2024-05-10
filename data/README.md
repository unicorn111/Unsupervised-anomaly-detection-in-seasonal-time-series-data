**seasonal_time_series_for_anomaly_detection**


This dataset contains seven CSV files with artificially generated, ordered, timestamped, single-valued metrics for three months divided by days of the week with no anomalies. Also, three CSV files are artificially generated, ordered, timestamped, and have single-valued metrics with anomalies, and two CSV files have a week representation (one with anomalies). Finally, it has one file with artificially generated, ordered, timestamped, single-valued metrics for three months.

Motivation<br />
This dataset was created as a part of a bachelor's thesis. Our proposed solution suggests dividing time series data based on its periodicity and training an auto-encoder model for each period for anomaly detection. For these needs, we decided to create this dataset based on the NAB dataset.

Composition<br />
Our dataset consists of two columns: timestamp and value. The timestamp column is represented by a date in the format "%Y-%m-%d %H:%M:%S" with a five-minute time interval. The value column is represented by a positive number. This dataset contains 67.7k rows in total. Each week's day CSV contains 3745 rows. Two CSV's containing weekly data have 2017 rows each. There are no missing values in this dataset. All weekday CSVs and weekly with no anomalies are meant for training; the rest with anomalies are meant for testing. This dataset was created based on the NAB dataset https://github.com/numenta/NAB/tree/v1.1/data

Generation process<br />
Dates were generated for January, February, and March of 2024; values were used from the NAB dataset but modified to show the seasonality of a week.

Uses<br />
This dataset was used in "Unsupervised anomaly detection in seasonal time series data" bachelor thesis for training auto-encoders and testing anomaly detection using auto-encoders. Precisely, art_monday.csv, art_tuesday.csv, art_wednesday.csv, art_thursday.csv, art_friday.csv, art_saturday.csv, art_sunday.csv, art_normal_week were used for training autoencoders and art_monday_collective_anomaly_down, art_wednesday_collective_anomaly_up.csv, art_saturday_point_anomaly.csv, art_anomaly_week.csv were used for data predicion. Even though this dataset was created for auto-encoders, it can be used for any anomaly detection techniques.

art_daily_jumpsup.csv is a part of the NAB dataset
