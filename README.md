# AQI Prediction using Machine Learning

This project focuses on predicting the Air Quality Index (AQI) using machine learning models. The dataset undergoes data cleaning and preprocessing before training multiple models, including:

- **Linear Regression**
- **Polynomial Linear Regression**
- **Random Forest**
- **Gradient Boosting**

Among these, **Random Forest** was found to be the most effective model due to its high R-squared value and low Mean Squared Error (MSE) compared to the others.

## Features
- **Real-time AQI Prediction** using trained models
- **Data Preprocessing** for handling missing values and outliers
- **Model Training & Evaluation** to select the best-performing algorithm
- **Integration with WAQI API** to fetch real-time air quality data

## Technologies Used
- **Python** (pandas, numpy, scikit-learn, matplotlib, seaborn)
- **Machine Learning Models** (Random Forest, Gradient Boosting, etc.)
- **Jupyter Notebook** for model development
- **WAQI API** for real-time AQI data retrieval

## Model Training & Selection
- The `Air_Quality_Prediction` notebook handles data cleaning and model training.
- The final trained Random Forest model is saved as `random_forest_model.pkl`.
- Other models can also be used for evaluation and comparison.

## Real-Time AQI Prediction
By integrating with the **WAQI Weather API**, the trained model can predict AQI for major cities in real-time with high accuracy.

## Using Pretrained Model
In order to run the model directly without going through the preprocessing and training phase, the Random Forest model can be downloaded from the repository releases:  
[Pretrained Model Download](https://github.com/AlwaysRead/AQI-Predictor/releases/tag/v1.0)  
and used directly as pretrained data.

## Dataset
- **Source:** Public air quality monitoring data (`city_day.csv`).
- Contains air quality parameters such as PM2.5, PM10, CO, NO2, SO2, and O3.

## Future Enhancements
- Implement deep learning models for improved accuracy.
- Develop a web-based dashboard for real-time AQI monitoring.
- Introduce IoT-based real-time data collection.

## Contact
For queries or contributions, feel free to reach out or create an issue in the repository.

