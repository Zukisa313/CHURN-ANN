# Customer Churn Prediction App

This project is a **Machine Learning web application** that predicts whether a bank customer is likely to **churn (leave the bank)** based on their financial and demographic information.

The application uses a **Deep Learning model built with TensorFlow/Keras** and is deployed through an interactive **Streamlit web interface**.

---

## Project Overview

Customer churn prediction is a common problem in the banking and telecom industries. Predicting which customers are likely to leave allows companies to take proactive steps to retain them.

This application allows a user to input customer information such as:

- Credit score
- Age
- Balance
- Geography
- Number of bank products
- Account activity
- Estimated salary

The model then predicts the **probability that the customer will churn**.

---

## Tech Stack

- Python
- TensorFlow / Keras
- Scikit-Learn
- Pandas
- NumPy
- Streamlit
- Pickle



---

## Model Features

The model uses the following input features:

| Feature | Description |
|------|------|
| CreditScore | Customer credit rating |
| Geography | Customer location |
| Gender | Male or Female |
| Age | Customer age |
| Tenure | Years with the bank |
| Balance | Bank account balance |
| NumOfProducts | Number of bank products used |
| HasCrCard | Whether the customer has a credit card |
| IsActiveMember | Whether the customer is active |
| EstimatedSalary | Customer estimated salary |

---

## Data Preprocessing

Before feeding data into the model:

1. **Gender Encoding**
   - Converted using a LabelEncoder.

2. **Geography Encoding**
   - Converted using OneHotEncoder.

3. **Feature Scaling**
   - Numerical features are standardized using StandardScaler.

These preprocessing objects were saved using `pickle` and reused in the application to ensure consistent transformations.

---

## Model

The model is a **TensorFlow/Keras neural network** trained to perform binary classification.

Output:

```

Probability of churn

```

Decision rule:

```

Probability > 0.5 → Customer likely to churn
Probability ≤ 0.5 → Customer likely to stay

```

---

## Running the Application

### 1 Install dependencies

```bash
pip install -r requirements.txt
```

### Run the Streamlit app
```
streamlit run app.py
```
### Open in browser
```
http://localhost:8501
```
## Applications

Customer churn prediction models are widely used in:

- Banking
- Telecommunications
- Subscription services
- Insurance
- FinTech platforms

They help companies reduce revenue loss by identifying at-risk customers.

---

## Future Improvements

Possible extensions include:

- Deploying the app to Streamlit Cloud
- Adding model explainability (SHAP values)
- Improving model performance with hyperparameter tuning
- Adding API support using FastAPI
- Integrating a database for real-time predictions

---

## Author

**Zukisa Mkhize**  
BSc Honours Applied Mathematics  
Stellenbosch University  

**Interests:**

- Data Science
- Machine Learning
- Quantitative Finance
- Financial Modelling




