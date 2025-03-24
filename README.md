# Air-Quality-Prediction

## Project Overview
Air pollution poses significant health risks, making air quality prediction essential for informed decision-making. This project leverages machine learning to predict Air Quality Index (AQI) trends using historical data from Washington, D.C. It provides insights into key pollutants influencing AQI and proposes an early warning system for deteriorating air conditions.

## Problem Statement
Urban air quality is impacted by various pollutants, including PM2.5, PM10, CO, NO₂, and O₃. Understanding how these pollutants contribute to AQI can help implement effective mitigation strategies. This project aims to analyze air quality data, engineer predictive features, and develop a machine learning model for accurate AQI forecasting.

## Dataset
**Source:** [Open Data DC](https://opendata.dc.gov/datasets/20c07bd1506249d4877ee45acfa73b71_76/explore)

**Description:**  
The dataset contains real-time air quality measurements from six monitoring sites in Washington, D.C. It includes pollutant concentration levels, timestamps, and site-specific details. Data preprocessing transforms the raw dataset into a structured format suitable for modeling.

## Project Workflow

### **1. Data Import, Exploration, and Cleaning**
- Load and inspect the dataset for missing values.
- Convert timestamps to datetime format.
- Pivot the dataset to represent pollutants as separate features.
- Perform exploratory data analysis (EDA) to understand pollutant distributions and correlations.

### **2. Data Transformation**
- Engineer cyclical time features (month, day, hour) for improved model performance.
- Implement geospatial mapping to visualize AQI across different sites.

### **3. AQI Calculation and Early Warning System**
- Compute AQI values for key pollutants using predefined breakpoints.
- Identify trends in AQI data through time-series analysis.
- Develop an early warning system to classify AQI levels (Normal, Caution, Warning, High Risk).

### **4. Model Training and Evaluation**
Several regression models are trained to predict AQI, including:
- Random Forest Regressor (Best Performing)
- Gradient Boosting Regressor
- Linear Regression
- Support Vector Regressor (SVR)  

Models are evaluated based on Mean Squared Error (MSE) and R-squared (R²) scores.

### **5. Air Quality Classification and Visualization**
- Classify AQI into categories such as Good, Moderate, and Unhealthy.
- Visualize pollutant contributions, feature importance, and AQI trends.
- Generate geospatial heatmaps for AQI levels across monitoring sites.

## Getting Started

### **Prerequisites**
- Python 3.6+
- Jupyter Notebook or Google Colab
- Required libraries: pandas, numpy, matplotlib, seaborn, scikit-learn, folium, plotly

### **Installation**
To install the required libraries, run:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn folium plotly
```

## Running the Project
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/Air-Quality-Prediction.git
    cd Air-Quality-Prediction
   ```
2. Open Air_Quality_Prediction.ipynb in Jupyter Notebook or Google Colab.
3. Run each cell sequentially to replicate the analysis.


## Conclusion
This project demonstrates the application of machine learning in air quality prediction. By identifying key pollutants contributing to AQI, implementing feature engineering techniques, and training robust models, it offers a data-driven approach to air quality assessment. The results can guide policymakers and researchers in mitigating air pollution effects.


## Acknowledgements
The dataset is sourced from Open Data DC. Special thanks to the contributors for making this data publicly available.

## License
This project is licensed under the MIT License.


