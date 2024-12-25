# Yulu Bike Sharing Demand Prediction

## Project Overview
This project aims to predict the demand for bike-sharing services based on various environmental and temporal factors. The dataset contains detailed records of bike rentals, weather conditions, and temporal features. The insights and predictions from this project can help optimize bike availability and improve customer satisfaction.

---

## Dataset
The dataset used in this project contains 8760 rows and 14 columns, with no missing or duplicate values. Key features include:
- **Date**: The date of the record.
- **Rented_Bike_Count**: Number of bikes rented.
- **Hour**: Hour of the day.
- **Temperature**: Temperature (°C).
- **Humidity**: Humidity (%).
- **Wind_speed**: Wind speed (m/s).
- **Visibility**: Visibility (10m).
- **Dew_Point_Temperature**: Dew point temperature (°C).
- **Solar_Radiation**: Solar radiation (MJ/m²).
- **Rainfall**: Rainfall (mm).
- **Snowfall**: Snowfall (cm).
- **Seasons**: Season of the year.
- **Holiday**: Whether the day is a holiday.
- **Functioning_Day**: Whether the system was functioning that day.

---

## Data Preprocessing
1. Renamed columns for consistency and readability.
2. Converted the `Date` column to datetime format and extracted `year`, `month`, and `day`.
3. Created a new feature `weekday_or_weekend` based on the day of the week.
4. Encoded categorical columns (`Functioning_Day`, `Holiday`, and `weekday_or_weekend`) with binary values.
5. Applied Z-score standardization on numerical features for scaling.

---

## Feature Engineering
The following transformations and features were engineered:
- Encoded temporal and categorical columns.
- Transformed continuous variables using Z-score standardization.
- Focused on features such as month, day, temperature, and weather-related variables to capture demand patterns.

---

## Modeling
### Model Used
- **Multiple Linear Regression**

### Performance Metrics
- Mean Absolute Error (MAE): 0.16
- Mean Squared Error (MSE): 0.09
- Root Mean Squared Error (RMSE): 0.29
- R-squared: 0.91

These metrics indicate a strong predictive ability of the model to estimate bike-sharing demand.

---

## Hypothesis Testing
1. **Difference in Bike Rentals on Holidays vs. Non-Holidays**:
   - Significant difference found, impacting demand.
2. **Difference in Bike Rentals Across Seasons**:
   - Seasonality plays a significant role in bike-sharing demand.
3. **Impact of Temperature on Bike Rentals**:
   - Positive correlation observed between temperature and demand.

---

## Tools and Technologies
- **Programming Language**: Python
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
- **Environment**: Google Colab

---

## Key Visualizations
1. Correlation heatmaps to identify feature relationships.
2. Time series plots for seasonal demand trends.
3. Distribution plots for rental patterns across hours and days.

---



## Future Scope
1. Incorporate advanced models like Random Forest or XGBoost for improved predictions.
2. Explore real-time data integration for live demand forecasting.
3. Investigate external factors like public events or traffic patterns to enhance model accuracy.

---

## Contributors
- [Rahul Kumar](https://github.com/rahulkumar-24)

---



