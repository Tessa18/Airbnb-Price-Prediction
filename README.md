# Airbnb-Price-Prediction
## Overview
This project aims to predict the price of Airbnb listings based on various features such as property attributes, amenities, and location. Using machine learning techniques, the model helps estimate rental prices, providing insights for both hosts and guests.

## Dataset
The dataset consists of Airbnb listing details, including:

-  **Numerical features**: Price-related attributes, review scores, and availability.
-  **Categorical features**: Room type, cancellation policy, and property type.
-  **Boolean features**: Cleaning fee, converted into binary values.
-  **Derived features**: Extracted from property descriptions to identify key amenities like Wi-Fi, parking, and breakfast.

## Data Preprocessing
-  **Handling Missing Values**: Imputing or dropping missing records.
-  **Feature Encoding**:

      **Label Encoding**: Applied to room_type, cancellation_policy, and recent_activity.

      **One-Hot Encoding**: Applied to categorical variables for better model compatibility.
-  **Feature Scaling**: Normalizing numerical variables to improve model performance.

## Feature Engineering
-  Extracting meaningful features from text data, such as identifying the presence of specific amenities using string matching.
-  Transforming test data using the same preprocessing steps as the training data.

## Modeling
The following machine learning models were implemented and compared based on RMSE (Root Mean Squared Error):

**1. Decision Tree Regressor** - Captures non-linear relationships in the data.

**2. Random Forest Regressor** - An ensemble method that improves prediction accuracy.

**3. XGBoost Regressor** - A gradient boosting algorithm that enhances performance using optimized tree-based learning.

## XGBoost Implementation Details
-  Used 1000 trees with a learning rate of 0.05.
-  Optimized using max depth of 8, subsample ratio of 0.8, and colsample_bytree of 0.8.
-  Evaluated using RMSE with validation monitoring.
-  Achieved improved performance over traditional tree-based models.

## Results & Insights
-  The models were evaluated based on RMSE (Root Mean Squared Error).
-  XGBoost demonstrated the best performance, reducing error compared to Decision Tree and Random Forest.
-  Feature importance analysis was conducted to determine the key drivers of price variation.

## How to Run the Project
1. Clone the repository:
-     git clone https://github.com/Tessa18/Airbnb_Price_Prediction.git
      cd Airbnb_Price_Prediction

2. Install the required dependencies:
-     pip install -r requirements.txt

3. Run the Jupyter Notebook:
-     jupyter notebook "Airbnb Price Prediction.ipynb"

## Future Improvements
-  Incorporate additional features like location-based data.
-  Experiment with deep learning models for improved predictions.
-  Deploy the model as a web-based price estimation tool.











