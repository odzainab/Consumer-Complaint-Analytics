## Table of Contents

- [Introduction](#introduction)
- [Business Objectives](#business-objectives)
- [Key Contents of the Dataset](#key-contents-of-the-dataset)
- [Tools Used](#tools-used)
- [Methodology](#methodology)
- [Data Visualization](#data-visualization)
- [Key Insights](#key-insights)
- [Recommendations](#recommendations)
- [Expected Business Impact](#expected-business-impact)
- [Conclusion](#conclusion)

## Introduction

Every year, millions of consumers raise concerns about financial products they rely on for daily life, from credit cards and mortgages to loans and credit reporting services. These complaints offer more than isolated grievances, collectively, they reveal patterns about where financial systems break down, how companies respond under pressure, and which consumer groups may be most affected.

The core problem is not just the number of complaints, but the bank’s inability to clearly identify where issues originate, how efficiently complaints are handled, and whether current response processes are effective.

The focus of this study is not only on when and where complaints occur, but also on how consistently financial institutions respond, and whether response timeliness and outcomes vary by company, product, or submission channel. These insights are intended to support regulators in strengthening consumer protection policies, help journalists highlight systemic fairness issues, and provide consumers with greater transparency into how financial institutions handle complaints.

---

## Business Objectives

✓ Which financial products generate the highest number of complaints?  
✓ What are the most common issues and sub-issues reported by customers?  
✓ How have consumer complaints evolved over time?  
✓ Are there any seasonal spikes or unusual patterns in complaint volumes?  
✓ What percentage of complaints receive a timely response?  
✓ How long does it take on average for the bank to respond to complaints?  
✓ What is the most common resolution?  
✓ How effective is the bank in resolving complaints successfully?  
✓ How does response timeliness impact complaint resolution outcomes?  
✓ Are delayed responses linked to higher dispute rates or unresolved cases?  

---

## Key Contents of the Dataset

The dataset contains consumer complaints related to financial products and services. It includes information on:

- Financial products and sub-products  
- Customer issues and sub-issues  
- Complaint submission channels  
- Submission and response dates  
- Company responses  
- Timely response status  
- State/location details  

The dataset was mainly used to analyze complaint trends, customer pain points, and operational response performance.

---

## Tools Used

- **Microsoft Power BI** – Built interactive dashboards and visualized key insights  
- **Power Query Editor (Power BI)** – Performed data cleaning, transformation, and modeling  
- **Microsoft PowerPoint** – Designed wireframes to plan dashboard structure and user experience before development

---

## Methodology

### Data Cleaning Process (Step-by-Step)

**Step 1: Data Import**  
The dataset was imported from Excel into Power BI using Power Query.

**Step 2: Duplicate Checking**  
The dataset was checked for duplicate records, and none were found.

**Step 3: Data Transformation**  
To improve data clarity and usability, a reference table containing full state names was introduced.

The dataset originally contained abbreviated state codes (e.g., “CA”, “NY”), which can be less intuitive for reporting and visualization.

A Left Outer Join was performed in Power Query to merge the main dataset with the state reference table, using the State column as the key. This allowed the inclusion of a new column containing full state names, enhancing readability and supporting more user-friendly analysis, especially in geographic visualizations.

**Step 4: Column Renaming**  
The column: “Timely response?” → renamed to “Timely response”  

✔ This improves:
- Readability  
- Consistency  
- Professional presentation  

**Step 5: Handling Missing Values**  
Missing values (nulls) in key categorical fields were replaced with: **“N/A”**

Affected columns:
- Sub-issue  
- Company public response  
- Company response to consumer  
- Timely response  

✔ Reasoning:
- Prevents blanks in reports  
- Maintains dataset completeness  
- Avoids loss of records  

**Step 6: Data Validation**  
After cleaning, validation checks were performed to ensure data accuracy and consistency. This included verifying data types, confirming that missing values were properly handled, and ensuring no unintended data loss occurred during transformation.

Key fields such as Complaint ID were also reviewed to confirm the absence of duplicate records.

---

## Data Visualization

### Complaint Overview
<img width="3075" height="1763" alt="Clean_Consumer Complaint_page-0001" src="https://github.com/user-attachments/assets/13b5fdfb-5fa0-4fd4-82c8-879f70e01bc6" />

### Complaint Insights
<img width="3075" height="1763" alt="Clean_Consumer Complaint_page-0002" src="https://github.com/user-attachments/assets/a8f6d594-4eca-4395-8dd3-396f32dba1ba" />

---

## Key Insights

### Complaint Volume & Operational Performance

A total of **62.52K consumer complaints** were recorded across the analyzed period, indicating a consistently high level of customer dissatisfaction across financial products and services.

Despite this volume, the institution demonstrated relatively strong operational responsiveness:

- The **Delayed Response Rate (3.84%)** is low, suggesting that the majority of complaints were handled within expected service levels.
- The **average response time of 1.22 days** indicates efficient front-line complaint handling processes.

However, the volume itself highlights a structural issue — high responsiveness does not necessarily indicate low customer friction, but rather strong handling of recurring operational problems.

### Complaint Trend Analysis

Consumer complaints show a **steady upward trend over time**, particularly accelerating from 2020 onward.

Key observations:
- This upward movement may indicate increasing customer awareness and willingness to report issues, not just worsening service quality.
- A significant spike in **2023** suggests either:
  - Increased operational strain within key financial products, or  
  - Changes in reporting behavior or regulatory awareness

This trend highlights the importance of proactive issue detection rather than reactive complaint handling.

### Product-Level Complaint Analysis

Complaint distribution is heavily concentrated in a few core financial products:

- **Checking/Savings Accounts (24.81K complaints)** represent the largest share of dissatisfaction, indicating foundational banking service issues such as account access, transaction handling, and service reliability.
- **Credit Card/Prepaid Services (16.20K complaints)** reflect recurring issues in billing accuracy, fraud disputes, and payment processing.
- **Mortgage-related complaints** remain consistently high, suggesting ongoing friction in long-term financial commitments such as repayment structures and servicing delays.

This concentration suggests that **core banking products are the primary drivers of customer dissatisfaction**, rather than niche services.

### Seasonal Complaint Patterns

Complaint activity shows clear **seasonal variation**:

- Peak activity occurs around **April**, which may be linked to financial cycles, billing periods, or regulatory reporting timelines.
- A noticeable decline in **November and December** suggests reduced customer activity or resolution backlogs being cleared toward year-end.

These patterns indicate that complaint volume is not random but influenced by **predictable operational cycles**.

### Response Timeliness

The institution demonstrates strong responsiveness overall:

- **58.62K complaints** were resolved within expected timelines.
- Only **2.40K complaints** experienced delays, indicating controlled operational backlog.
- A small portion of records contain **N/A values**, pointing to minor data completeness issues.

While performance is strong, delayed cases may still represent **high-risk complaints**, as delays often correlate with higher customer dissatisfaction.

---

## Complaint Insights

### Complaint Issues & Customer Pain Points

The most frequent customer issue is **Managing an account (15.1K complaints)**, highlighting fundamental friction in everyday banking operations.

Other significant issues include:
- Credit report inaccuracies
- Incorrect billing or statement-related errors

These issues suggest that dissatisfaction is primarily driven by:
- Data accuracy problems  
- Account management inefficiencies  
- Communication gaps between systems and customers  


### Geographic Complaint Distribution

Complaint activity is geographically concentrated in major economic regions:

- **California (13.71K complaints)** leads significantly, followed by Florida and Texas.
- These states represent high population density and high banking activity, naturally contributing to higher complaint volumes.
- Secondary contributors such as New York, Georgia, and New Jersey reinforce the pattern of urban financial pressure points.

This indicates that complaints are strongly linked to **population size and financial activity intensity**, rather than isolated regional issues.

### Complaint Resolution Analysis

The most common resolution outcome is **“Closed with explanation” (27.04K complaints)**.

This suggests that:
- Most complaints are resolved through clarification rather than compensation.
- Monetary relief is relatively rare, indicating limited financial remediation.
- A small number of cases remain unresolved or in progress, highlighting edge-case inefficiencies.

Overall, resolution patterns show a **communication-heavy resolution strategy rather than financial compensation-based resolution**.

## Response Timeliness & Operational Risk

Certain financial products show elevated operational risk in terms of delayed responses**:

- **Debt Collection (6.32% delayed rate)**
- **Credit Reporting Services (6.16% delayed rate)**

These categories are typically more complex and involve third-party dependencies, which may explain slower response times.

In contrast:
- **Mortgage complaints (0.24% delayed rate)** show strong operational control and structured handling processes.

This indicates that operational efficiency varies significantly by product complexity.

## Response Timeliness & Resolution Outcomes
A clear relationship emerges between response speed and resolution quality**:

- Most **timely responses result in “Closed with explanation” outcomes**, reinforcing the importance of fast handling in reducing escalation.
- Delayed responses are less frequent but tend to be associated with more complex or unresolved cases.

This suggests that **response timeliness is a strong operational lever influencing customer satisfaction and complaint closure behavior**.

---  

## General Insights

The analysis revealed that complaints are mainly concentrated around account management, credit reporting, and payment-related issues.

Although overall response performance is strong, certain product categories such as debt collection and credit reporting show operational inefficiencies.

Geographic patterns indicate higher complaint volumes in densely populated states such as California, Florida, and Texas.

---

## Recommendations

### 1. Customer Service / Support Teams  
**Focus: Complaint handling efficiency & response time**

- Reduce delayed response cases in high-risk product categories such as Debt Collection and Credit Reporting Services  
- Improve first-contact resolution to minimize repeat complaints and customer follow-ups  
- Standardize response templates for frequent issues such as account management and billing inquiries  
- Strengthen training programs to improve consistency and speed of complaint handling  

### 2. Operations / Process Teams  
**Focus: Process improvement & workflow efficiency**

- Conduct root cause analysis on delays observed in specific product lines  
- Optimize complaint routing and escalation workflows to ensure faster resolution  
- Improve tracking systems for monitoring the full complaint lifecycle from submission to closure  
- Identify bottlenecks in internal approval or investigation processes  


### 3. Product Teams (Banking & Financial Products)  
**Focus: Product-related complaint reduction**

- Review products generating the highest complaint volumes (e.g., Checking/Savings Accounts, Credit Cards)  
- Address recurring usability and service design issues contributing to customer dissatisfaction  
- Improve transparency in fees, transaction processes, and account operations  
- Collaborate with support teams to identify product pain points from complaint data  


### 4. Regional / Branch Management  
**Focus: Geographic complaint concentration**

- Focus on high-complaint regions such as California, Florida, and Texas  
- Identify regional service gaps or inconsistencies in customer experience delivery  
- Strengthen local customer support coverage and operational capacity  
- Monitor regional trends to detect early warning signs of service deterioration  

### 5. Senior Management / Strategy Team  
**Focus: Overall performance & customer experience strategy**

- Monitor complaint trends as a key Customer Experience (CX) performance indicator  
- Invest in automation tools to reduce response time and backlog accumulation  
- Use complaint insights to guide long-term operational improvements and risk management strategies  
- Align complaint analytics with enterprise-wide customer satisfaction goals  


## Expected Business Impact

- Improved customer satisfaction through faster and more consistent complaint resolution across all financial products.  

- Reduction in delayed response rates, particularly within high-risk product categories such as Debt Collection and Credit Reporting Services.  

- Better operational efficiency achieved through targeted process improvements in complaint handling workflows and escalation paths.  

- Enhanced decision-making supported by data-driven insights into customer pain points, product-level issues, and regional complaint trends.  

## Conclusion

The Consumer Complaint Analytics dashboard transformed raw data into actionable insights that support better operational monitoring and customer experience improvement.

While the bank demonstrates strong response performance overall, targeted improvements are needed in specific product areas to reduce delays and enhance customer satisfaction.
