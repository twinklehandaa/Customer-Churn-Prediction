# Customer Churn Prediction
Customer churn is a critical metric for subscription-based businesses. This project addresses the challenge of predicting which customers are likely to churn, enabling proactive customer retention efforts. The model utilizes a dataset of past subscriptions, including customer demographics, usage patterns, and subscription details, to identify patterns and predict future churn.
## Dataset

The dataset used in this project consists of two CSV files:

- `train.csv`: Contains historical subscription data, including the target variable `Churn` (indicating whether a customer canceled their subscription). This dataset is used for training the machine learning model.
- `test.csv`: Contains subscription data for which churn predictions need to be made. This dataset is used for evaluating the model's performance on unseen data.
## Methodology

The project follows a typical machine learning workflow:

1. **Data Exploration and Preprocessing:** Exploratory Data Analysis (EDA) was performed to understand the data, identify missing values, and visualize feature distributions. Missing values were handled using imputation. Categorical features were encoded using one-hot encoding. Numerical features were scaled using StandardScaler.
2. **Model Selection:** A Logistic Regression model was chosen for predicting churn due to its interpretability and efficiency for binary classification problems.
3. **Model Training:** The model was trained on the `train.csv` dataset.
4. **Model Evaluation:** The model's performance was evaluated using appropriate metrics (e.g., accuracy, precision, recall, F1-score, AUC-ROC) on a held-out validation set or through cross-validation.
5. **Prediction:** The trained model was used to predict churn probabilities for the subscriptions in `test.csv`.

The predictions were saved to a CSV file (`predicion.csv`)
