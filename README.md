# Customer Behavior Analysis and Sales Forecasting

## **1. Project Overview**

The goal of this project is to analyze customer behavior for an e-commerce platform and provide actionable insights to improve sales, customer engagement, and personalize the shopping experience. This analysis includes:
- **Customer Churn Prediction**: Building a model to predict whether customers are likely to churn.
- **Sales Forecasting**: Developing a model to forecast future sales based on historical data.

Through data preprocessing, exploratory data analysis (EDA), and predictive modeling, this project aims to deliver meaningful insights and optimized strategies to enhance business performance.

## **2. Data Overview**

The dataset used for this project contains the following columns:
- **Customer ID**: Unique identifier for each customer.
- **Age**: Customer's age.
- **Gender**: Gender of the customer.
- **Location**: Customer's location.
- **Device Type**: Type of device used by the customer.
- **Session Count**: Number of sessions the customer has engaged in.
- **Time Spent (mins)**: Total time the customer spent on the platform.
- **Products Viewed**: Number of products viewed by the customer.
- **Purchases**: Number of purchases made by the customer.
- **Total Amount Spent**: Total amount spent by the customer.
- **Last Activity Date**: Date of the last activity by the customer.
- **Churned**: Whether the customer has churned (True/False).

## **3. Methodologies and Analysis**

### **Data Preprocessing and Cleaning**
The dataset was preprocessed and cleaned by:
- Handling missing values.
- One-hot encoding categorical variables like **Gender**, **Location**, and **Device Type**.
- Normalizing numerical features like **Age**, **Session Count**, and **Total Amount Spent**.

### **Exploratory Data Analysis (EDA)**
In-depth EDA was performed to understand the relationships between different variables. Key insights were drawn from:
- **Correlation Analysis**: Identified strong correlations between **Total Amount Spent** and **Purchases**.
- **Customer Segmentation**: Segmented customers based on features such as **Location** and **Device Type**.

### **Churn Prediction**
- A **Random Forest Classifier** was used to predict customer churn. Hyperparameters were optimized using **GridSearchCV**.
- The model achieved an accuracy of **80%** and a balanced confusion matrix, providing a reliable churn prediction.

### **Sales Forecasting**
- A **Random Forest Regressor** was used to predict future sales.
- The model achieved an **R² Score of 0.633**, indicating that the model explains 63% of the variance in sales.

## **4. Insights and Business Recommendations**

### **Churn Insights**:
- High engagement (e.g., more products viewed and time spent on the platform) reduces the likelihood of churn.
- **Gender** and **Location** were not significant predictors of churn, but engagement metrics were key.

### **Sales Insights**:
- More engagement correlates with higher sales, particularly through increased time spent on the platform.
- **Time spent** on the platform emerged as the most significant factor for predicting future sales.

### **Business Recommendations**:
1. **Customer Retention**: Implement targeted marketing campaigns for high-risk customers based on churn predictions.
2. **Sales Optimization**: Recommend more products to highly engaged customers to boost sales.
3. **Platform Improvements**: Enhance features that encourage longer time spent on the platform, such as personalized content and offers.

## **5. Conclusion**

This project demonstrates the power of data-driven insights in optimizing e-commerce strategies. By predicting customer churn and forecasting sales, businesses can make more informed decisions to improve customer retention and increase revenue.
