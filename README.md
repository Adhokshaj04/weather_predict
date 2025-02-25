# Weather or Not

## Overview
**Weather or Not** is a weather prediction system that empowers users to generate their own weather forecasts using historical climate data and machine learning models. Unlike traditional weather forecasting services, this project allows users to run models locally, providing more control over their predictions.

## Inspiration
The inspiration behind this project was my interest in the complex systems of weather forecasting and data science. I aimed to create an innovative system where users can manage and generate forecasts independently instead of relying solely on third-party services.

## Features
- **Historical Climate Data Processing**: Cleans and preprocesses NOAA climate data spanning two decades (2005-2025).
- **Feature Engineering**: Adds rolling averages and time-based variables to enhance predictions.
- **Machine Learning Forecasting**: Utilizes **Ridge Regression** to predict future weather conditions.
- **Model Storage & Accessibility**: Saves trained models as pickle files, allowing users to run their own predictions.
- **Front-end Integration (Planned)**: A mobile application to display forecasts and answer dynamic user queries.
- **API Development (Planned)**: Automate predictions through an API interface for real-time forecasting.

## How It Works
1. **Data Collection & Processing**  
   - Scraped climate data from the **National Oceanic and Atmospheric Administration (NOAA)** ([source](https://www.ncei.noaa.gov/cdo-web/)).
   - Cleaned missing or infinite values and structured the dataset for efficient modeling.
   - Extracted rolling averages and other key indicators to capture weather trends.
2. **Model Training**  
   - Implemented **Ridge Regression** to handle multicollinearity and enhance forecasting accuracy.
   - Evaluated model performance by comparing predictions with actual historical data.
3. **Model Deployment**  
   - Saved the trained model as a pickle file.
   - Provided an interactive interface for users to input weather parameters and generate forecasts.

## Challenges Faced
- **Conceptual Scope**: Balancing between two main ideas:  
  1. A **customizable mobile weather app** displaying user-preferred data.  
  2. An **interactive forecast assistant** answering quick weather-related queries.
- **Data Handling**: Managing missing/infinite values and structuring input features for better predictions.
- **System Integration**: Connecting the machine learning model from Google Colab with a front-end built in React.

## Accomplishments
- Successfully utilized **publicly accessible NOAA data** for local weather forecasting.
- Developed a **machine learning model** that produces reliable forecasts comparable to industry standards.
- Established a foundation for a **scalable weather prediction system** with potential for further improvements.

## Future Improvements
- **Enhance Model Accuracy**: Implement more complex models such as **XGBoost** or LSTM for time-series forecasting.
- **Expand Data Sources**: Incorporate additional weather parameters and satellite data.
- **Develop API & Web App**: Create a front-end system for user-friendly interaction.
- **Mobile Application**: Design an interactive mobile app for real-time personalized weather insights.

## Technologies Used
- **Python** (Data Processing & Modeling)
- **Google Colab** (Model Training & Prototyping)
- **NOAA Climate Data Online** [(Dataset Source)](https://www.ncei.noaa.gov/cdo-web/search)
- **Machine Learning** (Ridge Regression)
- **React (Planned)** (Front-end Development)
- **Flask (Planned)** (API Development)

## Dataset Information
The dataset used for this project consists of historical climate data collected from NOAA between **2005-2025**. It includes key weather variables such as:
- Temperature
- Humidity
- Wind Speed
- Precipitation
- Pressure

For detailed dataset documentation, refer to the **dataset file** included in this repository.

## Getting Started

### Requirements
```sh
- Python 3.x
- Pandas, NumPy, Scikit-learn, Matplotlib
- Jupyter Notebook / Google Colab
```

### Installation
```sh
# Clone the repository
git clone https://github.com/Adhokshaj04/weather_predict.git
cd weather_predict

# Install dependencies
pip install -r requirements.txt

# Run the model
python weather_forecast.py
```
