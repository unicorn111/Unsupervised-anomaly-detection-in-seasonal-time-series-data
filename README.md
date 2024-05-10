# Unsupervised-anomaly-detection-in-seasonal-time-series-data


This repository is part of a bachelor thesis, "Unsupervised anomaly detection in seasonal time series data." It consists of two folders – data and models, and two jupyter notebooks – preliminary_research.ipynb and proposed_solution.ipynb.


**data**<br />
The data folder contains our artificially generated seasonal_time_series_for_anomaly_detection dataset, which consists of
13 CSV files with ordered, timestamped, single-valued metrics and 1 CSV from the NAB dataset. The full description can be found in the data folder.

**models**<br /> 
The models folder contains 8 trained models in the .hdf5 format. Each model name represents the data on which it was trained.


**preliminary_research.ipynb**<br /> 
This notebook contains the implementation of anomaly detection using  STL, Isolation Forest, k-means, Autoencoders, and median-based sliding window. There are plots that show the detected anomalies.

**proposed_solution.ipynb**<br /> 
This notebook contains the implementation of our proposed solution of anomaly detection based on Autoencoders. There are plots that show the stages of work of the proposed solution and detected anomalies.
