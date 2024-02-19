# California House Prediction

---

## Overview
This project focuses on predicting house prices in California, set against the backdrop of the 1990 housing market scenario. With property prices reaching high levels during this period, this analysis offers insights into real estate investment strategies, aiding in identifying profitable opportunities.

---

## Contents

1. **Business Problem Understanding**
2. **Data Understanding**
3. **Exploratory Data Analysis**
4. **Data Preparation**
5. **Modeling**
6. **Conclusion and Recommendation**

---


## Business Understanding

**Context:**
In 1990, California experienced a significant surge in property prices, influenced by factors like a strong economy, rapid population growth, and limited land availability. This project aims to understand these dynamics and provide a data-driven approach to pricing properties effectively.

**Challenge:**
The challenge lies in accurately predicting house prices in various Californian locales, considering multiple factors that influence these prices, such as location, property type, and economic conditions.

---

## Data Understanding

*(This project utilizes a comprehensive dataset that represents the housing market in California as of 1990. The dataset, sourced from the California Census data, includes a wide range of features such as median house values, median income, housing median age, total rooms, total bedrooms, population, households, and proximity to the ocean. Each record in the dataset corresponds to a district and includes aggregated data about the households within that district. The richness of this dataset allows for an in-depth analysis of housing prices, taking into account various socio-economic and geographic factors that might influence these prices. Understanding these nuances is crucial for developing accurate predictive models and making informed decisions in the real estate market)*

---

## Exploratory Data Analysis

*(The Exploratory Data Analysis (EDA) phase of this project focused on uncovering patterns, anomalies, and relationships within the California housing dataset. Initial steps involved a thorough examination of data distributions, where we observed the range and common values for crucial features like median house values, median income, and age of houses. Histograms and scatter plots were extensively used to visualize these aspects, revealing, for instance, a skewed distribution in house values, suggesting a concentration of more affordable houses compared to high-value properties.

Correlation analysis was another critical component, where we examined how different variables relate to the median house value. Notably, median income emerged as a strong predictor, indicating a direct correlation with housing prices. Geospatial analysis was also conducted to understand regional variations in housing prices, highlighting areas with exceptionally high or low prices. This analysis was complemented by heatmaps to visualize high-density clusters.

The EDA also involved identifying outliers and handling missing data, ensuring the integrity and reliability of the subsequent modeling process. Through these explorations, we gained valuable insights into the factors that drive house prices in California, setting a strong foundation for building our predictive models.)*

---

## Data Preparation

*(In the data preparation stage, we performed several key steps to ensure the dataset was primed for effective modeling. This involved cleaning the data by addressing missing values, where we opted for imputation strategies based on the nature of each feature. We also conducted feature engineering to enhance the dataset's predictive power, creating new variables that better represented the underlying real estate dynamics. To address potential skewness in the data, we applied normalization techniques, ensuring that all features contributed equally to the model. Finally, the dataset was split into training and test sets, providing a robust framework for both training our models and evaluating their performance objectively.)*

---

## Modeling

*(In the modeling stage of our project, we selected CatBoost Regressor as our final model due to its efficiency and high performance for large datasets. catboost is A one-dimensional array of categorical columns indices (specified as integers) or names (specified as strings). This array can contain both indices and names for different elements. If any features in the cat_features parameter are specified as names instead of indices, feature names must be provided for the training dataset. Therefore, the type of the X parameter in the future calls of the fit function must be either catboost.Pool with defined feature names data or pandas.DataFrame with defined column names.

We fine-tuned the CatBoost model's hyperparameters to optimize its performance, using a combination of grid and random search techniques for the best results. The model demonstrated excellent predictive accuracy in our validation tests, with a significant reduction in both bias and variance compared to initial baseline models. Its ability to efficiently process large amounts of data and accurately predict housing prices made it an ideal choice for our analysis.)*

---

## Conclusion and Recommendation
#Conclusion
1. The benchmark model uses catboost for the California House prediction model.
2. The model achieved an R2 value of about 0.8253, indicating that the model explained about 82.6% of the variance in house prices.
3. The average MAPE is about 18.09%, indicating that the predictions deviate on average 18.096% from the actual price.
4. With this model, businesses can forecast house prices more accurately, thus aiding investment decision-making and pricing strategies.
5. Without this model, businesses may rely on manual or heuristic analyses, which may become less accurate and more risky.

#Recomendation
1. Ensure training and testing data is representative and up-to-date.
2. Dedicate time to regular maintenance and upgrades to maintain model accuracy.
3. Explore deeper feature engineering to address outliers and market segmentation.
4. Consider using ensemble models to improve prediction accuracy and reliability.
5. Conduct continuous testing with current market data to ensure the model remains relevant to current conditions.
---


