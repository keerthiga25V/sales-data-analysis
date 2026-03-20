Sales Performance Analysis — Python & Power BI
Overview
This project analyzes sales transaction data from a global automobile parts company covering 2003 to 2005. The goal was to extract actionable business insights from raw data — from understanding which products drive the most revenue, to identifying which customers are at risk of churning.
The project covers the full data analysis workflow: data cleaning, exploratory analysis, customer segmentation using RFM, and a Power BI dashboard for stakeholder reporting.

Tools & Technologies
ToolPurposePython (Pandas, NumPy)Data cleaning & analysisGoogle ColabDevelopment environmentPower BIDashboard & visualizationGitHubVersion control

Dataset

Source: Sales transaction records
Size: 2,823 rows × 25 columns
Period: 2003 – 2005
Key Fields: Sales, Quantity Ordered, Product Line, Country, Deal Size, Order Status, Customer Name


What I Did
1. Data Cleaning

Removed irrelevant columns (phone numbers, address lines, postal codes)
Handled missing values — filled Territory and State with 'Unknown' where appropriate
Converted Order Date from string to datetime format for time-based analysis

2. Exploratory Data Analysis
Answered key business questions:

Which product line generates the most revenue?
Which countries are the top markets?
What is the monthly and quarterly sales trend?
How are orders distributed by deal size and status?

3. RFM Customer Segmentation
Built an RFM model to score and segment all 92 customers based on:

Recency — How recently did they purchase?
Frequency — How many times did they purchase?
Monetary — How much did they spend in total?

Customers were scored 1–5 on each dimension and grouped into segments: Champions, Loyal Customers, At Risk, Recent Customers, and Potential.

Key Findings

Classic Cars account for ~38% of total revenue ($3.9M out of $10.03M)
USA, Spain, and France together make up 58% of all sales — heavy geographic concentration
November is consistently the highest revenue month across all years — driven by holiday season demand
Q4 generates nearly double the revenue of Q3 ($3.8M vs $1.7M)
Medium deals drive 60% of total revenue — the company's core market
92% of orders are successfully shipped — strong operational performance
RFM analysis revealed 11 loyal customers contributing disproportionately to revenue, and 11 lost customers who haven't purchased recently


Business Recommendations

Prioritize Classic Cars inventory and marketing — highest revenue category by a wide margin
Reduce geographic dependency — USA alone is 35% of revenue, which is a risk
Launch Q3 promotions to counter the mid-year slowdown
Run win-back campaigns targeting the 11 lost customers identified in RFM analysis
Nurture the 60 potential customers — with targeted outreach they can move into the loyal segment


Dashboard
Built in Power BI with the following views:

KPI Cards — Total Revenue, Total Orders, Total Customers
Sales by Product Line
Sales by Country
Monthly Sales Trend
Deal Size Distribution
Order Status Breakdown
RFM Customer Segments



Project Files
├── sales_data.csv          # Original raw dataset
├── sales_clean.csv         # Cleaned dataset used for analysis
├── rfm_analysis.csv        # RFM scores and customer segments
├── sales_analysis.ipynb    # Python notebook with full analysis
├── dashboard_screenshot.png # Power BI dashboard
└── README.md

How to Run

Clone this repository
Open sales_analysis.ipynb in Jupyter or Google Colab
Upload sales_data.csv when prompted
Run all cells in order
For the dashboard, open Power BI and load sales_clean.csv and rfm_analysis.csv


Author
Keerthiga V
Aspiring Data Analyst
