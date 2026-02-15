# Household-Electricity-Peak-Forecastingroject Overview
This project focuses on forecasting household electricity consumption to identify peak demand periods. By predicting these peaks, we can recommend shifting usage to off-peak times, which reduces grid strain, lowers operational costs, and promotes sustainable energy management.


Dataset: 
I have used the Individual Household Electric Power Consumption dataset from the UCI Machine Learning Repository.
Size: ~2 million records.
Duration: Nearly four years of data (2006–2010).
Features: Global Active Power, Voltage, Global Intensity, and specific Sub-metering for kitchen, laundry, and climate control.


Tech Stack & Preprocessing :
Libraries: Scikit-learn, TensorFlow/Keras, Pandas, Matplotlib.
Workflow:
Missing value handling via time-based interpolation.
Outlier detection and capping using the IQR method.
Feature Engineering (Lag features, rolling statistics, and time-based features).
Dimensionality reduction using PCA.
Log transformation and Min-Max scaling.

Models & Results: 
Random Forest Regressor - 0.010209 (RMSE) |	0.005457(MAE) |	0.998542(R²)
Decision Tree           - 0.012301 (RMSE) |	0.006804(MAE) |	0.997883(R²)
SVR	                    - 0.012696 (RMSE) |	0.008211(MAE) |	0.997745(R²)
LSTM	                  - 0.014818 (RMSE) |	0.010035(MAE) |	0.996950(R²)
KNN	                    - 0.051599 (RMSE) |	0.032965(MAE) |	0.962756(R²)
