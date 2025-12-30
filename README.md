# Electric Power Consumption Prediction (RF, XGBR, CatB)

## Project Overview and Purpose
The goal of this project is to accurately forecast electric power consumption using historical usage data and temporal features. By comparing various Gradient Boosting and Ensemble models, the project identifies the most effective algorithm for capturing the non-linear patterns of energy demand, which is crucial for grid management and energy efficiency.

## Key Technologies and Libraries
- **Language**: Python
- **Machine Learning**: `scikit-learn`, `xgboost`, `catboost`
- **Data Manipulation**: `pandas`, `numpy`
- **Visualization**: `matplotlib`, `seaborn`
- **Evaluation**: Mean Squared Error (MSE), R² Score

## Methodology and Workflow
### Data Preprocessing
1. **Feature Engineering**: Extracted time-based features (Hour, Day, Month, Day of Week) to capture cyclical consumption patterns.
2. **Missing Values**: Performed data integrity checks and handled any missing or inconsistent records.
3. **Scaling**: Applied feature scaling to ensure uniformity across numerical inputs for the regression models.

### Model Architectures
The project implements and compares three powerful regression models:
- **Random Forest Regressor**: Used for its robust handling of outliers and ability to capture complex interactions.
- **XGBoost (XGBRegressor)**: A high-performance gradient boosting framework optimized for speed and accuracy.
- **CatBoost Regressor**: Specifically utilized for its superior handling of categorical features and efficiency in preventing overfitting.



## Results and Insights
- **Model Comparison**: The project provides a detailed comparison of MSE and R² scores across all three models.
- **Accuracy**: Ensemble methods like CatBoost and XGBoost generally provide superior results in energy forecasting due to their ability to model seasonal trends effectively.
- **Variable Importance**: Analysis of feature importance reveals that the time of day and day of the week are the strongest predictors of power consumption.

## How to Run
1. **Dataset**: Ensure the electric power consumption dataset is present in the working directory.
2. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
