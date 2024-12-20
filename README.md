# Predictive Maintenance for Swire Coca-Cola

## **Table of Contents**
1. [Business Problem](#1-business-problem)
   - 1.1. [Problem Statement](#11-problem-statement)
2. [Project Overview](#2-project-overview)
3. [Solution](#3-solution)
   - 3.1. [Survival Analysis](#31-survival-analysis)
   - 3.2. [Modeling Approach](#32-modeling-approach)
   - 3.3. [Predictive Model Results - XGBoost](#33-predictive-model-results-xgboost)
4. [Technologies Used](#4-technologies-used)
5. [My Contribution](#5-my-contribution)
6. [Business Value](#6-business-value)
   - 6.1. [ROI Sensitivity Analysis](#61-roi-sensitivity-analysis)
7. [Challenges](#7-challenges)
8. [Learnings](#8-learnings)
9. [Implementation Roadmap](#9-implementation-roadmap)
10. [Conclusion](#10-conclusion)


![logo](https://github.com/user-attachments/assets/cdc598fd-8d26-4bbf-b92e-4038b19456d7)

## 1. Business Problem 
Swire Coca-Cola faces significant unplanned downtime in its production plants, leading to an annual loss of approximately $60 million. These downtimes stem from mechanical failures, wear and tear, or unexpected breakdowns. The company aims to develop a predictive maintenance model to anticipate failures, reduce downtime, and enhance operational efficiency.

### 1.1. Problem Statement
- **Cost**: High costs associated with unexpected machine breakdowns ($60 million in annual losses).
- **Downtime Impact**: Inefficiencies in current reactive maintenance processes lead to increased downtime.
- **Operational Reliability**: Urgent need for a predictive maintenance approach to reduce unplanned outages and improve operational reliability.

## 2. Project Overview
This project focuses on shifting Swire Coca-Cola’s maintenance approach from reactive to predictive, leveraging historical data to anticipate failures and optimize maintenance scheduling. The predictive model aims to reduce downtime, minimize repair costs, and extend the life of production equipment.

## 3. Solution 
We developed a predictive model using historical downtime data to:
- **Predict when equipment will fail** 
- **Identify components frequently involved in breakdowns**
- **Optimize maintenance schedules** to reduce downtime

### 3.1. Survival Analysis
As part of the solution, we performed a **Survival Analysis** to understand the relationship between machine age and failure probabilities. This analysis helps in identifying the critical time points when failures are most likely to occur and can significantly improve maintenance scheduling.

Key features of the Survival Analysis:
- **Survival Probability**: The red line shows survival probability decreasing as machines age. Drops represent failure events; steeper drops indicate more frequent failures.
- **Critical Time Points**: 
  - The initial steep drop suggests high failure rates for new machines, possibly due to manufacturing defects or break-in issues. 
  - The plateauing later on indicates lower failure rates for older machines, likely due to the survival of the most reliable units or the impact of effective preventive maintenance.

This analysis has been integrated into the model to help prioritize maintenance schedules based on the likelihood of machine failure at specific ages.

### 3.2. Modeling Approach
Using advanced machine learning techniques like **Random Forest** and **XGBoost**, the project aimed to predict machine failure risks and optimize maintenance strategies by identifying key predictive features, such as maintenance intensity and machine age.

- **Logistic Regression**: Accuracy of 79% in predicting maintenance costs and failure impacts.
- **XGBoost**: Accuracy of 83%, with important features like **maintenance intensity** and **machine age** being crucial for the predictions.

### 3.3. Predictive Model Results- XGBoost
- **Post-Implementation Cost**:
  - Average Predicted Maintenance Cost: $715.99
  - Average Predicted Impact Cost: $358.00
  - Average Total Cost per Incident: $1073.99
- **Pre-Implementation Cost**:
  - Original Average Predicted Maintenance Cost: $1436.59
  - Original Impact Cost: $2873.17
  - Original Total Cost per Incident: $4309.76

## 4. Technologies Used
- **R**: For data analysis, exploration, and model development.
- **ggplot2**: For creating visualizations of maintenance trends and equipment breakdowns.
- **dplyr**: For data manipulation and cleaning.
- **tidyr**: For tidying up the data and reshaping datasets.
- **randomForest**: For machine learning and predicting failure likelihood.
- **xgboost**: For improved model performance and prediction accuracy.

## 5. My Contribution
- Worked on data exploration and visualization, focusing on creating intuitive charts for machine breakdown frequencies, seasonal maintenance trends, and maintenance cost distribution across equipment categories.
- Led the overall project coordination, ensuring alignment across different components of the modeling assignment.
- Contributed significantly to the **Exploratory Data Analysis (EDA)**, exploring various dimensions of the data such as machine age, maintenance types, and regional breakdowns.
- Worked on interpreting the model results and incorporating them into actionable business insights, focusing on cost analysis and how predictive maintenance could optimize operational strategies for Swire Coca-Cola.
- Contributed to the final report and presentation preparation, ensuring clear communication of the results to stakeholders.

## 6. Business Value 
This predictive maintenance system will:
- **Minimize Downtime**: By predicting equipment failures and optimizing schedules.
- **Reduce Maintenance Costs**: Proactive repairs and part procurement can reduce emergency maintenance costs.
- **Increase Production Efficiency**: Timely interventions will maximize machine uptime and ensure smoother operations.
- **Cost Savings**: Expected to save $12M annually by reducing unplanned maintenance costs.
- **Improved Operational Efficiency**: Anticipated 5% increase in production output, helping meet demand more effectively.

### 6.1. ROI Sensitivity Analysis
- **Annual Cost Savings**: Projected to save $12 million annually.
- **Downtime Reduction**: Model is expected to decrease unplanned downtime by 40%.
- **Higher Productivity**: Anticipated 5% increase in production output.
- **Less Inventory Waste**: Predictive stocking cuts down on unused parts by 15%, saving on storage and inventory costs.
- **High Return on Investment**: Forecasted to achieve a 150% ROI within the first year.

## 7. Challenges
- **Data Quality**: Inconsistent data and missing values required extensive cleaning.
- **Model Tuning**: Adjusting models to achieve a high prediction accuracy.
- **Integration**: Ensuring the predictive model could be integrated smoothly into existing workflows.

## 8. Learnings
- **Technical Skills**: Advanced my knowledge in predictive modeling and feature engineering.
- **Teamwork**: Worked collaboratively with team members to balance multiple tasks and deliver the project on time.
- **Business Insight**: Gained a deeper understanding of how predictive maintenance can impact operational efficiency and cost savings for businesses.

## 9. Implementation Roadmap
1. **Planning (0–3 months)**: Align objectives with stakeholders, upgrade infrastructure for data collection, and test predictive models.
2. **Pilot Testing (4–6 months)**: Test predictive maintenance on select machines, train teams on model use, and monitor results.
3. **Full-Scale Implementation (7–12 months)**: Roll out the model across all machines, integrate tools into workflows and dashboards, and track KPIs.
4. **Continuous Improvement (13+ months)**: Refine models with real-time feedback, explore AI-driven scheduling, and expand predictive insights.

## 10. Conclusion
This predictive maintenance approach is designed to:
- Reduce unplanned downtime by 40%.
- Achieve $12M in annual savings.
- Increase production efficiency by 5%.
- Realize a 150% return on investment in the first year.

This solution will help Swire Coca-Cola optimize machine usage, reduce unnecessary costs, and ensure smoother operations in the long term.

Thank you!
