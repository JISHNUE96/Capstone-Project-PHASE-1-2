# PHASE-1&2
Capstone Project Phase 1 & 2 (Data Collection,Data Preprocessing, EDA, Feature Engineering, Feature Selection,Split Data into Training and Testing Sets, Feature Scaling, Build the ML Model , Model Evaluation)

Machine Learning Project: Taiwan Air Quality Index Data

Project Overview: This project involves analyzing the Taiwan Air Quality Index (AQI) dataset to understand the trends in air quality and identify the relationship between various pollutants such as PM2.5, CO, SO2, and others. The primary goal is to predict the AQI levels based on concentrations of these pollutants using regression analysis techniques. The dataset spans from 2016 to 2024, offering a comprehensive view of Taiwan's air quality over time.

Problem Statement: The project aims to forecast the Air Quality Index (AQI) for various regions in Taiwan and predict pollutant levels, particularly PM2.5, based on historical data. This would assist in improving air quality management and provide insights into the factors affecting air quality. Regression techniques will be employed to model the relationship between AQI and pollutant levels, thereby predicting air quality for future time periods.

Project Objective:
Forecast the Air Quality Index (AQI) based on the levels of specific pollutants.
Predict PM2.5 levels and their impact on air quality.

Dataset: The dataset for this analysis is publicly available on the Kaggle ML Repository at the following link :- https://www.kaggle.com/datasets/taweilo/taiwan-air-quality-data-20162024

Data Description:
The dataset contains multiple features that represent different aspects of air quality measurements at various monitoring stations across Taiwan. Below is a summary of the dataset’s key features:

Source: Taiwan Air Quality Index Data (Kaggle)
Dataset Features: The dataset initially contains 1,048,576 rows, representing extensive air quality data. For the analysis, the data was sorted to focus on one month’s data, reducing it to 62,964 rows for more manageable processing. Below are the features in the dataset:
Date: Date and time of the reading (Text).
Sitename: Name of the monitoring station (Text).
County: County or city (Text).
AQI: Air Quality Index (Numeric).
Pollutants: Various air pollutants measured in different units such as SO2, CO, O3, PM10, PM2.5, NO2, NOx, NO (Numeric).
Wind Speed & Direction: Meteorological data for wind (Numeric).
Average Pollutant Levels: Moving averages for pollutants such as PM2.5, PM10, SO2, CO, etc. (Numeric).
Geographical Coordinates: Latitude and longitude of the monitoring station (Numeric).
Station ID: Unique identifier for the station (Numeric).

Data Collection:
The dataset is imported from Kaggle, containing comprehensive air quality readings collected from various monitoring stations across Taiwan over the period from 2016 to 2024. The first step in the project involves loading and exploring the dataset to understand its structure and identify distribution patterns.

Data Preprocessing & Cleaning:
Handling Missing Values: Address missing values using appropriate imputation techniques such as mean or KNN imputation.
Outlier Detection: Detect and handle outliers using statistical methods (e.g., Z-scores, IQR).
Data Transformation: Normalize skewed numerical features using logarithmic or other transformations to improve model performance.

Exploratory Data Analysis (EDA):
Gain deeper insights into the dataset through visualizations and statistical analysis.
Visualizations:
Histograms and KDE plots to analyze feature distributions.
Boxplots to identify outliers.
Heatmaps to evaluate feature correlations.
Pair plots for feature relationships.
Bar and line plots for pollutant trends.

Feature Engineering and Selection:
Encoding Categorical Data: Apply one-hot or label encoding to categorical variables such as sitename, county, and status.
Feature Importance: Use algorithms like Random Forest to rank features based on their importance.
Select K Best: Apply statistical tests to choose the most significant features for model building.

Model Building Process:
Split Data: Divide the dataset into training and testing sets to evaluate model performance.
Feature Scaling: Normalize data using techniques like Min-Max Scaling or Standard Scaling to ensure uniformity across features.
Build the ML Model: Train regression models, including Linear Regression, Decision Trees, and Random Forest, to predict AQI and PM2.5 levels.
Model Evaluation: Use metrics such as RMSE (Root Mean Squared Error) and MAE (Mean Absolute Error) to assess the accuracy and performance of the models.

Conclusion:

The project successfully predicts AQI levels using pollutant concentrations as inputs. By leveraging regression techniques, the model identifies the key factors impacting air quality and provides accurate forecasts. This analysis can support environmental policymakers, public health officials, and researchers in taking proactive measures to improve air quality and public health outcomes.
