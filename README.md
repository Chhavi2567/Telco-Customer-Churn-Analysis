# Telco Customer Churn Analysis

## Project Overview
This project aims to analyze customer churn behavior in the telecom industry using the **Telco Customer Churn** dataset. Customer churn refers to the scenario where customers stop using a company's services. The primary goal of this project is to uncover insights related to customer churn and understand key factors influencing churn behavior. This analysis is crucial for telecom companies to identify patterns that lead to churn and take proactive steps to retain their customers.

The project follows a structured approach, which includes:
- Data Preprocessing and Handling Missing Values
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Label Encoding
- Preparing the dataset for Machine Learning Models

## Dataset Source
The dataset used in this project has been taken from the [Kaggle Telco Customer Churn Dataset](https://www.kaggle.com/blastchar/telco-customer-churn). It contains data about customers from a telecom company, including demographic information, services subscribed to, and payment details.

## Dataset Description
The Telco Customer Churn dataset consists of 21 columns, including demographic, service-related, and financial information, along with the target variable `Churn`.

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
- **Handling Missing Values**: The `TotalCharges` column had missing values, which were handled through imputation.
- **Removing Unnecessary Columns**: The `customerID` column was removed as it was not relevant for the analysis.
- **Data Type Adjustments**: Converted the `TotalCharges` column from object type to numeric, which allowed for further analysis.
- **Outlier Detection and Handling**: Identified and handled outliers where necessary to ensure the accuracy of the analysis.

### 2. Exploratory Data Analysis (EDA)
- **Univariate Analysis**: Performed distribution analysis on individual features using histograms and box plots to understand data spread and skewness.
- **Bivariate and Multivariate Analysis**: Analyzed the relationship between features and the target variable `Churn` through cross-tabulations, correlation heatmaps, and pair plots to uncover potential predictors of churn.
- **Churn Analysis**: Explored key factors such as contract type, tenure, and payment methods to determine their influence on customer churn rates.

### 3. Feature Engineering
- No additional features were created in this analysis.

### 4. Label Encoding
- **Binary and Multiclass Encoding**: Binary categorical variables like `gender`, `Partner`, and `Churn` were encoded as 0 and 1. Multiclass categorical features such as `Contract` and `PaymentMethod` were encoded into numerical labels.

## Key Insights from the Analysis
- **Contract Type**: Customers with month-to-month contracts are more likely to churn compared to those with one or two-year contracts. This suggests that longer contract durations could reduce churn.
- **Tenure**: Customers who have stayed with the company for a shorter period are more likely to churn. Retention strategies should focus on newer customers.
- **Payment Method**: Customers who use electronic checks as their payment method tend to churn more compared to those who use automatic payments like bank transfers or credit cards.
- **Service Subscription**: Customers without internet service and those not subscribed to premium services like streaming TV or movies show higher churn rates, indicating a possible relationship between service usage and customer loyalty.

## Suggestions to Reduce Churn
Based on the insights from the analysis, here are some actionable suggestions for the company to reduce churn:

1. **Incentivize Long-Term Contracts**: 
   - Offer attractive discounts or additional services for customers who switch from month-to-month contracts to longer-term contracts. This could increase customer retention by reducing the ease of churn.

2. **Focus on New Customer Retention**:
   - Customers with shorter tenure are more likely to churn. Introduce targeted onboarding programs and regular follow-ups for new customers during their first few months to enhance their satisfaction and engagement.

3. **Promote Automatic Payment Methods**:
   - Encourage customers to use automatic payment methods (e.g., bank transfer or credit card) instead of electronic checks. Offering discounts or loyalty points for switching to automatic payments could help reduce churn.

4. **Enhance Service Bundling**:
   - Promote bundled services (e.g., internet, phone, and streaming services) to customers who currently subscribe to only one service. This can improve customer stickiness as they are less likely to churn if they use multiple services from the company.

5. **Offer Customizable Service Packages**:
   - Provide customizable service packages that cater to different customer needs. Flexibility in choosing services and pricing can reduce churn by aligning the services with the customer’s preferences.

6. **Loyalty Programs and Rewards**:
   - Introduce a loyalty program that rewards long-term customers with exclusive offers, discounts, or free upgrades. Recognizing customer loyalty can increase their commitment to the company.

## Conclusion
The analysis reveals that churn is closely related to customer contract type, tenure, and payment method. By implementing strategies such as promoting long-term contracts, focusing on new customer retention, and offering bundled services, the company can significantly reduce churn rates and improve customer satisfaction.

Understanding these factors can help telecom companies develop targeted strategies to reduce churn and improve customer retention.
