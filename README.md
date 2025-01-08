# Airline Customer Satisfaction Analysis

## Overview

This project predicts customer satisfaction for a fictional airline (Invistco Airlines), created solely for this analysis, based on customer feedback. The goal is to identify key factors influencing satisfaction and provide actionable insights to convert neutral or dissatisfied customers into satisfied ones.

## Key Insights

**Exploratory Data Analysis**

- Dataset: 130K rows, minimal missing data.

- Demographics: Majority aged 20-60, slight female majority.

**Satisfaction Levels:**

- Business Class: Highest satisfaction (48%).

- Economy Plus: Moderate satisfaction (7%).

- Economy: Areas for improvement (45%).

- Top Factors: Online boarding, inflight entertainment, and convenience of departure/arrival times.


## Predictive Modeling

### *Best Models:*

- Random Forest Classifier (Accuracy: ~96%, AUC: ~99%) for most subsets.

- Gradient Boosting Classifier for specific cases (e.g., Economy Plus).

### *Approach:*

- 60/40 data split for training/testing.

- Recursive feature elimination to identify top contributors to satisfaction.

Suggested Visual: A table or graph comparing model accuracies and AUC scores across subsets.

## Potential Results and Impacts

- By improving the top influential features, the analysis predicts:

- Inflight Wi-Fi Service: Increasing satisfaction here can yield profits of over $20K.

- Online Boarding: Improvements in this area result in a substantial boost to customer satisfaction and convenience.

- Inflight Entertainment: Predicted profit impact of ~$10K.

- Ease of Online Booking: Enhancements can bring ~$3.5K profit.

These improvements not only increase satisfaction but also enhance customer retention, especially in the economy class, which shows 60% dissatisfaction. Additionally, disloyal customers can be converted with targeted offers and discounts, maximizing revenue and reducing churn.

**Suggested Visuals:**

A cost-benefit bar graph showing the profitability of improving different features.

Pie charts representing satisfaction levels for loyal vs. disloyal customers.

## Recommendations

- Focus on Key Features: Invest in inflight Wi-Fi, online boarding, and entertainment for the highest cost-benefit ratio.

- Address High Dissatisfaction Areas: Target dissatisfied Economy passengers with tailored services and incentives.

- Retention Strategies: Offer discounts or rewards to disloyal customers to improve satisfaction and prevent churn.

## Limitations

- Data Gaps: Missing details like ticket prices and inflight service costs make precise cost-benefit calculations challenging.

- Satisfaction Metric: A binary classification (satisfied vs. dissatisfied/neutral) limits the granularity of analysis. A numerical satisfaction score would allow more detailed insights.

## Conclusion

Investing in inflight Wi-Fi, online boarding, and entertainment improvements can significantly boost satisfaction and profits. Prioritize tailored services for dissatisfied demographics and implement retention strategies for long-term growth.

Suggested Final Visual: A summary infographic showing overall model performance, key findings, and recommendations.
