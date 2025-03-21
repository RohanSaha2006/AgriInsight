# AgriInsight: Data-Driven Solutions for Food Security in India
## TRAIN-IT Hackathon 2025 | ImpactX Track

### Project Overview
This project analyzes agricultural data to address food security challenges in India through data-driven crop planning and forecasting. We developed a comprehensive analysis pipeline that processes historical crop production data to identify patterns, create predictive models, and generate recommendations for improving food security.

### Problem Statement
Despite being a major agricultural producer, India still faces significant food security issues due to price volatility, distribution inefficiencies, and production uncertainties. Our solution uses data science to optimize crop selection and improve agricultural productivity and sustainability.

### Key Notebook Cells
Our approach is structured in cells that progressively analyze and model the agricultural data:

1. *Setup and Problem Definition (Cell 1)*: Initializes libraries, defines our problem statement, and loads datasets
2. *Data Cleaning (Cell 2)*: Handles missing values, standardizes names, and creates derived features like yield
3. *Exploratory Data Analysis (Cell 3)*: Visualizes production trends, top crops, and seasonal patterns
4. *Feature Engineering (Cell 4)*: Creates lag features and encodes categorical variables
5. *Baseline Model (Cell 5)*: Implements linear regression as initial approach
6. *Advanced Model (Cell 6)*: Develops Random Forest model with improved performance
7. *Model Evaluation (Cell 7)*: Analyzes errors and validates model performance
8. *Food Security Analysis (Cell 9)*: Identifies vulnerable regions through custom metrics
9. *Sustainability Analysis (Cell 10)*: Assesses resource efficiency and sustainable practices
10. *Crop Recommendations (Cell 11)*: Provides data-driven crop selection guidance
11. *Impact Assessment (Cell 12)*: Quantifies potential benefits of implementation
12. *Documentation (Cell 13)*: Summarizes methodology, findings, and limitations
13. *Submission Package (Cell 14)*: Prepares final deliverables

### Datasets Used
- *Agricultural Production Dataset (APY)*: State-wise crop production statistics with 246,091 entries across 7 columns
- *Agricultural Commodity Price Dataset*: Market prices data with 23,093 entries across 10 columns

### Model Performance
- *Baseline Model (Linear Regression)*:
  - RMSE: 15,304,310.01
  - MAE: 1,182,554.75
  - R² Score: 0.16
  
- *Advanced Model (Random Forest)*:
  - RMSE: 6,443,694.69
  - MAE: 245,958.54
  - R² Score: 0.85

### Key Findings
- Production shows significant variation across states, creating regional dependencies
- Historical production trends reveal year-to-year fluctuations affected by climate and policy changes
- Top 10 crops dominate national agricultural output, with coconut leading production volumes
- Seasonal distribution shows distinct production patterns affecting year-round food availability
- Our model identifies optimal crops for different regions to maximize yield and sustainability

### Impact Projections
- 15% yield increase through optimized crop selection
- 30% reduction in vulnerable regions through targeted interventions
- 20% improvement in sustainable farming practices

### Required Dependencies

pandas
numpy
matplotlib
seaborn
scikit-learn
plotly


### Instructions to Run
1. Download the datasets and place in the appropriate directory
2. Execute the notebook cells in sequence from Cell 1 through Cell 14
3. View the generated visualizations and model results
4. Explore the crop recommendations for specific regions

### Team: The Technical Firsts
- Shambhavi Srivastava
- Rohan Saha

### Acknowledgements
- Data provided by TRAIN-IT Hackathon 2025 organizers
- Trinity Club, Army Institute of Technology, Pune
