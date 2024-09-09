# Taxi Data Analysis - Regression Model and Results

**Taxi Project** explores the relationship between ride features and pricing using regression models to predict fare prices. The analysis leverages anonymized taxi data to identify key factors that influence pricing, focusing on building and evaluating a regression model to optimize fare predictions.



## 1. Regression Model

### Objective:

The main objective of this analysis is to build a regression model that predicts the taxi fare price based on various factors such as:
- Distance traveled
- Pickup and drop-off locations
- Time of day
- Traffic conditions
- Day of the week

### Model Selection:

We selected a multiple linear regression model to understand the linear relationship between these features and fare price. The features included in the model were:
- **Distance**: Primary predictor of fare, as expected.
- **Time of Day**: To capture peak vs off-peak effects.
- **Pickup/Drop-off Zones**: Geographical location influence.
- **Day of Week**: Weekdays vs weekends have distinct pricing patterns.

### Model Training:

The dataset was split into training and testing sets, with 70% of the data used for training and 30% for testing. The model was trained on the training data and evaluated on the testing data using metrics like Mean Squared Error (MSE) and R-squared.



## 2. Results

### Key Metrics:

- **R-squared value**: 0.78
  - This indicates that 78% of the variance in fare prices can be explained by the features in the model.

- **Mean Squared Error (MSE)**: $15.6
  - This metric helps assess the average squared difference between actual and predicted values. A lower MSE indicates better performance.
  
![image](https://github.com/user-attachments/assets/e4f9e16d-a75f-40e1-aa0d-cfb9cc117072)  

![image](https://github.com/user-attachments/assets/0f43a8b5-8f15-4b6a-89c7-f2abe94eda8e)



### Feature Importance:

- **Distance**: As expected, distance was the most significant predictor of fare, with a strong positive correlation.
- **Time of Day**: Fares were found to be higher during peak hours (morning and evening commutes) compared to late night or early afternoon times.
- **Location**: Pickup and drop-off zones significantly impacted fares, especially in high-demand areas like the central business district.
- **Day of the Week**: Weekends displayed slightly higher fares, possibly due to increased leisure travel.  

![image](https://github.com/user-attachments/assets/4e6dba15-83f8-49a2-9758-b2ee5f02f8ea)



## 3. Recommendations & Next Steps

1. **Model Improvements**: Consider integrating more advanced regression models or machine learning techniques, such as Random Forest Regression or Gradient Boosting, to capture nonlinear relationships.
   
2. **Additional Features**: Include weather conditions, traffic congestion levels, or surge pricing events as additional predictors to improve model accuracy.

3. **Real-Time Predictions**: Deploy the regression model to make real-time predictions for fare pricing based on current trip parameters, helping drivers and passengers make informed decisions.


