# High-value-prediction
### Overview
This project focuses on feature engineering and logistic regression analysis for a dataset related to food delivery services. The primary goal is to analyze customer behavior, optimize delivery metrics, and explore the relationships between various numerical, temporal, and categorical features to provide actionable business insights. Additionally, logistic regression was applied to predict key outcomes, and its performance was evaluated using metrics like accuracy, recall, precision, and F1-score. Confusion matrices and insights from the results are included to answer specific business questions.

### Data Used
The dataset includes synthetic information about food delivery orders, consisting of:
* Order Details: Order ID, customer ID, order amount, and meal category.
* Time-Based Features: Order and delivery timestamps
* Customer Attributes: Customer loyalty points and account creation dates.
* Other Features: Delivery fees and payment methods.
  
## Methoodology
### Data Preprocessing
* Handling Missing Values: Ensured data completeness by filling or removing missing values.
* Feature Creation: Created new columns like delivery duration and customer tenure.
* Encoding: Applied one-hot encoding for categorical variables (e.g., meal_category, payment_method).

### Exploratory Data Analysis (EDA)
* Explored correlations between numerical features, such as order_amount and delivery_fee.

### Feature Engineering
* Temporal Features: Derived delivery duration by calculating the time difference between order_date and delivery_time.
* Customer Insights: Calculated lifetime value and loyalty points trends.
* Numerical Transformations: Normalized or scaled features for consistent analysis.

### Logistic Regression
*Model Objective: Predict binary outcomes such as whether an order will be delivered on time.


# Key Questions Explored
1.) What is the distribution of delivery durations?
  * Answer: Delivery durations were calculated as the difference between order_date and delivery_time. The analysis showed an average delivery duration of       
approximately 45 minutes.

2.) What insights can accuracy, recall, and F1-score provide about logistic regression performance?
  * Answer: The logistic regression model achieved:
    * Accuracy: 85%
    * Recall: 82%
    * Precision: 88%
    * F1-Score: 85%
* These metrics indicate that the model was robust, but false negatives (late deliveries predicted as on-time) remained an area for improvement.

3.)What does the confusion matrix reveal about the model?
  * Answer: The confusion matrix highlighted that while the model accurately identified most on-time deliveries, there was a significant proportion of false negatives, suggesting the need for better feature selection or additional data.


# Business Insights and Results
* Delivery Optimization: Identified an average delivery duration of 45 minutes, suggesting resource allocation during peak times to reduce delays.
* Customer Segmentation: High-loyalty customers were identified for potential targeted marketing campaigns.
* Predictive Insights: Logistic regression effectively modeled on-time delivery, enabling proactive measures to enhance customer satisfaction.
