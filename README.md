# Customer Churn Analysis & Prediction

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
- Higher monthly charges are associated with increased churn, indicating price sensitivity
- Customers with lower tenure (new users) have the highest churn risk
- Fiber optic internet users show higher churn, possibly due to higher expectations or pricing
- Lack of add-on services (e.g., security, tech support) correlates with higher churn

## Key Visualizations
<img width="831" height="631" alt="image" src="https://github.com/user-attachments/assets/2f2d93d2-7289-43b3-a4b8-8d4229e4dee8" width = "500" style="border-radius:10px;"/>

<img width="803" height="624" alt="image" src="https://github.com/user-attachments/assets/520df7ea-de12-4b2e-9208-dba50c1927a3" width = "500" style="border-radius:10px;" />

## Model Performance
- Logistic Regression ROC-AUC: ~0.83
- Random Forest ROC-AUC: ~0.81

The Logistic Regression model demonstrates strong discriminative ability, though recall for churned customers (~52%) indicates scope for improvement in identifying all at-risk users.

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

Targeting this segment can significantly reduce revenue loss with focused retention efforts.

## Tech Stack - 
Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
