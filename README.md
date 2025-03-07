# AQI Prediction using Machine Learning

This project focuses on predicting the Air Quality Index (AQI) using machine learning models. The dataset undergoes data cleaning and preprocessing before training multiple models, including:

- **Linear Regression**
- **Polynomial Linear Regression**
- **Random Forest**
- **Gradient Boosting**

Among these, **Random Forest** was found to be the most effective model due to its high R-squared value and low Mean Squared Error (MSE) compared to the others.

## Dataset
- **Source:** Public air quality monitoring data (`city_day.csv`).
- Contains air quality parameters also known as 'Pollutants' such as PM2.5, PM10, NO, NOX, CO, NO2, SO2, O3, Benzene, Toluene, Xylene.


## Features
- **Real-time AQI Prediction** using trained models
- **Data Preprocessing** for handling missing values and outliers
- **Model Training & Evaluation** to select the best-performing algorithm
- **Integration with WAQI API** to fetch real-time air quality data for any major stations/cities

## Technologies Used
- **Python** (pandas, numpy, scikit-learn, matplotlib, seaborn, xgboost, lightgbm, pickle )
- **Machine Learning Models** (Random Forest, Gradient Boosting, etc.)
- **Jupyter Notebook** for model development
- **WAQI API** for real-time AQI data retrieval

## Model Training & Selection
- The `Air_Quality_Prediction` notebook handles data cleaning and model training.
- The final trained Random Forest model is saved as `random_forest_model.pkl`.
- Other models can also be used for evaluation and comparison based on any feature selection.

## Real-Time AQI Prediction
By integrating with the **WAQI Weather API**, the trained model can predict AQI for major cities in real-time with high accuracy.

## Flow Diagram

![Flow Diagram](images/Diagram.png)


## Installation

### 1. Clone the Repository

    git clone https://github.com/yourusername/aqi-predictor.git
    cd aqi-predictor

### 2. Install Dependencies
#### Python Requirements
    pip install -r requirements.txt

#### Enable Git LFS for Large Model Files
    git lfs install
    git lfs track "*.pkl"
    git add .gitattributes

### 3. Get API Keys

    WAQI API: Sign up at WAQI to get an API key.
    Replace API_TOKEN in Air_Quality_prediction.ipynb.
    

## Deployment

This project can be deployed using:
   
    Render with gunicorn -w 4 -b 0.0.0.0:$PORT aqi_predictor:app


## Future Enhancements
- Implement deep learning models for improved accuracy.
- Develop a web-based dashboard for real-time AQI monitoring.
- Introduce IoT-based real-time data collection.

## Contact
For queries or contributions, feel free to reach out or create an issue in the repository.

