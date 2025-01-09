# Airline Customer Satisfaction Analysis

## Overview

This project predicts customer satisfaction for a fictional airline (Invistco Airlines), created solely for this analysis, based on customer feedback. The goal is to identify key factors influencing satisfaction and provide actionable insights to convert neutral or dissatisfied customers into satisfied ones.


## Key Insights from Exploratory Data Analysis (EDA) 
- **Dataset**: ~130K rows, minimal missing data (393 rows in "Arrival Delay in Minutes" filled with 0).
  (https://www.kaggle.com/datasets/teejmahal20/airline-passenger-satisfaction) 
- **Demographics**: Majority of passengers are aged 20–60, with a slight female majority.  
- **Satisfaction Trends**:  
  - **Highest Satisfaction**: Business travelers (69%) and Business Class passengers (48%).  
  - **Top Features**: Online boarding, inflight entertainment, and departure/arrival convenience received high ratings.  
  - **Improvement Areas**: Dissatisfaction was higher among younger (<25) and older (>65) age groups, and Economy Class passengers.  


## **Modeling Approach**  
### **1. Methodology**  
- **Data Splitting**: A 60-40 split for training and testing datasets was used to ensure robust evaluation.  
- **Target Variable**: Customer satisfaction (binary: satisfied vs. neutral/dissatisfied).  
- **Models Evaluated**:  
  - Logistic Regression, Decision Tree, Bagging, Random Forest, Gradient Boosting, and K-Nearest Neighbors classifiers.  

### **2. Recursive Feature Elimination (RFE)**  
- To enhance model performance, **RFE** was used to iteratively identify and remove the weakest features.  
- After feature reduction, models were retrained using the top predictive features, optimizing accuracy and interpretability.

<img src = "https://github.com/user-attachments/assets/e6556b23-a028-40b7-bf7a-c5eaaa0b3dca" width = 900 height = 400 >

### **3. Key Metrics**  
- **Accuracy**: Proportion of correctly classified instances.  
- **AUC (Area Under the Curve)**: Measures model performance across classification thresholds.  

**Top Performing Models**:  
- **Entire Dataset**: Random Forest Classifier (95.96% accuracy, 99.31% AUC).  
- **Subset Analyses**:  
  - Random Forest excelled in Business Class, loyal customers, and most age groups.  
  - Gradient Boosting outperformed in Economy Plus, disloyal customers, and older passengers (>65).  


## **Cost-Profit Analysis**  
### <ins> **Assumptions and Theory**  
The cost-profit analysis presented below is **theoretical** and based on assumed values. While these estimates are illustrative, they provide a framework to evaluate the business impact of feature improvements.

### <ins> **__Profit and Costs__**  
- Profit per dissatisfied passenger turned satisfied: **$500** (assumed).  
- Costs associated with increasing satisfaction by one unit for key variables:  
1. Flight Distance: $400
2. Inflight Wifi Service: $80
3. Ease of Online Booking: $60
4. Gate location: $140
5. Online Boarding: $70
6. Seat Comfort: $110
7. Inflight Entertainment: $50
8. On-board Service: $30
9. Leg-room Service: $500 
10. Baggage Handling: $20
11. Check-in Service: $20
12. Inflight Service: $40
13. Cleanliness: $20

### <ins>**__Key Observations__**  
1. **Highest ROI Features**:  
   - Improving **Inflight Wi-Fi Service** and **Online Boarding** yielded the highest return due to low costs and high impact on satisfaction.  
2. **Moderate ROI Features**:  
   - Enhancements to **Inflight Entertainment**, **Ease of Online Booking**, and **Food and Drink** provided balanced returns.  
3. **High Cost Features**:  
   - Features like **Legroom Service** ($500 per unit) were deemed less practical for immediate investment due to their high costs.
  
  <img src = "https://github.com/user-attachments/assets/209739ea-a6fa-4865-bf8b-f037ae5de89e" width = 900 height = 400 >

Decision performance analysis highlights that Inflight WiFi Service and Online Boarding are the most profitable features in terms of cost-benefit. Enhancements to these features could generate over $20,000 in additional revenue. Following these, Inflight Entertainment and Ease of Online Booking offer substantial benefits, with potential yields of approximately $10,000 and $3,500, respectively.

## **Business Recommendations**  
1. **Focus on Cost-Efficient Improvements**: Prioritize **Inflight Wi-Fi**, **Online Boarding**, and **Inflight Entertainment** for maximum profitability.  
2. **Targeted Efforts**: Develop loyalty strategies and incentives for disloyal or dissatisfied customer segments.  
3. **Class-Specific Enhancements**: Address dissatisfaction in Economy Class and personalize services for younger and older passengers.  


## **Limitations**  
- The dataset lacked variables like ticket price and inflight costs, which could have enabled a more detailed analysis.  
- Satisfaction was measured as a binary variable; a numerical scale (e.g., 1–10) could have provided richer insights.  
- **Cost estimates and profit assumptions are theoretical and should be validated with real-world data for actionable business strategies.**
