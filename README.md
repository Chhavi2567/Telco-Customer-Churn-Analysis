# Telco Customer Churn Analysis

## Project Overview
This project focuses on performing Exploratory Data Analysis (EDA) on the Telco Customer Churn dataset. The primary goal of this project is to uncover insights related to customer churn and understand key factors influencing churn behavior.

Churn refers to the phenomenon where customers stop doing business with a company. The dataset contains information about the customers of a telecom company, their demographics, services they have subscribed to, and their payment behavior.

The project follows a structured approach that includes:
- Data Preprocessing and Handling Missing Values
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Label Encoding
- Preparation for Machine Learning Models

## Dataset Description
The Telco Customer Churn dataset consists of 21 features, including both categorical and numerical columns, and the target variable `Churn`.

### Columns in the Dataset:
1. **customerID**: Unique ID for each customer.
2. **gender**: Customer's gender (Male, Female).
3. **SeniorCitizen**: Indicates if the customer is a senior citizen (1 = Yes, 0 = No).
4. **Partner**: Whether the customer has a partner (Yes, No).
5. **Dependents**: Whether the customer has dependents (Yes, No).
6. **tenure**: Number of months the customer has stayed with the company.
7. **PhoneService**: Whether the customer has a phone service (Yes, No).
8. **MultipleLines**: Whether the customer has multiple lines (Yes, No, No phone service).
9. **InternetService**: Type of internet service (DSL, Fiber optic, No).
10. **OnlineSecurity**: Whether the customer has online security (Yes, No, No internet service).
11. **OnlineBackup**: Whether the customer has online backup (Yes, No, No internet service).
12. **DeviceProtection**: Whether the customer has device protection (Yes, No, No internet service).
13. **TechSupport**: Whether the customer has tech support (Yes, No, No internet service).
14. **StreamingTV**: Whether the customer has streaming TV (Yes, No, No internet service).
15. **StreamingMovies**: Whether the customer has streaming movies (Yes, No, No internet service).
16. **Contract**: The contract term of the customer (Month-to-month, One year, Two year).
17. **PaperlessBilling**: Whether the customer has paperless billing (Yes, No).
18. **PaymentMethod**: The customer’s payment method (Electronic check, Mailed check, Bank transfer (automatic), Credit card).
19. **MonthlyCharges**: The amount charged to the customer monthly.
20. **TotalCharges**: The total amount charged to the customer.
21. **Churn**: Whether the customer churned (Yes, No).

## Steps Performed

### 1. Data Preprocessing
- **Handling Missing Values**: The dataset had missing values in the `TotalCharges` column. These values were imputed based on the business understanding and the distribution of the feature.
- **Data Type Corrections**: Converted the `TotalCharges` column from object type to numeric.

### 2. Exploratory Data Analysis (EDA)
- **Univariate Analysis**: Analyzed the distribution of each feature individually using histograms, bar charts, and box plots.
- **Bivariate Analysis**: Investigated the relationships between features and the target variable `Churn` to understand which factors influence churn.
- **Correlation Analysis**: Examined correlations between numerical features to identify multicollinearity.

### 3. Feature Engineering
- **Feature Creation**: Created new features based on existing data, such as grouping tenure into categories (e.g., short-term, long-term).
- **Categorical Encoding**: Converted categorical variables into numerical format using Label Encoding for better compatibility with machine learning models.

### 4. Label Encoding
- Applied Label Encoding on binary categorical features such as `gender`, `Partner`, and `Churn`, converting them into 0 and 1 values for model compatibility.

## Conclusion
This project provides an in-depth exploration of the Telco Customer Churn dataset, revealing key insights into customer behavior and the factors that lead to churn. The analysis serves as a foundation for building predictive models that can help the telecom company retain its customers.

## How to Use
- Clone the repository to your local machine.
- Install the necessary Python libraries as mentioned in the `requirements.txt`.
- Run the notebook to view the data analysis steps and insights.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
