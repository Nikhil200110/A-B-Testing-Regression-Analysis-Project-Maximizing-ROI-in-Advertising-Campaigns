# A-B-Testing-Regression-Analysis-Project-Maximizing-ROI-in-Advertising-Campaigns
Leveraged statistical hypothesis testing and predictive analytics to evaluate Facebook and AdWords campaigns, identifying the most cost-effective platform and optimizing strategies to maximize conversions and ROI for targeted.
# Ad Campaign Analysis: Facebook vs. AdWords

## Project Overview

This project aims to analyze and compare the effectiveness of two advertising campaigns run on Facebook and AdWords over the year 2019. The primary objective is to determine which platform yields better results in terms of clicks, conversions, and cost-effectiveness. This analysis will help optimize advertising strategies and maximize return on investment (ROI) for future campaigns.

---

## Problem Statement

As a marketing agency, our goal is to maximize ROI for our clients. We conducted ad campaigns on Facebook and AdWords and needed to identify the platform that performs better. By understanding the strengths and weaknesses of each platform, we can allocate resources efficiently and improve campaign outcomes.

**Research Question:**
Which ad platform is more effective in terms of conversions, clicks, and overall cost-effectiveness?

---

## Tools and Libraries Used

- **Data Manipulation and Analysis:** Pandas, NumPy
- **Data Visualization:** Matplotlib, Seaborn
- **Statistical Analysis:** Scipy, Statsmodels
- **Machine Learning:** Scikit-learn (Linear Regression)
- **Others:** Warnings, Cointegration Testing

---

## Dataset Description

The dataset contains daily performance metrics for the Facebook and AdWords campaigns for the year 2019, with a total of 365 rows. Key features include:

- **Date:** Campaign date (from January 1st to December 31st, 2019).
- **Ad Views:** Number of times the ad was viewed.
- **Ad Clicks:** Number of clicks received on the ad.
- **Ad Conversions:** Number of conversions resulting from the ad.
- **Cost per Ad:** Cost of running the campaign.
- **Click-Through Rate (CTR):** Ratio of clicks to views.
- **Conversion Rate:** Ratio of conversions to clicks.
- **Cost per Click (CPC):** Average cost per click.

---

## Steps Undertaken

### 1. **Data Cleaning and Preparation**

- Converted the `Date` column to datetime format for temporal analysis.
- Processed percentage and monetary columns to numeric format for analysis.
- Ensured all columns had appropriate data types for computation.

### 2. **Exploratory Data Analysis (EDA)**

- **Distribution Analysis:** Used histograms to analyze the distribution of clicks and conversions for both platforms. Found that Facebook ads had a higher frequency of conversions compared to AdWords.
- **Category Analysis:** Categorized conversions into ranges (e.g., less than 6, 6-10) to analyze frequency. Facebook showed more high-conversion days than AdWords.
- **Correlation Analysis:** Assessed the relationship between clicks and conversions. Found a strong correlation (0.87) for Facebook and a moderate correlation (0.45) for AdWords.

### 3. **Hypothesis Testing**

- **Hypothesis:** Facebook ads result in higher conversions than AdWords ads.
- Performed a T-test comparing the mean conversions of Facebook and AdWords.
- Results:
  - Mean conversions: Facebook (11.74), AdWords (5.98).
  - T-statistic: 32.88, p-value: 9.35e-134.
  - Conclusion: Strong evidence to reject the null hypothesis, confirming that Facebook ads are more effective in driving conversions.

### 4. **Regression Analysis**

- Built a Linear Regression model to predict Facebook ad conversions based on clicks.
- Model Evaluation:
  - R2 Score: 76.35%
  - Mean Squared Error: Low, indicating good model fit.
- Insights:
  - Predicted conversions for 50 clicks: 10.37
  - Predicted conversions for 80 clicks: 16.56

### 5. **Temporal Analysis**

- **Weekly Analysis:** Found higher conversions at the beginning of the workweek (Monday and Tuesday).
- **Monthly Trends:** Identified months with lower conversions (e.g., February, May) and those with higher conversions.

### 6. **Cost Analysis**

- Calculated Cost Per Conversion (CPC) for each month. Found lower CPC in May and November, suggesting these months were cost-effective for advertising.

### 7. **Cointegration Testing**

- Tested for a long-term equilibrium relationship between advertising spend and conversions.
- Results:
  - Significant cointegration found, indicating a stable, proportional impact of budget changes on conversions over time.

---

## Key Findings

1. Facebook ads outperformed AdWords in terms of conversions, clicks, and ROI.
2. Strong correlation (0.87) between Facebook ad clicks and conversions suggests its high effectiveness.
3. Facebook showed higher high-conversion days compared to AdWords.
4. Temporal analysis revealed optimal advertising periods (e.g., Mondays and November).
5. Regression analysis provided actionable predictions for expected conversions based on ad clicks.
6. CPC analysis identified cost-effective months for budget allocation.
7. Cointegration results suggest that increasing ad spend on Facebook leads to proportional increases in conversions.

---

## Business Impact

This analysis enables informed decision-making for future campaigns, including:

- Allocating more resources to Facebook campaigns to maximize ROI.
- Optimizing ad spend during cost-effective months.
- Utilizing regression insights to set realistic campaign goals.
- Understanding temporal trends to schedule ads during high-conversion periods.

---

## Conclusion

By leveraging data analysis, statistical testing, and predictive modeling, this project provided actionable insights into optimizing ad campaign strategies. The findings highlight Facebook’s superior performance in driving conversions, offering a roadmap for improving advertising effectiveness and ROI.

