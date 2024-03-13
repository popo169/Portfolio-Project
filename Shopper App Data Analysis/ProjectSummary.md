# Project Summary: Analysis of Part-Time Shopper Job Data
## Background
As a part-time shopper, I embarked on a data analysis project to optimize my earnings and decision-making process while working. Leveraging my background in data science and analytics, I delved into the details of my shopping orders to uncover patterns and insights that could lead to a more effective and profitable approach to my job.


## Project Objectives:
-	Optimizing Earnings: The primary goal was to maximize earnings by making informed decisions on which orders to accept.
-	Efficient Decision-Making: With a constant stream of shopping orders, the aim was to develop a formula or model facilitating quick and accurate decision-making, ensuring valuable opportunities were not missed.
-	Evaluating Previous Performance: Insights into profitability based on location, time periods, and weekdays were derived from historical order data.


## Techniques Used:
1.	Data Collection: A comprehensive dataset was compiled with Excel then converted to CSV file. It contains details such as pay, batch size, location, store, items, and timestamps for each shopping order.
2.	Data Preprocessing: Rigorous preprocessing was undertaken to refine and prepare the data for analysis. This included handling missing values, type conversions, and the creation of new informative features.
3.	Exploratory Data Analysis (EDA): EDA played a pivotal role in uncovering underlying trends and patterns. Visualizations were utilized to reveal correlations, trends, and potential outliers.
4.	Features Engineering: New features such as active time, pay rate, and desired pay were crafted to extract valuable insights and facilitate the development of predictive models.
5.	Regression Models: Regression modeling emerged as the optimal approach for formulating a decision-making model. Various regression techniques were explored, integrating diverse independent variables to predict active time and optimize order acceptance.
6.	Model Evaluation: Performance metrics including R-squared, Adjusted R-squared, AIC, BIC, and F-Statistics were employed to gauge model effectiveness and identify optimal strategies.
7.	Decision Support System: Leveraging the developed models and insights, a decision support formula was formulated to guide order acceptance based on predicted active times.

## Key Findings:
-	Insights from Simplest Model: The basic model considering pay and item number yielded crucial insights.
-	Formula:
  1.	With the simplest model, the minimum active time is 26.9 minutes
  2.	Total estimated active time = 26.9 + Display_km * 1.6 + item * 1.7
  3.	To simplify calculation, I would estimate active time = 27 + (Display_km + item) * 1.5
  4.	From the result, I should only accept orders at least 9 (desire pay rate $18 * 0.5 hr)
  5.	To judge if I should accept the order, I will calculate: Pay - Display KM * 0.1 * 2 (round trip) - Desire Pay Rate * Estimated Active Time = Pay - Display KM * 0.1 * 2 - 18 * (27 + (Display_km + item) * 1.5) / 60 If it is positive, I should take the order.
-	Average Active Time: The mean active time for orders was found to be approximately 80 minutes.
-	Time-Based Trends: A dip in orders was observed between 10:00 to 12:00, indicating a potential period of lower demand.
-	Impact of Batch Size: Batch size 3 emerged as the most profitable, while batch size 2 exhibited the least profitability.
- Profitable Days and Times: Sunday, Monday, and Tuesday stood out as more profitable, particularly during the dinner period.

## Challenges:
-	Biased Data: The dataset displayed some biases, potentially affecting the accuracy of the models.
-	Small Dataset: With a limited number of records, the dataset's size posed challenges in achieving robust model performance.
-	Feature Engineering: Creating informative features from the existing dataset can be both an art and a science. Determining which features are relevant and how to transform them effectively to enhance model performance is a significant challenge.
-	Model Selection: Choosing the most appropriate regression model among various options can be daunting. Comparing different models based on metrics such as R-squared, AIC, BIC, and F-statistics requires a deep understanding of their implications and trade-offs.
-	Evaluation Metrics: Understanding the nuances of evaluation metrics such as MSE, R-squared, and F-statistics, and interpreting their values in the context of the project objectives posed a challenge in assessing model performance accurately.

## Future Steps:
-	Model Refinement: Continuous refinement and updates to the decision support system with fresh data and enhanced models.
-	Exploration of Advanced Techniques: Delve into advanced machine learning methods such as ensemble methods and neural networks for further optimization.
-	Community Collaboration: Collaborate with fellow shoppers to establish a platform for shared insights and strategies.
-	Analysis of Feature Interactions: Dive deeper into feature interactions and correlations to craft an enhanced predictive model.

In conclusion, this project has empowered informed, data-driven decision-making, optimized earnings, and enhanced the overall shopping experience. Leveraging the robust tools of data science, new avenues for success within the gig economy have been unlocked.
