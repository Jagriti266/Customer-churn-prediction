# Customer Churn Prediction

This project focuses on predicting customer churn for a bank using various machine learning models. Customer churn, also known as customer attrition, is the loss of clients or customers. Predicting churn is crucial for businesses to retain customers and improve their services.

## Dataset

The dataset used in this project is `Churn_Modelling.csv`, which contains information about bank customers, including their demographics, account details, and whether they have exited the bank.

**Columns:**

- `RowNumber`: Row number.
- `CustomerId`: Unique identifier for each customer.
- `Surname`: Customer's surname.
- `CreditScore`: Customer's credit score.
- `Geography`: Customer's location (France, Spain, Germany).
- `Gender`: Customer's gender (Male, Female).
- `Age`: Customer's age.
- `Tenure`: Number of years the customer has been with the bank.
- `Balance`: Customer's account balance.
- `NumOfProducts`: Number of bank products the customer uses.
- `HasCrCard`: Whether the customer has a credit card (1: Yes, 0: No).
- `IsActiveMember`: Whether the customer is an active member (1: Yes, 0: No).
- `EstimatedSalary`: Customer's estimated salary.
- `Exited`: Whether the customer has exited the bank (1: Yes, 0: No) - This is the target variable.

## Analysis and Modeling

The project involves the following steps:

1.  **Data Loading and Exploration**: Load the dataset and perform initial exploration to understand the data distribution and identify potential issues.
2.  **Data Preprocessing**:
    - Drop irrelevant columns (`RowNumber`, `CustomerId`, `Surname`).
    - Encode categorical variables (`Geography`, `Gender`) using one-hot encoding.
    - Scale numerical features using StandardScaler.
3.  **Data Splitting**: Split the data into training and testing sets.
4.  **Model Training**: Train different classification models to predict customer churn. The models used include:
    - Logistic Regression
    - Random Forest Classifier
    - Gradient Boosting Classifier
5.  **Model Evaluation**: Evaluate the performance of each model using metrics such as accuracy.

## Results

The models were trained and evaluated on the dataset. The accuracy scores for each model are as follows:

-   **Random Forest Classifier**: 0.999875 (Training), 0.8635 (Validation)
-   **Logistic Regression**: 0.772
-   **Gradient Boosting Classifier**: 0.865

## Usage

To run this project:

1.  Clone the repository.
2.  Install the required libraries (`pandas`, `numpy`, `matplotlib`, `seaborn`, `sklearn`, `imblearn`).
3.  Run the Jupyter Notebook or Python script containing the code.
