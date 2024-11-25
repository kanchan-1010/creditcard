Credit Card Fraud Detection Model
This project is a Credit Card Fraud Detection Web App built using Python and Streamlit. The model is trained on a dataset of credit card transactions to classify transactions as legitimate or fraudulent using Logistic Regression.
Features
Machine Learning Model: A Logistic Regression model is used for binary classification.
Data Balancing: Legitimate and fraudulent transactions are balanced using undersampling to handle class imbalance.
Interactive Web App: Built with Streamlit, the app allows users to input transaction features and predict whether a transaction is legitimate or fraudulent.
Evaluation Metrics: The app evaluates the model's performance using accuracy on both training and test data.
Dataset
The dataset used for training the model is creditcard.csv. This dataset contains credit card transaction records with features like V1, V2, ..., V28, Amount, and a Class label where:

Class = 0: Legitimate Transaction
Class = 1: Fraudulent Transaction
Model Workflow
Data Preprocessing:

Transactions are separated into legitimate and fraudulent classes.
Legitimate transactions are undersampled to balance the data.
Features (V1 to V28 and Amount) are used as input, while the Class column is the target.
Train-Test Split:

The data is split into training (80%) and testing (20%) sets, ensuring class stratification.
Model Training:

A Logistic Regression model is trained using the scikit-learn library.
Evaluation:

Model performance is evaluated using accuracy on both training and test datasets.
Deployment:

The trained model is integrated into a Streamlit app for real-time predictions
Dependencies
Python 3.7+
pandas
numpy
scikit-learn
streamlit
Acknowledgements
The dataset used in this project is publicly available on Kaggle.
This project uses Streamlit for building the interactive web application.
Future Enhancements
Use advanced models like Random Forest or Gradient Boosting for better performance.
Improve user interface for better usability.
Deploy the app on cloud platforms like AWS or Heroku for public access.
