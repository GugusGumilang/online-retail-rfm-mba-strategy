# 🛒 Optimizing E-Commerce Customer Value
**RFM Segmentation & Shopping Cart Analysis for Retail Retention Strategies in the UK**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

## 📌 Problem Statement
The local market (UK) is the company’s primary revenue driver, but this organic ecosystem is facing the threat of customer value leakage. The main issue isn’t a lack of transaction volume, but rather growth inefficiencies and churn risk. The company has failed to drive mid-tier customers (*Loyalists*) to upgrade to top-tier customers (*Champions*), and operates without a safety net for high-value customers who are beginning to show signs of inactivity (*At Risk*). Without tactical intervention, these organic assets will gradually migrate into the inactive segment (*Hibernating*), undermining the company’s core revenue foundation.

## 🧠 Strategic Context
Many operational decisions backfire because they’re trapped by the illusion of aggregate metrics. If we critically filter out transaction anomalies from the *Whales* (foreign B2B distributors that skew average revenue) and disregard dormant accounts (*Hibernating*) that incur high reactivation costs (*low ROI*), the true health of the company’s business relies entirely on the domestic retail market. Therefore, the most rational strategy is to build the independence of the local ecosystem by maximizing *Customer Lifetime Value* (CLV) from the active customer segment.

## 🚀 Business Objectives
This analysis project formulates an *actionable* framework through three main pillars:
1. **Defend the Core:** Design a proactive retention system to secure the *Champions* segment.
2. **Upsell the Mid-Tier:** Optimize *Average Order Value* (AOV) in the *Loyalists* segment through *cross-selling* and *bundling* strategies validated by *Market Basket Analysis* (MBA) algorithms.
3. **Intercept the Exit:** Intercept customers in the *At Risk* segment with personalized reactivation campaigns before they permanently churn.

## 🛠️ Methodology & Data
<p className="text-sm text-muted-foreground mb-6 italic">
  Dataset: <a href="[https://www.kaggle.com/datasets/carrie1/ecommerce-data](https://archive.ics.uci.edu/dataset/352/online+retail)" target="_blank" rel="noopener noreferrer" className="text-emerald-400 font-mono hover:text-emerald-300 hover:underline transition-colors duration-200">Online_Retail_UK_2011.csv</a> (~541k+ rows)
</p>

1. **Data Sanity Check:** Cleaning transaction anomalies (returns & *guest checkouts*) to obtain unbiased fundamental data.
2. **Macro & Geographical EDA:** Separating domestic retail customer profiles from international wholesale anomalies (*Whales*).
3. **RFM Profiling (Quintile Method):** Calculating *Recency, Frequency, Monetary* values to classify customers into strategic segments.
4. **Market Basket Analysis (Apriori Algorithm):** Measuring *Support, Confidence*, and *Lift* to design *bundling* packages based on historical probabilities.

## 📊 Key Findings
* **The Whale Vulnerability:** Historically, the top 10% of customers have accounted for >61% of total revenue, but the majority are European B2B players. Focusing on this figure masks the weaknesses of the UK retail market.
* **Missed Cross-Selling Opportunities:** Although the UK market accounts for the highest transaction volume, shopping carts are often suboptimal. There is significant room to increase transaction value without having to acquire new customers.
* **Product Synergy Validated:** MBA analysis found a strong correlation between similar product variants (e.g., *Jumbo Bag Pink Polkadot* and *Red Retrospot* have a **Lift of 7.16**). These combined purchases are proven not to be coincidental, but rather a consumption pattern that the system can replicate.

## 💡 Strategic Recommendations
1. **Calibrated VIP Program:** Prioritize incentives such as priority shipping or exclusive early access to new products to retain the UK *Champions* segment.
2. **Smart Bundling Engine:** Implement recommendation features on the *website* using product pairing matrices from MBA results to encourage *Loyalists* to add items to their carts.
3. **Targeted Win-Back:** Use the product catalog with the highest *Lift* value as campaign material specifically for the *At Risk* segment, offering items that are statistically most relevant to them.
