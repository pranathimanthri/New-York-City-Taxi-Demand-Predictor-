# NYC Taxi Demand Predictor

## Introduction

The NYC Taxi Demand Predictor project utilizes historical taxi trip data combined with weather information to forecast taxi demand across New York City. By accurately predicting demand, the project aims to optimize taxi fleet management, reduce operational costs, and contribute to improved urban mobility and planning. This initiative supports data-driven decision-making in one of the busiest transportation networks in the United States.

## Project Objectives

The primary objective of this project is to develop predictive models that estimate taxi ride demand on an hourly basis. This includes enhancing the accuracy of forecasts by integrating diverse datasets, such as historical taxi trip records and real-time weather data. By identifying demand trends and patterns, the project also seeks to inform taxi companies and city planners on effective fleet allocation and urban infrastructure management.

## Data Collection and Preprocessing

Data for this project was collected from the New York City Taxi & Limousine Commission (TLC) and a dedicated Weather API. Historical trip data, specifically for Yellow Taxi services during January to March 2023, was extracted using Python libraries such as `requests` and `Beautiful Soup`. In parallel, weather data—including temperature, precipitation, wind speed, and visibility—was gathered to understand its influence on taxi demand. After extraction, the raw data was cleaned by parsing time fields, removing invalid entries, and calculating new features like trip duration and average speed. This meticulous preprocessing ensured that the dataset was robust and ready for subsequent analysis and modeling.

## Exploratory Data Analysis (EDA)

In the exploratory data analysis phase, the project team examined various aspects of taxi usage patterns. The analysis focused on understanding passenger count distributions, payment methods, trip durations, and average speeds. Detailed temporal analyses were conducted to identify hourly, daily, and monthly demand trends. Visual tools such as histograms and time-series graphs were employed to detect outliers and understand the underlying patterns, offering crucial insights into urban travel behavior and demand fluctuations throughout the day and week.

## Feature Engineering

Feature engineering played a pivotal role in transforming raw data into a format suitable for predictive modeling. The process involved creating new attributes such as the duration of each taxi ride and calculating the average speed per trip. Additionally, time-based features (e.g., hour, day of the week, and month) were derived to capture temporal trends in taxi demand. The integration of weather data with taxi trip records further enriched the dataset, enabling a more nuanced analysis of how environmental factors affect travel patterns.

## Predictive Modeling

The predictive modeling stage involved implementing and comparing several machine learning algorithms to forecast taxi demand. Four regression techniques were used in this project: XGBoost, LightGBM, CatBoost, and AdaBoostRegressor. Each model was trained using a carefully prepared dataset that included historical demand metrics and weather conditions. Among the models, CatBoost demonstrated the best performance with a Mean Absolute Error (MAE) of 1.5315. LightGBM and XGBoost also performed well, while AdaBoostRegressor was found to be less effective for this particular dataset. The evaluation of these models provided insights into their strengths and limitations when applied to large, complex datasets.

## Results and Key Insights

The analysis revealed several key insights that can influence taxi fleet management and urban planning. Weather conditions, such as rain, snow, and extreme temperatures, were found to significantly impact taxi demand, with inclement weather leading to higher usage. Temporal patterns indicated that taxi demand peaks during the evening rush hours and remains relatively higher on weekdays compared to weekends. Additionally, the geographical distribution of taxi pickups identified demand hotspots across New York City, highlighting areas where taxis should be strategically pre-positioned. These findings underscore the value of integrating data analytics into operational planning and resource allocation in urban transportation.

## Future Improvements

Looking ahead, there are multiple avenues to further enhance the NYC Taxi Demand Predictor project. Future work could include integrating real-time traffic and weather updates to refine the accuracy of predictions. Expanding the dataset to incorporate additional factors—such as local events and public transport changes—could also provide a more comprehensive picture of taxi demand. Furthermore, exploring advanced machine learning and artificial intelligence techniques may yield even more accurate and robust predictive models.

## Technologies Used

This project is developed using Python and leverages several powerful libraries. Data extraction was performed using `requests` and `Beautiful Soup`, while data manipulation and analysis were carried out using `pandas`. For predictive modeling, machine learning libraries such as XGBoost, LightGBM, CatBoost, and AdaBoost were utilized. Visualization of data and model results was achieved through Matplotlib, providing clear graphical representations of the trends and patterns identified during the analysis.

