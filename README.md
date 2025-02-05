# Monthly Revenue Prediction Based on Historical Data

## Project Overview
This project explores the use of various regression model to predict monthly revenue based on historical data. The dataset ( taken from this project https://github.com/Aminkay95/Retail-Data-Analysis-sql ) includes revenue information for various months, with the goal of building a predictive model that uses the month as a categorical feature. The project demonstrates data preprocessing, model training, evaluation, and interpretation of results. The best-performing model, a Linear Regression model, was saved by serializing it into a file named lr_model.pkl using the pickle library

---

## Methodology

### Data Preprocessing
1. **One-Hot Encoding**:
   - The `Month` column was encoded using one-hot encoding to convert categorical values into numerical format.
   - This allows the linear regression model to process the categorical feature.

2. **Train-Test Split**:
   - The dataset was split into training (80%) and testing (20%) subsets.

### Model Training
- Various models were used to predict revenue based on the one-hot encoded `Month` values.

### Model Evaluation
- **Mean Squared Error (MSE)** was used as the primary evaluation metric.
- **R-squared (R²)** was also analyze the performance of the models.

---

## Results

- **MSE**: An MSE of approximately **76100000000 ** was archieved across the various models, indicating large prediction errors.
- **R-squared**: The R² score was also low across the models, suggesting that the models failed to explain the variability in revenue based on the month.

### Key Insights
1. The high MSE and low R² score suggest poor model performance.
2. Predicting revenue based solely on the `Month` feature is insufficient, as additional predictors (e.g., seasonal trends, marketing campaigns, or economic indicators) may be required.

---

## Conclusions
- The models' poor performance highlights the importance of feature selection and data quality in predictive modeling.
- Future iterations of this project should include more comprehensive features to improve the model’s accuracy and interpretability.
  

---

## Technologies Used
- **Python**
  - pandas
  - scikit-learn

---

## How to Run the Project
1. Clone the repository.
2. Install the required dependencies:
   ```bash
   pip install pandas scikit-learn
   ```
3. Run the script to preprocess the data, train the model, and evaluate its performance.


