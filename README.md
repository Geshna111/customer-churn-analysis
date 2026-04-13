# Customer Churn Analysis & Prediction

> End-to-end data analysis and machine learning project focused on identifying high-risk customers and translating insights into actionable business strategies.

## Problem Statement - 
Customer churn leads to significant revenue loss in subscription-based businesses. 
This project aims to identify customers at high risk of churn and provide actionable 
strategies to improve customer retention and reduce revenue loss.

## Dataset 
- Source: Kaggle (IBM Telco Customer Churn Dataset)
- Records: ~7,000 customers
- Features: 21 variables including demographics, services, contract details, and billing information

## Key Insights
- Customers on month-to-month contracts show significantly higher churn compared to long-term contracts
- Customers with higher monthly charges show increased churn, indicating price sensitivity and potential dissatisfaction with perceived value
- Customers with lower tenure (new users) have the highest churn risk, highlighting onboarding gaps
- Fiber optic internet users show higher churn, possibly due to higher expectations or pricing concerns
- Customers without add-on services (e.g., security, tech support) are more likely to churn, suggesting lower engagement

## Key Drivers of Churn
- Contract type (month-to-month)
- Tenure (short-duration customers)
- Monthly charges (higher pricing segments)
- Lack of value-added services (security, support)

## Key Visualizations

### Churn Distribution
<img src="https://github.com/user-attachments/assets/2f2d93d2-7289-43b3-a4b8-8d4229e4dee8" width="500"/>

### Tenure vs Churn
<img src="https://github.com/user-attachments/assets/520df7ea-de12-4b2e-9208-dba50c1927a3" width="500"/>

## Model Performance
- Logistic Regression ROC-AUC: ~0.83
- Random Forest ROC-AUC: ~0.81

The Logistic Regression model demonstrates strong discriminative ability. However, recall for churned customers (~52%) indicates that nearly half of actual churn cases are not being captured. This highlights a trade-off between precision and recall and suggests scope for improvement through threshold tuning or class balancing techniques.

## Business Recommendations
- Offer discounted long-term contracts to customers on month-to-month plans
- Implement targeted retention campaigns for high-risk customer segments
- Improve onboarding experience for new customers to reduce early churn
- Re-evaluate pricing strategies for high monthly charge segments
- Promote value-added services (security, support) to increase customer stickiness

## Business Impact
- ~7% of customers identified as high-risk (churn probability > 0.7)
- Estimated monthly revenue at risk: ₹2.3–2.5 lakh

Calculation:
Assuming average revenue of ₹500 per customer,  
478 high-risk customers × ₹500 ≈ ₹2,39,000/month  

Even a 20–30% improvement in retention for this segment could result in significant monthly revenue savings, making targeted intervention highly valuable.

## Tech Stack - 
Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
