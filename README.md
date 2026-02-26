# Analysing-Tropospheric-Formaldehyde-HCHO-gas-in-Sri-Lanka
Analysing HCHO data from popular Sri Lankan cities, to understand air quality issues and promoting sustainable  development practices.

The main objectives are to understand the importance of HCHO monitoring, develop insights into potential sources and spatio-temporal trends, and develop time series prediction algorithms.

Key sections and findings include:
Data Preprocessing (Part 2):
Pandas was chosen as the framework for preprocessing the dataset of 12,779 datapoints.
The three initial datasets for Colombo Proper, Deniyaya, Matara, Nuwara Eliya Proper; Kandy Proper; and Bibile, Monaragala, Kurunegala Proper, and Jaffna Proper were merged into a single dataframe, 'df_sl_cities'.
Missing HCHO values (4,863 null values in the merged dataset) were handled using the Interpolation method, grouped by location.
Statistical analysis showed Colombo Proper had the highest mean HCHO reading (0.000154), and Nuwara Eliya Proper had the lowest (0.000082).
Spatio-Temporal Analysis (Part 3):
The average HCHO readings were lower for most cities during the assumed COVID-19 lockdown period (2020-03-12 to 2021-12-31).
Correlation analysis with external factors (Precipitation, Temperature_avg, and Elevation) for Colombo Proper, Kurunegala Proper, and Nuwara Eliya Proper suggested:
HCHO reading was higher when Precipitation was lower (weak negative correlation).
HCHO reading was higher when Average Temperature was higher (weak positive correlation).
HCHO reading was higher when Elevation was lower.
Machine Learning (Part 4):
SARIMAX models were used for time series forecasting for each location.
The models for each city showed Mean Absolute Error and Mean Squared Error values very close to zero, indicating accurate value predictions, and were forecasted for the next 30 days.
