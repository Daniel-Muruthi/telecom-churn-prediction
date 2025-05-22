# Telecom Customer Churn Prediction

## 📈 Project Overview

This project focuses on predicting customer churn in the telecommunications sector using machine learning techniques. By analyzing customer demographics, service usage patterns, and account information, the model aims to identify customers at risk of leaving, enabling proactive retention strategies.

## 📊 Dataset Summary

- **Source**: [Kaggle - Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- **Total Records**: 7,043 customers
- **Features**: 21 attributes including:
  - **Demographics**: Gender, SeniorCitizen, Partner, Dependents
  - **Services**: PhoneService, MultipleLines, InternetService, OnlineSecurity, OnlineBackup, DeviceProtection, TechSupport, StreamingTV, StreamingMovies
  - **Account Info**: Tenure, Contract, PaperlessBilling, PaymentMethod
  - **Billing**: MonthlyCharges, TotalCharges
  - **Target**: Churn (Yes/No)

## 🧪 Exploratory Data Analysis (EDA)

- **Churn Distribution**: Approximately 26.6% of customers have churned, indicating class imbalance.
- **Contract Type vs. Churn**: Higher churn observed in month-to-month contracts compared to one-year or two-year contracts.
- **Monthly Charges vs. Churn**: Customers with higher monthly charges tend to churn more.
- **Correlation Analysis**: Identified key features correlated with churn, such as tenure and contract type.

## 🛠️ Data Preprocessing

- **Handling Missing Values**: Checked for and addressed any missing data.
- **Encoding Categorical Variables**: Applied label encoding and one-hot encoding where appropriate.
- **Feature Scaling**: Standardized numerical features to ensure uniformity.
- **Train-Test Split**: Divided data into training and testing sets to evaluate model performance.

## 🤖 Model Development

### Tuned Logistic Regression Model

After hyperparameter tuning, the Logistic Regression model demonstrated improved performance:

- **Accuracy**: 80.2% - 80% of all predictions are correct
- **Precision**: 64.9% - For every 100 customers flagged as high-risk 65 will actually churn (successful interventions) and 35 will be false positives (unnecessary outreach)
- **Recall**: 55.9% - Model identifies over half of all potential churners
- **F1-Score**: 60.1% - Good trade-off between precision and recall for business applications
- **ROC AUC Score**: 0.836 - the model correctly ranks customers by churn risk 83.6% of the time.

These metrics indicate a balanced and robust model, effectively distinguishing between churned and retained customers.

## 📌 Key Takeaways

- Manual and Non-automatic payment methods lead to higher churn rates.
- PaperlessBilling had the strongest retention factor proving digital engagement strongly correlates with loyalty
- Higher charges may contribute to customer dissatisfaction and churn.

## 📁 Repository Structure

- `index.ipynb`: Main notebook containing data exploration, preprocessing, and model development.
- `WA_Fn-UseC_-Telco-Customer-Churn.csv`: Dataset file.

## 🚀 Future Work

- **Model Enhancement**: Feature engineering, ensemble methods, real-time scoring.
- **Deployment**: Develop a user-friendly interface for real-time churn prediction.

## 📬 Contact

For further information or inquiries, please contact [Daniel Muruthi](mailto:adinomuruthi1@gmail.com).

---