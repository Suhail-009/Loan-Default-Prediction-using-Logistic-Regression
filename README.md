# Loan-Default-Prediction-using-Logistic-Regression
A beginner-friendly machine learning project to predict whether a customer will default on a loan based on demographic and financial details. This project demonstrates data cleaning, encoding, exploratory analysis, model building, and evaluation using Python.

__📂 Project Overview__

The goal of this project is to build a classification model that predicts loan default using features such as:

* Applicant & Co-applicant Income
* Loan Amount
* Loan Term
* Credit History
* Education
* Property Area
* Marital Status
* Self Employment Status

This project uses Logistic Regression, a simple and effective algorithm for binary classification.

__🧾 Dataset__

The dataset (loan_data.csv) contains 500 rows and the following columns:

| Column            | Description                                       |
| ----------------- | ------------------------------------------------- |
| CustomerID        | Unique customer identifier                        |
| Gender            | Male / Female                                     |
| Married           | Yes / No                                          |
| Dependents        | Number of dependents                              |
| Education         | Graduate / Not Graduate                           |
| Self_Employed     | Yes / No                                          |
| ApplicantIncome   | Monthly income                                    |
| CoapplicantIncome | Additional income                                 |
| LoanAmount        | Loan amount requested                             |
| Loan_Amount_Term  | Duration of loan                                  |
| Credit_History    | 1 = good history, 0 = bad                         |
| Property_Area     | Urban/Semiurban/Rural                             |
| **Loan_Default**  | **Target variable** (1 = default, 0 = no default) |

**1. Data Loading**

Imported CSV using pandas.

**2. Exploratory Data Analysis (EDA)**

* Checked data types
* Summary statistics
* Missing values
* Basic distributions

**3. Data Cleaning**

* Removed unnecessary columns (CustomerID)
* Verified no missing values

**4. Encoding Categorical Variables**

Used LabelEncoder for columns like Gender, Married, Property_Area, etc.

**5. Feature Selection**

Defined:

* X → predictors
* y → target (Loan_Default)

**6. Train/Test Split**

80% training, 20% testing.

**7. Model Training**

Used Logistic Regression with 1000 max iterations.

**8. Model Evaluation**

Measured:

* Accuracy
* Confusion Matrix
* Precision, Recall, F1-Score

**9. Feature Importance**

Identified which features most influence loan default.

📊 Results

* Accuracy: 0.95%
* Customers with low combined income, high loan amount, or no credit history had the highest default probability.
* Logistic Regression provides a clear interpretation of feature influence.

🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

__📦 Project Structure__

Loan-Default-Prediction/

│

├── loan_data.csv

├── loan_default_prediction.ipynb

├── README.md

└── images/ (optional visualizations)

__🚀 How to Run the Project__

**1. Clone the repository**

git clone https://github.com/your-username/loan-default-prediction.git

**2. Install dependencies**

pip install -r requirements.txt

**3. Run the notebook**

jupyter notebook loan_default_prediction.ipynb

