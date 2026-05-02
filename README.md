# 📊 Global Ads Performance Analysis
 
A comprehensive exploratory data analysis (EDA) of global digital advertising campaign performance across platforms, campaign types, industries, and geographies — covering a full year of data (Jan 2024 – Dec 2024).
 
---
 
## 📁 Project Structure
 
```
├── Analysis.ipynb                    # Main Jupyter Notebook with full EDA
├── global_ads_performance_dataset.csv  # Raw dataset
└── README.md                         # Project documentation
```
 
---
 
## 📌 Objective
 
To analyze global ad campaign data and uncover actionable insights on:
- Which platforms deliver the best return on ad spend (ROAS)
- Which campaign types are most cost-efficient
- Which industries generate the highest revenue
- Where budget is being wasted and how to optimize it
---
 
## 📦 Dataset Overview
 
| Feature | Description |
|---|---|
| `date` | Date the campaign ran |
| `platform` | Ad platform (Google Ads, Meta Ads, TikTok Ads) |
| `campaign_type` | Type of campaign (Search, Display, Video, Shopping) |
| `industry` | Business category (SaaS, EdTech, E-commerce, Healthcare, Fintech) |
| `country` | Geographic location |
| `impressions` | Number of times the ad was shown |
| `clicks` | Number of user interactions |
| `ad_spend` | Amount of money spent on ads |
| `conversions` | Number of desired actions completed |
| `CTR` | Click Through Rate |
| `CPC` | Cost Per Click |
| `CPA` | Cost Per Acquisition |
| `ROAS` | Return on Ad Spend |
| `revenue` | Revenue generated |
 
---
 
## 📊 Key Metrics (Overall)
 
| Metric | Value |
|---|---|
| Total Impressions | 185,254,234 |
| Total Clicks | 7,132,816 |
| Total Conversions | 326,812 |
| Total Ad Spend | $11,108,749 |
| Total Revenue | $54,183,331 |
| Total Profit | $43,074,582 |
| Overall ROAS | 4.88x |
| Overall CTR | 3.85% |
| Average CPA | $33.99 |
| Average CPC | $1.56 |
 
---
 
## 🔍 Analysis Performed
 
### 1. Data Cleaning & Validation
- Null value detection and handling
- KPI validation (CTR, CPC, CPA, ROAS cross-checked against raw inputs)
- Duplicate removal
- Zero value analysis
- Date parsing and feature engineering (month, day, year, profit)
### 2. Exploratory Data Analysis (EDA)
- ROAS by Platform
- ROAS by Campaign Type
- Revenue Trend Over Time
- ROAS Trend Over Time
- Ad Spend vs Revenue Trend
- Platform Profitability (Profit = Revenue − Ad Spend)
- Wasteful Campaigns (High Spend, Low Conversions)
- Most Cost-Efficient Campaigns (Low CPA)
- Industry-wise ROAS Comparison
---
 
## 💡 Key Insights
 
- 🟢 **TikTok Ads** is the most efficient platform — ROAS of **9.54** and CPA of **$21.67**, generating **$17.57M profit** on just $2.65M spend
- 🔴 **Google Ads** consumed **57% of total budget** ($6.35M) but delivered the lowest ROAS of **4.11** and highest CPA of **$48.43**
- 🟢 **Search campaigns** outperform all other types with a ROAS of **5.31** and lowest CPA of **$31.64**
- 🔴 **229 campaigns** with above-average CPA are burning **$2.13M (19.2% of total spend)**
- 🟡 **SaaS** leads industry ROAS at **5.04**, while **Fintech** lags at **4.48**
- 🔵 Daily revenue swings from a peak of **$493,585** to a low of **$3,174** — a 155x gap indicating high volatility
---
 
## ✅ Recommendations
 
1. **Rebalance budget toward TikTok Ads** — 2x more efficient than Google Ads per dollar spent
2. **Scale Search campaigns** — best ROAS (5.31) and lowest CPA ($31.64) across all campaign types
3. **Audit 229 wasteful campaigns** — reclaim $2.13M in inefficient spend
4. **Focus on SaaS, EdTech, and E-commerce** — all deliver ROAS above 5.0
5. **Prioritise India and UAE markets** — highest ROAS efficiency among top-revenue countries
6. **Set CPA guardrails** — auto-flag any campaign exceeding $70 CPA (2x average)
7. **Implement dayparting** — reduce the extreme daily revenue volatility (155x swing)
---
 
## 🛠️ Tech Stack
 
| Tool | Purpose |
|---|---|
| Python 3 | Core programming language |
| Pandas | Data manipulation and analysis |
| NumPy | Numerical computations |
| Matplotlib | Data visualization |
| Seaborn | Statistical data visualization |
| Jupyter Notebook | Interactive analysis environment |
 
---
 
## 🚀 Getting Started
 
### Prerequisites
```bash
pip install pandas numpy matplotlib seaborn jupyter
```
 
### Run the Notebook
```bash
git clone https://github.com/your-username/global-ads-performance-analysis.git
cd global-ads-performance-analysis
jupyter notebook Analysis.ipynb
```
 
---
 
## 📝 Conclusion
 
This analysis of 364 days of global advertising data reveals a portfolio generating a healthy **overall ROAS of 4.88x** and **total profit of $43.07M**. However, significant inefficiencies exist — primarily in Google Ads and Shopping campaigns. By eliminating wasteful spend, rebalancing platform allocation toward TikTok, and scaling high-performing Search campaigns, the business can significantly improve ROAS and profit margins without increasing the overall budget.
 
---
 
## 📄 License
 
This project is open source and available under the [MIT License](LICENSE).
 
---
 
## 🙋‍♂️ Author
 
Made with ❤️ for data-driven advertising insights.  
Feel free to ⭐ the repo if you found this useful!
