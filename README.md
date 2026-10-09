# 🛒 End-to-End Customer Intelligence Pipeline

## Why I Built This
While studying data analytics, I realized there's a massive gap between just writing a quick script and actually driving real business decisions. You always hear data scientists complain about messy data, and analysts struggle when data isn't modeled correctly in the first place. 

I wanted to understand the *entire* ecosystem. How does a company actually take raw, messy transactions, transform them into a reliable database, build dashboards, and use machine learning to predict user behavior? 

So, I decided to play the role of Data Engineer, Data Analyst, and Data Scientist all at once. I grabbed a messy dataset of over half a million retail transactions to see if I could clean it up, visualize the business's health, and actually predict which customers were about to churn.

## The Tech Stack I Used
- **Cloud Database:** Google BigQuery (because local CSVs just don't cut it for half a million rows!)
- **Data Engineering:** SQL (cleaning anomalies, engineering new features)
- **Machine Learning:** Python via Google Colab (pandas, scikit-learn, Random Forest)
- **Business Intelligence:** Power BI (DAX, relational modeling, and interactive dashboards)

##  How I Built It 
1. **Wrangling the Mess:** I started by uploading 540,000+ rows of raw, unstructured retail transaction data straight into a Google BigQuery data warehouse.
2. **Cleaning House (ETL):** I wrote SQL scripts to filter out the business anomalies (like canceled orders and missing customer IDs) and engineered a few new metrics, like calculating the total sales per transaction.
3. **Predicting the Future:** I connected a Python environment directly to my clean cloud data. Using RFM (Recency, Frequency, Monetary) analysis, I trained a Random Forest classification model. The goal? Predict if a customer was at risk of churning based *only* on their spending habits. (It hit a 64% baseline accuracy—not bad for just using historical transaction data!)
4. **Bringing it to Life:** I pushed those machine learning predictions back into BigQuery and hooked up Power BI to the live cloud database. I built an interactive dashboard to track executive KPIs, cohort retention, and most importantly, generate an actionable "hit list" of high-risk customers.

## 📊 The Real-World Business Impact
I personally believe data is only useful if it helps the business. One way data can help a business is by identifying high-value customers who are flagged as churn risks. I believe that this pipeline actually gives a marketing team something to work with. They can send targeted retention campaigns to the right people before they leave, thereby directly protecting Monthly Recurring Revenue and Customer Lifetime Value!
