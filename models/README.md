# Models Directory

This directory describes our trained machine learning models for agricultural production forecasting.

## Model Files (Not Included in Repository)
Due to GitHub's file size limitations, the following model files are not included in this repository:

- **random_forest_model.pkl** (1.3GB): Our advanced Random Forest model for production prediction (R² score: 0.85)
- **crop_production_model.pkl**: Specialized model for crop production forecasting with regional calibration
- **label_encoder_state.pkl**: Label encoder for transforming state names into numeric format
- **label_encoder_crop.pkl**: Label encoder for transforming crop types into numeric format

## Model Performance
- **Baseline Model (Linear Regression)**:
  - RMSE: 15,304,310.01
  - MAE: 1,182,554.75
  - R² Score: 0.16
  
- **Advanced Model (Random Forest)**:
  - RMSE: 6,443,694.69
  - MAE: 245,958.54
  - R² Score: 0.85

## Model Implementation
The models can be recreated using the code in our notebook:
- See `notebooks/impactx-agriculture.ipynb` Cell 6 for the Random Forest implementation
- The model uses 100 estimators with default parameters
- Label encoders are created for State, District, Season, and Crop variables

## Additional Files
For model evaluation and recommendations, see:
- **model_performance.csv**: Detailed metrics on model performance
- **crop_recommendations.csv**: Generated crop recommendations by region
