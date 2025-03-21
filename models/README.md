# Models Directory

This directory contains our trained machine learning models for agricultural production forecasting.

## Model Files
- **random_forest_model.pkl**: Our advanced Random Forest model for production prediction (R² score: 0.85)
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

## Model Usage
These models can be loaded using joblib in Python:

```python
import joblib

# Load the Random Forest model
rf_model = joblib.load("random_forest_model.pkl")

# Load the crop production model
crop_model = joblib.load("crop_production_model.pkl")

# Load label encoders
le_state = joblib.load("label_encoder_state.pkl")
le_crop = joblib.load("label_encoder_crop.pkl")

# Example: Encoding new data
state_encoded = le_state.transform(["Maharashtra"])
crop_encoded = le_crop.transform(["Rice"])

# Make predictions with the model
predictions = rf_model.predict(X_test)
