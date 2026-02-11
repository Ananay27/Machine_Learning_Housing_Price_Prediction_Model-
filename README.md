# Machine_Learning_Housing_Price_Prediction_Model-
Built a machine learning pipeline to predict California housing prices. The project includes data preprocessing with pipelines, handling numerical &amp; categorical features, training Random Forest models, and saving the model &amp; pipeline for inference on new data.

📊 Dataset

The dataset used is the California Housing dataset, sourced from Kaggle. It contains information about housing blocks in California, including:

- median_income – Median income of households

- housing_median_age – Median age of houses

- total_rooms, total_bedrooms – Number of rooms and bedrooms

- population – Population of the block

- households – Number of households

- median_house_value – Target variable (house value)

- ocean_proximity – Categorical feature indicating proximity to the ocean 🌊

🛠 Data Preprocessing

- Numerical features: Handled using median imputation and standard scaling.

- Categorical features: ocean_proximity transformed using one-hot encoding.

All preprocessing steps were combined into a pipeline, ensuring reproducibility and consistent transformation for both training and new data.

🤖 Modeling and Evaluation
Three regression models were evaluated to predict housing prices:

- Linear Regression – Baseline performance.

- Decision Tree Regressor – Captured non-linear relationships but overfitted on training data.

- Random Forest Regressor – Ensemble method with the best performance among the three.

Evaluation was performed using cross-validated Root Mean Squared Error (RMSE) to ensure robust performance estimates. The Random Forest model was chosen for final predictions.

📈 Results (Random Forest Regressor)

- Mean Absolute Error (MAE): 37,339

- Root Mean Squared Error (RMSE): 54,271

- R² Score: 0.774 ✅

These results indicate that the model explains ~77% of the variance in housing prices and predicts values with good accuracy.

💡 Key Learnings

- Implemented a complete machine learning workflow, from preprocessing to model deployment.

- Learned to handle both numerical and categorical features effectively using pipelines.

- Gained practical experience in model comparison and evaluation using cross-validation.

- Developed the ability to serialize models and preprocessing pipelines for reusable, production-ready predictions.

📝 Usage Notes

- Only a sample input dataset is included in the repository; the full dataset is available on Kaggle.

- Designed to be easy to run for anyone reviewing the repository, demonstrating technical skills and practical ML application.

⚙️ Dependencies

- Python 3.8+

- pandas

- numpy

- matplotlib

- scikit-learn

- joblib
