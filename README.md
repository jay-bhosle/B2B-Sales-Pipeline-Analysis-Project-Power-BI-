# B2B Sales Pipeline – Power BI Analytics  
**Evaluating sales performance, pipeline health, and conversion trends for a hardware company**

## Project Overview
This project transforms a raw B2B sales pipeline into an interactive Power BI dashboard. The goal is to assess sales team performance, spot bottlenecks, track quarter‑over‑quarter trends, and deliver data‑driven recommendations to boost revenue.

## Tools & Technologies
- **Power BI** – Data modelling, DAX measures, interactive dashboards  
- **Power Query** – Data cleaning and transformation  
- **Excel/CSV** – Source data

## Data Quality & Preparation
Before analysis, I resolved several data issues:
- Removed duplicate dimension records  
- Handled missing values for region, industry, and sales agent  
- Standardised sales stage and region naming  
- Excluded invalid opportunities (null or zero value)  
- Fixed date inconsistencies between creation and close dates

## DAX Measures & Model
I built a comprehensive measure library to power all visuals, including:
- **Core KPIs:** Total Opportunities, Won/Lost Revenue, Win Rate, Average Deal Size  
- **Time Intelligence:** Won Revenue QoQ, QoQ Revenue Growth %, Pipeline Created Value  
- **Product Analysis:** Product Win Rate, Revenue Share %  

<img width="1920" height="1080" alt="1" src="https://github.com/user-attachments/assets/c6a99817-8691-4a3f-a706-f8c9afee5466" />

## Dashboard Pages & Key Insights

### 1. Executive Overview
High‑level view of won revenue by quarter and top‑performing sales agents.  
<img width="1920" height="1080" alt="2" src="https://github.com/user-attachments/assets/282afbad-534b-486e-967d-e477e0e5895f" />

### 2. Sales Team Performance
Detailed table ranking every sales agent by opportunities, win rate, and average deal size. Pinpoints under‑performers and stars.  
<img width="1920" height="1080" alt="3" src="https://github.com/user-attachments/assets/891bb44a-fd28-4cf0-8556-b5a27aa4548a" />

### 3. Product & Pipeline
- **GTX Pro** and **GTX Plus Pro** dominate, together accounting for over **48% of won revenue**.  
- The “Engaging” stage holds the most open opportunities, a key pipeline driver.  
<img width="1920" height="1080" alt="4" src="https://github.com/user-attachments/assets/eca0f909-e090-49ee-b910-e3785e0a3a23" />

### 4. Trends
Quarter‑over‑quarter analysis shows clear seasonality and growth patterns:
- Won revenue peaked in **2017‑Q2**; pipelines built in earlier quarters fed this success.  
- QoQ revenue growth spiked at nearly **5%** in one quarter, showing targeted uplift.  
<img width="1920" height="1080" alt="5" src="https://github.com/user-attachments/assets/a764c528-b8e0-44e0-890f-c04bc9725a07" />

## Key Takeaways
- **Overall Win Rate:** 63% – a strong baseline across all agents.  
- **Top Performers:** Agents like *Elease Gluck* (63% win rate, high deal size) and *James Ascencio* (66% win rate) set the benchmark.  
- **Coaching Opportunity:** Several agents have high volume but win rates below 60%; focused coaching can lift revenue quickly.  
- **Product Strategy:** GTX Pro family is the star; cross‑sell and upsell motions around these products will yield the highest returns.  
- **Pipeline Health:** Open pipeline value remains robust, ensuring future quarters are well supplied.

## Recommendations
<img width="1920" height="1080" alt="6" src="https://github.com/user-attachments/assets/1d80c4d8-26d5-41df-b53a-d14272f73337" />

1. **Coach low‑win‑rate, high‑volume agents** – Small improvements here deliver oversized revenue impact.  
2. **Replicate top‑performer strategies** – Document and share the practices of agents with the highest win rates and deal sizes.  
3. **Prioritise high‑win‑rate products** – Embed GTX Pro and GTX Plus Pro in all cross‑sell and upsell motions.  
4. **Monitor pipeline creation trends** – Ensure enough opportunities are being generated to sustain future growth; use the Trends page as an early‑warning system.

---

*The Power BI file contains 7 pages (including slicers). All supporting screenshots are in the `images/` folder.*
