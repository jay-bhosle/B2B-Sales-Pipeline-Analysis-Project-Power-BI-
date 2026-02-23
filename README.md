📊 B2B Sales Analytics Dashboard (Power BI)

An end-to-end Power BI project analyzing B2B sales pipeline performance for a computer hardware company.

This dashboard evaluates:

Sales performance

Win rates

Revenue trends

Product effectiveness

Pipeline efficiency

🖼 Image 1 — Project Overview (Pre-Dashboard Page)
🔎 Project Overview

This project analyzes B2B sales pipeline data using Power BI to:

Evaluate sales team and agent performance

Identify lagging sales agents

Analyze quarter-over-quarter revenue trends

Assess product win rates and pipeline efficiency

Provide actionable insights to improve revenue outcomes

🧹 Data Quality Issues Identified & Resolved

Duplicate records in dimension tables

Missing categorical values (industry, region, sales agent)

Inconsistent naming conventions for sales stages and regions

Invalid opportunity values (null or zero)

Date inconsistencies between created and closed dates

📐 Key DAX Measures
Base Measures
Total Opportunities = COUNT(Sales[Opportunity ID])
Total Pipeline Value = SUM(Sales[Opportunity Value])

Revenue & Performance
Won Opportunities = CALCULATE([Total Opportunities], Sales[Stage] = "Closed Won")
Won Revenue = CALCULATE([Total Pipeline Value], Sales[Stage] = "Closed Won")
Open Pipeline Value = CALCULATE([Total Pipeline Value], Sales[Stage] IN {"Prospecting","Proposal"})

Conversion Metrics
Win Rate = DIVIDE([Won Opportunities], [Total Opportunities])
Average Deal Size = DIVIDE([Won Revenue], [Won Opportunities])

Time Intelligence
QoQ Revenue Growth % =
VAR PrevQ = CALCULATE([Won Revenue], DATEADD('Date'[Date], -1, QUARTER))
RETURN DIVIDE([Won Revenue] - PrevQ, PrevQ)
<img width="1920" height="1080" alt="Screenshot (167)" src="https://github.com/user-attachments/assets/2fab97fa-0bde-4fd2-9ee6-2e8eabe5a502" />
167

🖼 Image 2 — Executive Overview Dashboard
📌 KPI Summary
KPI	Value
Won Revenue	10M
Win Rate	63%
Open Pipeline Value	3M
QoQ Revenue Growth	39%
📈 Insights

Strong overall win rate (0.63)

Healthy open pipeline supporting future revenue

Positive quarterly revenue growth

Revenue concentration among top-performing agents
<img width="1920" height="1080" alt="Screenshot (168)" src="https://github.com/user-attachments/assets/32ea752a-58c5-4ca2-af29-f250ab285997" />
168

🖼 Image 3 — Sales Team Performance
👥 Agent-Level Analysis
Metrics Evaluated:

Total Opportunities

Won Revenue

Win Rate

Average Deal Size

Visual Highlights:

Bubble chart reveals correlation between opportunity volume and win rate

Some agents handle high volume but underperform on win rate

Top performers generate disproportionate revenue contribution

📌 Insight: Coaching low win-rate, high-volume agents could significantly improve total revenue.
<img width="1920" height="1080" alt="Screenshot (169)" src="https://github.com/user-attachments/assets/079b25e5-c9ed-4d78-b6f9-a31bc79b240e" />
169

🖼 Image 4 — Product & Pipeline Analysis
🏷 Win Rate by Product

Most products maintain ~60–65% win rate

MG Special and GTX Pro show strongest performance

💰 Won Revenue by Product

Revenue Contribution:

GTX Pro → 35%

GTX Plus Pro → 26%

MG Advanced → 22%

Remaining products contribute smaller shares

📌 Insight: Revenue concentration exists in a few flagship products.

🔄 Pipeline Stage Distribution

Opportunities by stage:

Won → 4K

Lost → 2K

Engaging → 2K

Prospecting → 1K

📌 Insight: Significant drop-off between early and mid-stage pipeline.
<img width="1920" height="1080" alt="Screenshot (171)" src="https://github.com/user-attachments/assets/b4e81e46-2f16-4182-b144-db0210b3038c" />
171

🖼 Image 5 — Trends Dashboard
📊 Revenue & Pipeline Trends (Year-Quarter)

Revenue peaked at 3.09M in Q2

Slight decline across Q3 and Q4

Open pipeline fluctuates with revenue

📈 QoQ Revenue Growth

Q2 Growth: +172%

Q3: -3%

Q4: -6%

📌 Insight:
Revenue growth momentum slowed after Q2 spike — pipeline monitoring is critical.
<img width="1920" height="1080" alt="Screenshot (172)" src="https://github.com/user-attachments/assets/9a983552-7bae-4676-8b7c-390b8408bcac" />
172

🖼 Image 6 — Business Recommendations
🎯 Strategic Recommendations

Focus coaching on low win-rate, high-volume sales agents

Replicate strategies from top-performing teams across regions

Prioritize high win-rate products for cross-sell & upsell initiatives

Monitor pipeline creation trends to anticipate revenue performance

🚀 Business Impact

Implementing these recommendations can lead to:

📈 Increased revenue growth

📉 Improved win rates

🎯 Better sales agent efficiency

💡 Stronger product strategy alignment

🔮 More predictable revenue forecasting
<img width="1920" height="1080" alt="Screenshot (173)" src="https://github.com/user-attachments/assets/e1ab9034-531b-40ca-bd98-df827b8886a0" />
173

🛠 Tools & Technologies

Power BI

DAX (Data Analysis Expressions)

Power Query

Data Modeling

Time Intelligence Functions

📂 Dashboard Structure

Pre-Dashboard (Documentation & Measures)

Executive Overview

Sales Team Performance

Product & Pipeline

Trends

Recommendations

Slicers

🧠 Key Takeaways

Revenue is concentrated among a small number of agents and products

Win rate optimization presents the largest opportunity

Pipeline monitoring is critical for forecasting

Data-driven coaching improves performance efficiency
