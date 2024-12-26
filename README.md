# Fresh-Cart-Ads-Campaign-Analysis

# Business Overview/Problem
FreshCart, like many e-commerce platforms, relies heavily on online advertising to acquire new customers and retain existing ones. 
However, in the midst of an increasingly competitive market and fluctuating ad costs, the company has identified two main challenges:
 
A. Inefficient Ad Spend: The company suspects that not every dollar spent on digital advertising is yielding the desired ROI. 
Some campaigns may be costing more than they return in revenue.
 
B. Identifying Effective Channels: With multiple platforms available for advertising, from search engines to social media,
FreshCart is finding it challenging to determine which channels offer the best return on investment.
 
As the competition in the online grocery sector has skyrocketed, the cost of customer acquisition is rising. 
FreshCart is looking for the most efficient way to save cost and optimize its digital ad spend.


# Rationale for the Project
Marketing analytics is the process of using data to understand how marketing campaigns perform and find how to improve them. It helps businesses know which strategies work best, where to spend money, and how to better connect with customers.
By analyzing the performance of different advertising channels, FreshCart can:
 
A. Identify demography or regions where the ads perform best.
 
B. Understand which campaigns are under or over-funded and reallocate funds accordingly.
 
C. Determine which platforms or strategies yield the highest return

# Aim of the Project
The aim of this project is to analyze FreshCart past advertising data and create a strategy to optimize their digital ad spending. The specific objectives are:
 
A. Evaluate the effectiveness of current advertising campaigns across platforms.
 
B. Identify top-performing channels for advertising.
 
C. Assess demography engagement and conversion rates.
 
D. Recommend strategies for better budget allocation.

# Project Scope
A. Data Integration: Connect Excel to Power BI
 
B. Data Cleaning: Clean data and transform to the required format in Power Query
 
C. Data Modelling: Create data models in Power BI
 
D. Reporting & Recommendations: Write report of the analysis and provide recommendations.
 
E. Analysis & Visualization: Analyze data, define KPIs, and visualize it in Power BI

# Steps: The steps used in perfoming these analysis are as follows

## Data Collection and Preparation: 
- I successfully obtained the dataset from AMDARI’s learning site in Excel format, imported into Power BI and then transformed, I checked for errors, inconsistencies, duplication,
missing values, and blanks, thereby improving data quality.
- Date Table Creation: I createded a Date Table to help build a data model that allows for precise tracking of ad performance across time.
- DAX Measures Creation: Using Power BI, I created DAX measures to determine key performance indicators (KPIs) required for maximizing ad campaign efficiency across different platforms.
### 1. Cost Per Conversion 
= Var Cost=SUM(ad_campaign_data[Cost])
Var Conversion=SUM(ad_campaign_data[Conversions])
Return
DIVIDE(Cost,Conversion,0)

### 2. Conversion_Rate =
Var Conversion= SUM(ad_campaign_data[Conversions])
Var Click= SUM(ad_campaign_data[Clicks])
Return
DIVIDE( Conversion, Click, 0)

### 3. CTR =
Var Clicks = SUM(ad_campaign_data[Clicks])
Var Impressions = SUM(ad_campaign_data[Impressions])
Return
DIVIDE(Clicks,Impressions,0)

### 4. ROAS =
Var Revenue = SUM(ad_campaign_data[Sales Revenue])
Var Cost = SUM(ad_campaign_data[Cost])
Return
DIVIDE(Revenue,Cost,0)

### 5. TOTAL ADS SPENT = SUM(ad_campaign_data[Cost])

### 6. TOTAL REVENUE = SUM(ad_campaign_data[Sales Revenue])
Visualization: I used several charts to comprehend the data and provide insights that aided data-driven decision-making.

# Findings

- Twitter and YouTube have been the top 2 platforms with the best conversion rate with 6.79% and 6.41% respectively. 
This shows that the audience have been very receptive to Fresh Cart's ads
- Ads on YouTube generated the most sales (29.4k) with Twitter following closely at 28.1k
- While Twitter is almost generating as much sales as YouTube, its return on Ad spent (ROAS) is considerably lower.
  This means the company is spending more on Twitter to generate similar sales revenue that twitter will give
- YouTube's cost pert conversion is significantly lower ($2.72) than Twitter ($ 14.21) despoite having similar conversion rates.
 This indicates that YouTube is nore cost effective for customer acquisition
- YouTube has generated more returns despite running fewer ad campaigns(12 in total) than Twitter (which had 9), with even shorter duration when compared to Twitter.
  This means Fresh Cart has invested more time and resources into Twitter in terms of campaign frequency and duration while YouTube yielded better returns

# Insights:
## YouTube or Twitter:Which platform is the most effective platform for Ad Campaigns?
YouTubehas been the most effective platform for Fresh Cart's advertising for the following treasons
1.  High Conversion Rate: Both YouTube and Twitter have conversion rate that exceed the e-commerce industry's
  average of 1-3%, this indicates that their audience are highly receptive to FreshCart'ads.
2. Lowest Cost Per Conversion:YouTube's Cost Per Conversion is significantly lower than Twitter, which is more than 5 times higher than YouTube.
   This indicates the cost effectiveness of the platform in converting viewers into customers
3. Impressive ROAS: The return on Ads spend (ROAS) for YouTube stands at impressive rrate 1298.84%. This means that Fresh Cart gets $12.99 in return for every
   dollar spent on YouTube advertising. This is sinificanrtly higher than the ROAS on other platforms including Twitter (420.18%)
4. Efficiency: YouTube generates more sales than Twitter even with fewer campaign(9 vs 12) and shorter ad durations.

   
Considering all these factors, YouTube is the mosty effective platform for Fresh Cart's advertising. it offers a combination of high conversion rates,
 maximises sales revenue, an impressive ROAS, and the lowest cost per conversion, all while requiring fewer campaign and shorter durations.

## Which is the least effective platform for Ads campaign?
Based on this analysis, Google Ads has been the least effective or potentialkly overfunded platform for Fresh Cart's advertising for the following reasons
1. Google Ads has the lowest conversion rate at 4.62%, which is notably lower than the conversion rates of other platforms
2. Highest Cost Per Conversion: Google Ads also has the highest Cost Per Conversion at $35, making it the most expensive platform in terms of acquiring a customer
3. Least ROAS: Google Ads is at the bottonm in terms of ROAS with 180.88%. While this is still a positive return, it's considerably lower than the other platform
4. Google Ads generated sales revenue of $8.07k, which is higher than instagram but significantlt lower than YouTube, Twitter and Facebook.




