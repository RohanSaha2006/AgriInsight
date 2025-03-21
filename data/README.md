# Data Directory

This directory contains the datasets used in our agricultural data analysis.

## Datasets Included

### 1. Agricultural Production Dataset (APY)
- **File**: apy.csv
- **Size**: 15.32 MB (246,091 entries across 7 columns)
- **Source**: TRAIN-IT Hackathon 2025
- **Description**: State-wise, district-wise crop production statistics
- **Columns**:
  - State_Name: Name of the Indian state
  - District_Name: Name of the district
  - Crop_Year: Year of crop production
  - Season: Growing season (Kharif, Rabi, Whole Year, etc.)
  - Crop: Type of crop cultivated
  - Area: Area under cultivation (in hectares)
  - Production: Crop production (in metric tonnes)

### 2. Agricultural Commodity Price Dataset
- **File**: Price_Agriculture_commodities_Week.csv
- **Size**: 1.9 MB (23,093 entries across 10 columns)
- **Source**: TRAIN-IT Hackathon 2025
- **Description**: Market prices of various agricultural commodities
- **Columns**:
  - State: State name
  - District: District name
  - Market: Market name
  - Commodity: Agricultural commodity type
  - Variety: Specific variety of the commodity
  - Grade: Quality grade
  - Arrival_Date: Date of market arrival
  - Min_Price: Minimum price (₹)
  - Max_Price: Maximum price (₹)
  - Modal_Price: Most common price (₹)

## Data Preprocessing
Key preprocessing steps applied to these datasets:
1. Handling missing values (3,730 missing production values identified and addressed)
2. Creating derived features (yield = production/area)
3. Standardizing state and district names
4. Creating lag features for time series analysis
5. Encoding categorical variables for model compatibility

## Usage
These datasets are directly used in our notebook:
1. The notebook automatically loads these files from this directory
2. Data preprocessing is handled in Cell 2
3. Exploratory analysis is performed in Cell 3
4. Feature engineering using this data is implemented in Cell 4

Both datasets have been included in this repository for ease of reproducibility and to allow for immediate execution of the analysis.
