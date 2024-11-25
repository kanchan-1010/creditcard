# Credit Card Fraud Detection Web App

This project is a **Credit Card Fraud Detection Web App** built using **Python** and **Streamlit**. The model is trained on a dataset of credit card transactions to classify transactions as legitimate or fraudulent using **Logistic Regression**.

## Features

- **Machine Learning Model**: A Logistic Regression model is used for binary classification.
- **Data Balancing**: Legitimate and fraudulent transactions are balanced using undersampling to handle class imbalance.
- **Interactive Web App**: Built with Streamlit, the app allows users to input transaction features and predict whether a transaction is legitimate or fraudulent.
- **Evaluation Metrics**: The app evaluates the model's performance using accuracy on both training and test data.

## Dataset

- **Shape**: The dataset has 284,807 rows and 31 columns.
- **Columns**:
  - `Time`: Time of the transaction.
  - `V1` to `V28`: Transformed features obtained via PCA (Principal Component Analysis).
  - `Amount`: Transaction amount.
  - `Class`: Indicates whether the transaction is fraudulent (`1`) or not (`0`).
- **Data Types**:
  - All columns except `Class` are of type `float64`.
  - The `Class` column is of type `int64`.
- **Classes**:
  - `Class = 0`: Legitimate Transaction
  - `Class = 1`: Fraudulent Transaction

## Model Workflow

### 1. Data Preprocessing
- Transactions are separated into legitimate and fraudulent classes.
- Legitimate transactions are undersampled to balance the data.
- Features (`V1` to `V28` and `Amount`) are used as input, while the `Class` column is the target.

### 2. Train-Test Split
- The data is split into training (80%) and testing (20%) sets, ensuring class stratification.

### 3. Model Training
- A Logistic Regression model is trained using the **scikit-learn** library.

### 4. Evaluation
- Model performance is evaluated using accuracy on both training and test datasets.

### 5. Deployment
- The trained model is integrated into a **Streamlit** app for real-time predictions.

## Dependencies

Ensure you have the following dependencies installed:

- Python 3.7+
- pandas
- numpy
- scikit-learn
- streamlit

Install the dependencies using:

```bash
pip install -r requirements.txt
```

## Deployment

1. Clone this repository.
2. Run the Streamlit app locally using the following command:

```bash
streamlit run app.py
```

## Acknowledgements

- The dataset used in this project is publicly available on **Kaggle**.
- This project uses **Streamlit** for building the interactive web application.

## Future Enhancements

- Use advanced models like **Random Forest** or **Gradient Boosting** for better performance.
- Improve the user interface for better usability.
- Deploy the app on cloud platforms like **AWS** or **Heroku** for public access.
