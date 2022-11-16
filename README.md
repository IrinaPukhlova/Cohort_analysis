# Cohort_analysis for retail e-store

## Tech Stack
Python / Pandas / Matplotlib / Seaborn / Jupiter Notebook

The main analysis is done in the Jupiter Notebook file [cohort_analysis.ipynb](https://github.com/IrinaPukhlova/AB_testing/blob/main/AB_testing_project.ipynb)

## Goal
We need to find the customer groups that bring us the most and the worst revenue for a retail store. And analyze their behavior to plan marketing activities to improve sales and customer service.

## Metrics and method of analysis
To solve this problem, we perform a cohort analysis with Revenue and ARPU (Average revenue per user) metrics with data from December 1, 2009, to December 9, 2010.

## Cohort Analysis
- Cohort analysis in marketing helps to observe user behavior and track their actions in order to more accurately assess the effectiveness of marketing channels.
- In cohort analysis, the audience is divided into cohorts - groups of users who took the same action in a given period of time.
- For this analysis, you need to define:
  - The user action that puts him in the cohort.
  - Cohort size - the period during which the action was performed.
  - Reporting period - how long you will analyze the cohort.
  - The key metric is the metric you are analyzing.
- Then you need to form cohorts, compare them by the desired metric and analyze the results.

## Definition for analysis in this case
Customer action : purchase

Cohort size : month

Reporting period : 12 months from 01-12-2009 to 01-12-2010

Key metrics : Revenue and ARPU (Average revenue per user)

## Conclusion
- We found the more valuable customer groups that bring us the most revenue in total and per customer - it's "2009-12 cohort"
    - The high performance in Month_0 is most likely due to the Christmas/New Year's sales period, but the high ARPU in the following months suggests that the audience that came to us in this period is of very high quality, and with a constant high level of purchasing power. That's why we need to focus on these tools and actions to attract new customers
    - We can use this cohort as a benchmark for other cohorts, which we will receive in December each year
    - Continue to monitor this group, and if there is a decrease in APRU for several months, additional marketing efforts should be made for buyers from this cohort
    
- We also found another leader in Month_0 -> the "2010-09 cohort":
    - It's worth analyzing the products bought during that period, and if there's no seasonal effect, it's worth looking at the channels that were used to attract new customers in 09-2010 to try and apply those practices to attract customers in the following months
    
- the worst ARPU in "cohort 2010-06" and "2010-05 cohort"
    - They can be used as an anti-benchmark for the other periods
    - It is worth additional marketing incentives for these cohorts to increase sales in the following months
    
- For all future cohorts, we need to improve the number of sales in the next month after the first sale (Month_1) 
    - All old cohorts have the lowest ARPU Month_1 compared to the following months 
    - It is worth adding a marketing tool to increase ARPU in the first month after the first purchase, such as an email newsletter with discounts, recommendations, or giving the customer a personal discount.
