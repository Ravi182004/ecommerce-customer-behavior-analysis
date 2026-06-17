E-Commerce Customer Behavior Analysis

Exploratory Data Analysis · Customer Segmentation · Churn Risk · Retention Strategy

Project Overview
This project performs an in-depth analysis of customer behavior on an e-commerce platform using a dataset of 350 customers. The goal is to uncover spending patterns, identify key customer segments, classify churn risk, and propose targeted retention strategies.
A full 13-page Strategic Report (CustomerBehaviourReport.pdf) is included alongside the Jupyter Notebook.

 Dataset

ColumnDescriptionCustomer IDUnique customer identifierGenderMale / FemaleAgeCustomer age (26–43)CityNew York, LA, Chicago, SF, Miami, HoustonMembership TypeGold / Silver / BronzeTotal SpendTotal amount spent ($)Items PurchasedNumber of items boughtAverage RatingCustomer rating (1–5)Discount AppliedWhether a discount was usedDays Since Last PurchaseRecency of activitySatisfaction LevelSatisfied / Neutral / Unsatisfied


Key Findings

Gender

Male customers outspend female customers on average ($986.93 vs $703.83)
Males also purchase more items (14.44 vs 10.76) and rate higher (4.31 vs 3.73)

Membership Tier

Gold members spend nearly 3× more than Bronze members ($1,311 vs $473)
Bronze members have the lowest satisfaction (3.33/5) and highest churn concentration


Geography

San Francisco and New York are top-performing markets (avg. spend $1,050–$1,165)
Houston is the weakest market at just $446.89 average spend — a 160%+ gap vs New York


 Age

Customers aged 28–30 are the highest spenders with the most purchases
This group is still building brand loyalty — a key window for retention investment


Satisfaction

Distribution: ~127 Satisfied · ~108 Neutral · ~117 Unsatisfied
Unsatisfied customers cluster among Bronze/Silver members in Chicago, Houston, and Miami



Churn Risk Classification

Customers were classified based on Days Since Last Purchase:

Risk LevelThresholdCount% of Base Low (Active)≤ 30 days22664.6% Medium (At-Risk)31–90 days12435.4% High (Churned)> 90 days00%


35.4% of customers are at medium churn risk — the single biggest revenue recovery opportunity.




Retention Strategies

SegmentRiskStrategyBronze & Silver (Medium Risk)⚠️ MediumRe-engagement campaign — personalized emails, limited discounts, feedback surveysGold Members (Low Risk)✅ LowVIP loyalty perks — early access, surprise gifts, referral bonusesHouston & Chicago⚠️ Medium–HighGeo-targeted marketing — local influencer campaigns, city-specific promotionsAll Medium Risk⚠️ MediumPersonalized reactivation — cart reminders, product recommendations


Tech Stack


Python 3
Pandas — data loading, cleaning, feature engineering
NumPy — numerical operations
Matplotlib & Seaborn — data visualization
Scikit-learn — LabelEncoder for categorical encoding
