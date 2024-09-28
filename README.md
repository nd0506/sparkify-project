# Sparkify Project: Predicting At-Risk Users

## Project Overview

Sparkify is a music streaming app facing a critical challenge: identifying at-risk users who are likely to cancel their subscription. Like many businesses, retaining users is essential for Sparkify's growth and profitability. By identifying these users early, Sparkify can implement targeted promotions to increase retention and ultimately boost revenue.

In this project, we leverage user event data from the Sparkify app to build a machine learning model that predicts at-risk users. The dataset includes key information such as:

* User Profile: User ID, name, gender, location, subscription level, etc.
* User Behavior: Actions within the app (e.g., play song, downgrade, upgrade, cancel subscription, thumbs up/down), session details, song play time, and more.
* Timestamp: The time each event occurred.

**Strategy to predict At-Risk Users:**

* **Data Processing & Cleaning:** Remove invalid or missing data to ensure data quality.
* **Exploratory Data Analysis (EDA):** Analyze the data to uncover patterns and identify key features for prediction.
    * **Churn Definition:** Users who cancel their subscription are labeled as "churn" (1), while others are labeled as "non-churn" (0).
    * **Behavioral Analysis:** Compare behaviors between churned and non-churned users to select relevant features.
* **Feature Engineering:** Select and create the most predictive features for the model.
* **Modeling:** Test various machine learning models to find the best-performing one.
* **Evaluation:** Use the F1-score to evaluate model performance, ensuring a balance between precision and recall.

## Project Report: [Read on Medium](https://medium.com/@nhungdnn.06/spotting-at-risk-users-a-data-driven-approach-to-early-identification-bf5f1a2a03cb)

## Repository Structure
`mini_sparkify_event_data.json.zip` : user event data. This project is using this dataset to build the model to predict churned users.
`Sparkify.ipnb`: Jupyter Notebook file that contains codes for data processing, modeling and model evaluation.
