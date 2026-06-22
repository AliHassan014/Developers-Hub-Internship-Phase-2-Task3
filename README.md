# Developers-Hub-Internship-Phase-2-Task3
Objective
Parse and preprocess time series energy data
Resample data for hourly forecasting
Engineer time-based features (hour, day, weekday, weekend)
Apply ARIMA, Prophet, and XGBoost models
Compare model performance using RMSE
Visualize actual vs predicted energy usage
 Dataset

Household Power Consumption Dataset

Key Features:
Global_active_power
Global_reactive_power
Voltage
Global_intensity
Sub_metering_1, Sub_metering_2, Sub_metering_3
Technologies Used
Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn
Statsmodels (ARIMA)
Prophet (Meta)
XGBoost
Workflow
1. Data Loading & Preprocessing
Loaded CSV dataset
Parsed Date and Time into a single DateTime index
Converted data types to numeric
Handled missing values
2. Time Series Resampling
Resampled data into hourly averages
Selected Global_active_power as target variable
3. Feature Engineering
Extracted time-based features:
Hour
Day
Month
Day of Week
Weekend indicator
Created lag features for ML models
4. ARIMA Model
Built statistical time series model
Forecasted future energy consumption
Evaluated using RMSE
5. Prophet Model
Converted data into ds and y format
Modeled trend and seasonality
Generated future forecasts
6. XGBoost Model
Converted time series into supervised learning problem
Used lag + time features
Trained regression model for forecasting
7. Model Evaluation
Compared models using RMSE (Root Mean Squared Error)
Visualized actual vs predicted values
 Results
ARIMA: Baseline statistical performance
Prophet: Good handling of trends and seasonality
XGBoost: Best performance for complex nonlinear patterns
 Visualization
Time series plots of energy consumption
Actual vs predicted comparisons for all models
RMSE comparison bar chart
 How to Run
Download dataset
Open Jupyter Notebook
Install required libraries:
pip install pandas numpy matplotlib seaborn scikit-learn statsmodels prophet xgboost
Run notebook step by step
 Conclusion

This project demonstrates that energy consumption forecasting can be effectively modeled using both statistical and machine learning approaches. Among the tested models, XGBoost provides the most accurate predictions due to its ability to capture complex patterns, while Prophet offers strong performance in trend and seasonality modeling.
