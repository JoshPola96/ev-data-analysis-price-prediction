# Electric Vehicle Data Analysis and Price Prediction

## Project Overview
This project analyzes electric vehicle (EV) registration data to explore trends, characteristics, and predict future pricing and range capabilities. Using machine learning techniques including neural networks and clustering algorithms, the project provides insights into the evolving EV market landscape.

## Key Features
- **Comprehensive Data Analysis** of EV registrations with visualizations of trends and distributions
- **Advanced Neural Network Model** with BatchNormalization and Dropout layers for predicting future EV prices and ranges
- **Bayesian Hyperparameter Optimization** to tune model architecture and learning parameters
- **DBSCAN Clustering** with parameter grid search to identify optimal vehicle groupings
- **Multi-dimensional Visualizations** showing relationships between vehicle characteristics

## Data
The analysis uses the "Electric Vehicle Population Data" dataset containing registration information including:
- Vehicle make, model, and year
- EV type (Battery Electric or Plug-in Hybrid)
- Electric range and price (MSRP)
- Geographic location data (county, city, coordinates)
- Clean Alternative Fuel Vehicle (CAFV) eligibility status

## Technical Implementation

### Data Preprocessing
- Coordinate extraction from vehicle location data using regex pattern matching
- Handling of missing values and data type conversion
- Feature engineering for model preparation including categorical encoding
- Data normalization using MinMaxScaler for price and range prediction

### Exploratory Data Analysis
- Visualization of EV adoption trends over time using sequential plots
- Analysis of top manufacturers and models by electric range
- Geographic distribution analysis by county and city
- Growth rate calculation for year-over-year comparisons
- Correlation analysis between numerical features

### Neural Network Architecture
- Implementation of a deep neural network using TensorFlow and Keras
- Dynamic layer configuration with BatchNormalization for training stability
- Dropout layers to prevent overfitting
- Multiple hidden layers with optimized activation functions
- Hyperparameter optimization using Keras Tuner with Bayesian approach
- Early stopping and learning rate scheduling for optimal convergence
- Multi-output regression model predicting both price and range simultaneously

### Clustering Analysis
- DBSCAN algorithm implementation with scikit-learn pipelines
- Parameter grid search for optimal eps and min_samples values
- Column transformer for mixed data type preprocessing
- Multi-dimensional visualization of clusters (2D and 3D plots)
- Geographic clustering visualization using coordinate data

## Results and Insights
- Identified significant growth trends in EV adoption across specific regions
- Established correlations between vehicle attributes, most notably price and range
- Forecasted future price and range trends for different vehicle types through 2030
- Discovered distinct vehicle segments through unsupervised learning
- Created ranking scores to identify top-performing models based on price-to-range ratio

## Technologies Used
- **Python** for data processing and analysis
- **Pandas & NumPy** for data manipulation
- **Matplotlib & Seaborn** for data visualization
- **TensorFlow & Keras** for deep learning model development
- **Keras Tuner** for hyperparameter optimization
- **Scikit-learn** for preprocessing, model evaluation, and clustering algorithms

## Acknowledgements
Data source: Electric Vehicle Population Data
