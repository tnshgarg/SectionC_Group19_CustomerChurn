# Credit Card Customer Retention Analytics

## Project Overview

This project presents a data-driven analysis of a bank’s credit card subscription outreach campaign. Using 30,488 customer records, we analyzed demographic and operational variables to identify high-conversion segments and optimize marketing efficiency.

The objective is to reduce wasted outreach efforts and improve overall campaign ROI through targeted segmentation and engagement optimization.

---

## Problem Statement

The bank faces high operational expenditure (OpEx) due to broad-based calling campaigns with a low baseline conversion rate of 12.66%.

Objective:  
Leverage demographic profiling and campaign metrics to identify high-propensity customer segments and optimize contact strategies.

---

## Dataset Summary

- Total Records: 30,488  
- Total Subscribed: 3,859  
- Conversion Rate: 12.66%  
- Average Call Duration: 259 seconds  
- Total Variables: 16  

### Key Variables

Demographics:
- age  
- job  
- education  
- marital  

Financial Indicators:
- default  
- housing  
- loan  

Campaign Metrics:
- duration  
- campaign  
- pdays  
- previous  

Target Variable:
- y (Subscribed: Yes/No)

Source: Kaggle – Credit Card Customer Churn/Retention Dataset

---

## Key Findings

### 1. Engagement Duration Impact

- Subscribed Average Duration: ~550 seconds  
- Not Subscribed Average Duration: ~220 seconds  
- Inflection Threshold: ~300 seconds (5 minutes)

Longer call engagement strongly correlates with higher subscription probability.

---

### 2. High-Converting Segments

Top Job Categories (by conversion volume):
- Admin  
- Blue-Collar  
- Technician  

Education Distribution of Subscribers:
- University Degree: 40%  
- High School: 24.2%  
- Professional Course: 13.9%  

University graduates are nearly twice as likely to subscribe compared to high school graduates.

---

### 3. Channel Performance

Cellular outreach significantly outperforms traditional telephone (landline) communication.

---

### 4. Temporal Trends

- Highest contact volume: May  
- Highest proportional conversion efficiency: October and December  

Year-end campaigns show stronger efficiency relative to outreach volume.

---

## KPI Framework

| KPI | Value | Purpose |
|------|--------|------------|
| Total Contacts | 30,488 | Campaign reach |
| Total Subscribed | 3,859 | Revenue outcome |
| Conversion Rate | 12.66% | ROI metric |
| Avg Call Duration | 259s | Engagement baseline |

---

## Strategic Recommendations

1. Transition fully to cellular outreach.
2. Encourage agents to sustain conversations beyond 5 minutes for high-potential leads.
3. Reallocate part of Q2 marketing budget toward Q4 (October–December).
4. Prioritize university degree holders and top-performing job segments.
5. Implement a three-contact cap to reduce customer fatigue and inefficiency.

---

## Data Cleaning & Preparation

- Standardized categorical values using ARRAYFORMULA(PROPER(...)).
- Preserved "Unknown" as a valid category to avoid skew.
- Engineered binary target flag for conversion calculation.
- Treated duration = 0 as no contact established.
- Interpreted pdays = 999 as not previously contacted.

Tools Used:
- Google Sheets
- Pivot Tables
- COUNTIFS / AVERAGEIFS
- Dashboard slicers and charts

---

## Impact Estimation

- Reduction of ~8,000 low-propensity calls
- Potential conversion improvement from 12.66% to 15%
- Estimated 700+ additional subscriptions
- Reduced customer fatigue from excessive follow-ups

---

## Future Scope

- Logistic Regression–based propensity scoring
- CRM integration for real-time monitoring
- Automated lead scoring framework

---

## Team Contributions

| Team Member | Role |
|--------------|--------|
| Tanish Garg | Presentation Lead |
| Harshil | Data Cleaning Lead |
| Sachin Jaiswal | KPI Developer |
| Omved Nagre | Dashboard Developer |
| Nishtha Gupta | KPI Developer |
| Abhay | Data Sourcing |
| Ashish Kushwaha | Report Writer |

---

## Conclusion

This analysis transforms 30,488 raw customer records into a structured, data-driven marketing strategy. By identifying engagement thresholds, high-performing demographic segments, and optimal campaign timing, the bank can shift from volume-based outreach to targeted, value-driven marketing to improve ROI and operational efficiency.
