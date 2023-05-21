# Flight Price Prediction

This project focuses on predicting flight prices using machine learning techniques. It involves scraping flight data from a website, extracting relevant features, and training a model to make accurate price predictions. The goal is to help users estimate flight costs and make informed travel decisions.

## Project Overview

The project follows the following steps:

1. **Data Collection:** Flight data is scraped from a flights website using the Selenium library. The scraped information includes departure time, arrival time, day of the flight, flight duration, number of passengers, number of stops, and the timestamp of scraping. This data is stored in a structured format, such as a pandas DataFrame, for further analysis.

2. **Feature Engineering:** Additional features are derived from the available data to improve the predictive power of the model. The geolocator library is utilized to calculate the distance between the departure and arrival airports, which is then included as a feature in the DataFrame. Furthermore, the countries of the arrival airports are mapped to sub-regions in the world, allowing the determination of low, mid, or high seasonality on the flight date. This seasonality information is also added as a feature.

3. **Machine Learning Model:** After preprocessing the data and engineering the necessary features, a machine learning model is trained on the available dataset. Various algorithms and techniques, such as regression or ensemble methods, can be explored to achieve accurate flight price predictions. The model learns the patterns and relationships within the data to estimate flight prices based on the input features.

4. **Evaluation and Deployment:** The trained model is evaluated using appropriate evaluation metrics to assess its performance and generalization ability. The model's accuracy and predictive capabilities are assessed to ensure reliable flight price predictions. Once satisfied with the model's performance, it can be deployed to make predictions on new, unseen flight data.

## Project Structure

The project structure is organized as follows:

- `data/`: This directory contains the scraped flight data stored in a structured format, Excel.
- `notebooks/`: This directory contains Jupyter notebooks providing detailed explanations and step-by-step implementations of the project.
- `scripts/`: This directory contains Python scripts for data preprocessing, feature engineering, model training, and prediction.
- `models/`: This directory contains the trained machine learning models or serialized model objects.
- `requirements.txt`: This file lists the required Python libraries and versions to reproduce the project environment.

