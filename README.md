# 🛒 AI-Powered Customer Churn & Retention Intelligence

An end-to-end **Machine Learning + Explainable AI + Generative AI** application that predicts e-commerce customer churn, identifies the key factors driving churn using SHAP, and generates personalized retention strategies using Groq GenAI.

The project transforms raw customer data into **actionable retention intelligence**, helping businesses identify high-risk customers and understand *why* they are likely to churn.

---

## 🚀 Live Application

🔗 **Try the deployed application:**  
[Customer Churn Intelligence App](YOUR_STREAMLIT_APP_URL)

Users can enter customer information and instantly receive:
- Churn probability
- Customer risk classification
- Customer value segment
- Key churn drivers
- AI-generated retention recommendations

---

## 🎯 Project Objective

Customer churn directly impacts revenue, customer lifetime value, and acquisition costs.

This project answers three important business questions:

1. **Who is likely to churn?**
2. **Why is the customer likely to churn?**
3. **What action can the business take to retain them?**

---

## ✨ Key Features

### 🤖 Churn Prediction
A **Random Forest classifier** predicts individual customer churn probability based on behavioral, transactional, demographic, and engagement features.

### ⚠️ Customer Risk Intelligence
Customers are categorized into meaningful risk levels based on their predicted churn probability.

### 💰 Customer Value Segmentation
Customer purchasing behaviour is used to classify customers into value segments, enabling retention efforts to focus on commercially important customers.

### 🔍 SHAP Explainability
**SHAP (SHapley Additive exPlanations)** explains individual predictions and identifies the customer-specific factors increasing or decreasing churn risk.

### 🧠 AI-Powered Retention Strategy
Customer risk, value, churn probability, and SHAP drivers are passed to **Groq-powered Generative AI** to generate personalized and actionable retention recommendations.

### 🌐 Interactive Streamlit Application
A user-friendly Streamlit interface connects the entire ML + XAI + GenAI pipeline into a deployable business application.

---

## 🔄 End-to-End Workflow

```text
Customer Data
      │
      ▼
Data Cleaning & EDA
      │
      ▼
Feature Engineering
      │
      ▼
Machine Learning Models
      │
      ▼
Random Forest Churn Model
      │
      ▼
Churn Probability
      │
      ├───────────────┐
      ▼               ▼
Risk Level      Customer Value
      │               │
      └───────┬───────┘
              ▼
      SHAP Explainability
              │
              ▼
       Key Churn Drivers
              │
              ▼
          Groq GenAI
              │
              ▼
 Personalized Retention Strategy
              │
              ▼
       Streamlit Application
```

---

## 📊 Customer Insights

The analysis explores customer behaviour across key dimensions such as:

- Purchase frequency and spending behaviour
- Average purchase value
- Customer engagement
- Satisfaction score
- Membership status
- Website activity
- Support interactions
- Days since last purchase
- Customer referrals
- Churn behaviour

These insights help identify patterns associated with customer retention and churn.

---

## 🧪 Machine Learning

Multiple classification approaches were evaluated for churn prediction, with **Random Forest selected as the final model**.

### Evaluation Metrics

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC

For a churn use case, identifying actual churners is particularly important because missing a high-risk customer can result in lost revenue and retention opportunities.

---

## 🔍 Explainable AI with SHAP

Traditional ML models can provide accurate predictions but often fail to explain *why* a prediction was made.

SHAP adds transparency by showing how individual customer features influence churn probability.

For each prediction, the application identifies:

**Features increasing churn risk ↑**

and

**Features reducing churn risk ↓**

This makes the model significantly more useful for business decision-making.

---

## 🧠 Generative AI Retention Intelligence

Instead of stopping at churn prediction, the application converts model insights into **business actions**.

The GenAI layer receives:

```text
Churn Probability
        +
Risk Level
        +
Customer Value
        +
Top SHAP Drivers
        ↓
Groq LLM
        ↓
Personalized Retention Strategy
```

This allows the system to recommend customer-specific interventions rather than generic retention campaigns.

---

## 💡 Example Business Use Case

Consider a customer with:

```text
Churn Probability: 82%
Risk Level: High
Customer Value: High
```

SHAP may identify:

```text
Low Satisfaction Score
High Days Since Last Purchase
Low Website Engagement
```

The system can then recommend actions such as:

- Personalized re-engagement campaign
- Targeted loyalty incentive
- Customer support outreach
- Product recommendations based on previous purchases

This turns a **prediction into an actionable retention decision**.

---

## 🛠️ Tech Stack

| Category | Technologies |
|---|---|
| Programming | Python |
| Data Analysis | Pandas, NumPy |
| Machine Learning | Scikit-learn |
| ML Model | Random Forest |
| Explainable AI | SHAP |
| Generative AI | Groq API |
| Visualization | Matplotlib |
| Application | Streamlit |
| Model Persistence | Joblib |
| Deployment | Streamlit Community Cloud |
| Version Control | Git & GitHub |

---

## 📁 Project Structure

```text
AI-Powered-Customer-Churn-Intelligence/
│
├── app/
│   └── app.py
│
├── data/
│   └── customer data
│
├── models/
│   └── best_churn_model.joblib
│
├── notebooks/
│   ├── EDA / analysis notebooks
│   ├── ML modeling
│   └── Groq recommendations
│
├── src/
│   ├── __init__.py
│   ├── explainability.py
│   └── genai.py
│
├── .gitignore
├── requirements.txt
└── README.md
```

---

## ⚙️ Run Locally

### 1. Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd AI-Powered-Customer-Churn-Intelligence
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Configure Groq

Create a `.env` file:

```env
GROQ_API_KEY=your_groq_api_key
GROQ_MODEL=your_groq_model
```

> ⚠️ Never commit your `.env` file or API key to GitHub.

### 4. Run the application

```bash
python -m streamlit run app/app.py
```

---

## 📌 Key Takeaways

- Built an **end-to-end churn intelligence system** rather than only a prediction model.
- Applied **Random Forest** for customer-level churn probability prediction.
- Integrated **SHAP explainability** to identify customer-specific churn drivers.
- Combined churn risk with **customer value intelligence** for better prioritization.
- Integrated **Groq GenAI** to convert ML explanations into actionable retention strategies.
- Developed an interactive **Streamlit application** for real-time customer analysis.
- Designed the solution around the business objective of **improving retention and reducing revenue at risk**.

---

## 🔮 Future Improvements

- Real-time integration with CRM/customer databases
- Automated retention campaign triggering
- Customer Lifetime Value (CLV) prediction
- Churn monitoring dashboard
- Model monitoring and drift detection
- A/B testing of AI-generated retention strategies

---

## 👩‍💻 Author

**Aastha Singh**

Interested in **Data Analytics, Machine Learning, Generative AI, and Product Analytics**.

⭐ If you found this project useful, consider starring the repository.
