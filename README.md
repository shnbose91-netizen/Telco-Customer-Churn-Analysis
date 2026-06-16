# Telco-Customer-Churn-Analysis
Telco customer churn decoded — 27% churn rate, 6 root causes, 6 retention strategies. Built in Power BI.
# 📊 Telco Customer Churn Analysis — Power BI Dashboard

> **"Customers don't leave without warning. The data always knows before we do."**

![Power BI](https://img.shields.io/badge/Tool-Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Dataset](https://img.shields.io/badge/Dataset-Kaggle%20Telco%20Churn-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

---

## 📌 Table of Contents

- [Project Overview](#-project-overview)
- [Business Problem](#-business-problem)
- [Dashboard Highlights](#-dashboard-highlights)
- [Key Findings & Root Cause Analysis](#-key-findings--root-cause-analysis)
- [Recommendations](#-strategic-recommendations)
- [Dataset](#-dataset)
- [Tools Used](#-tools-used)
- [How to Use](#-how-to-use)
- [Key Takeaway](#-key-takeaway)

---

## 🧭 Project Overview

This project is an end-to-end **Customer Churn Analysis** built for a telecommunications company using **Microsoft Power BI** on the publicly available **Kaggle Telco Customer Churn dataset**.

Churn analysis is one of the most critical exercises any subscription-based business can undertake. The goal here was not simply to count how many customers left — it was to understand **who left, why they left, and what structural patterns made them vulnerable** long before they made the decision to cancel.

The dashboard translates raw customer data across 7,043 records and 21 features into a strategic retention framework — one that a business can act on immediately, not just admire visually.

---

## 🔴 Business Problem

Telecommunications is a fiercely competitive, commoditized market. Customers have more choices than ever, switching costs are low, and brand loyalty is eroding. In this environment, **retaining existing customers is significantly more cost-effective than acquiring new ones** — industry research consistently shows that acquiring a new customer costs 5 to 7 times more than keeping one.

This dataset reveals a business under quiet but serious revenue pressure:

| Metric | Value |
|---|---|
| Total Customers | 7,043 |
| Churned Customers | 1,869 |
| **Overall Churn Rate** | **27%** |
| Monthly Revenue at Risk | $139,130 |
| Total Revenue | $16.06M |

A **27% churn rate** is not a rounding error — it is a structural problem. Nearly one in three customers is walking out the door. At $139K in monthly revenue at risk, unchecked churn compounds into a multi-million dollar annual loss when factoring in the cost of replacement acquisition.

The business questions driving this analysis were:

1. Which customer segments are churning at the highest rates?
2. What behavioural, contractual, and service-level patterns are predictive of churn?
3. Where should the business focus its retention investment for the highest return?

---

## 📊 Dashboard Highlights

The Power BI dashboard is organized into six analytical panels, each targeting a distinct churn dimension:

| Panel | What It Answers |
|---|---|
| **KPI Banner** | Snapshot of churned customers, churn rate, total customers, revenue at risk, and total revenue |
| **Churn Rate by Monthly Charges** | Whether spend level correlates with churn risk |
| **Churn Rate by Payment Method** | Whether how customers pay predicts whether they stay |
| **Churn Distribution by Tenure & Contract Type** | How long customers have been with the company and what type of contract they hold affects their probability of leaving |
| **Churn Rate by Internet Service** | Whether the type of internet service is linked to dissatisfaction |
| **Churn Rate by Addon Services Adoption** | Whether customers who use value-added services are more loyal |
| **Key Insights Table** | A ranked summary of the top churn drivers with their respective churn rates |

---

## 🔍 Key Findings & Root Cause Analysis

The analysis makes clear that churn is **not random**. It clusters predictably and powerfully around a small set of behavioural and contractual signals. Below is a detailed breakdown of every major finding.

---

### 1. 🗓️ Contract Type — The Strongest Predictor of Churn

**New customers with month-to-month contract churn at 51%.** One-year contract customers churn at dramatically lower rates, and two-year contract customers show near-zero churn.

This finding points to a fundamental absence of switching cost and long-term commitment. When a customer is on a rolling monthly plan, every billing cycle is a renewal decision — and every renewal decision is an opportunity to leave. These customers have made no financial commitment to the relationship, so departing carries no penalty. The contrast with annual contract holders is stark and statistically unambiguous.

> **The implication:** Contract structure is the single most powerful lever in the entire retention toolkit. Locking a customer into a longer-term plan dramatically reduces churn exposure — not because it traps them, but because it signals mutual investment in the relationship.

---

### 2. 💳 Payment Method — A Proxy for Engagement Level

**Electronic check users churn at 45%** — nearly three times the rate of credit card (15%) or bank transfer (17%) users.

This is not simply about payment logistics. Customers who pay manually each month tend to be less embedded in the service ecosystem. Auto-pay enrollment, by contrast, correlates with a more passive, habitual relationship with the service — one that does not require the customer to actively reconsider their subscription each month. Manual payers think about the bill. Auto-payers don't.

> **The implication:** Payment method is a leading indicator of engagement depth. Migrating customers to auto-pay is a low-cost, high-return intervention that reduces both churn risk and late payment friction simultaneously.

---

### 3. 🌐 Fiber Optic — The Premium Paradox

**Fiber optic customers churn at 42%**, compared to just 19% for DSL users and 7% for those with no internet service.

This is one of the most counterintuitive findings in the dataset. Premium customers paying for the highest-tier service are leaving at the highest rate. This is not a satisfaction story — it is an **expectations mismatch story**. Fiber optic customers are paying more, which means their expectations for service quality, reliability, and value for money are proportionally higher. When those expectations go unmet — whether through service interruptions, pricing that feels unjustified, or a lack of differentiated support — they leave, and they leave quickly.

> **The implication:** High-value customers require high-touch retention strategies. The business cannot afford to assume that premium customers are satisfied simply because they are paying more.

---

### 4. 🔒 Absence of Add-On Services — Reducing Perceived Value

Customers without **Online Security** and without **Tech Support** both churn at **42%**. Across all add-on service categories — Device Protection, Online Backup, Online Security, Streaming Movies, Streaming TV, and Tech Support — the pattern is consistent: customers without these services churn at significantly higher rates than those who have adopted them.

Add-on services function as **stickiness mechanisms**. They deepen the customer's functional reliance on the provider, increase the perceived cost of switching, and raise the total value the customer extracts from the relationship. A customer using only a bare-bones plan is a customer who can leave and immediately replicate their service elsewhere. A customer using online security, backup, and tech support has woven the provider into their digital life.

> **The implication:** Add-on adoption is not a revenue upsell — it is a retention investment. Getting customers to adopt even one additional service meaningfully reduces their churn probability.

---

### 5. 🆕 New Customers — The Most Vulnerable Window

The **New Connection (tenure less than 15 months) and Developing tenure cohort (tenure is between 15 to 24 months)** (newest customers) shows a **51% and 36% churn rate respectievely on month-to-month contracts**, with the rate declining to 33% for Established customers(tenure is between 24 to 50 months) and 25% for Loyal customers(tenure more than 50 months) on the same contract type.

The pattern is clear: **the earlier in the customer lifecycle, the higher the churn risk.** This reflects a universal truth in subscription businesses — the first 90 days are the highest-risk window. New customers have not yet experienced enough value to feel committed. If the onboarding experience fails to demonstrate clear, immediate utility, the customer has no anchor keeping them in the relationship.

> **The implication:** Onboarding is not a support function — it is a retention function. The business needs a structured, proactive engagement program for customers in their first three months.

---

### 6. 💰 Spend Level — Middle Segment Overlooked

Churn by monthly charges shows **medium spenders churning at 33%** and **high spenders at 28%**, with low spenders at 16%.

The medium spend segment is particularly concerning because it is often deprioritised in retention strategy — these customers are not generating top-tier revenue, so they do not receive the white-glove treatment that high-value customers get. Yet they are churning at nearly the same rate, and they represent a large proportion of the customer base.

> **The implication:** Retention strategy must not be exclusively top-down. A tiered retention approach that includes medium-spend customers will recover more total revenue than one that focuses only on the highest spenders.

---

## ✅ Strategic Recommendations

Based on the findings above, the following six recommendations are prioritized by expected impact and implementation feasibility.

---

### 🔴 Priority 1 — Drive Contract Upgrades Aggressively

**Target:** Month-to-month customers (51% churn rate)

Launch a **Contract Loyalty Program** that incentivises month-to-month customers to upgrade to annual or two-year plans. Offer tangible, immediate value in exchange for commitment — a locked-in monthly rate, one or two months free, or bonus add-on services bundled into the upgraded plan. The goal is to make the annual plan feel like the obviously smarter financial choice, not a constraint.

Even converting 20% of the month-to-month base to annual contracts would represent a significant reduction in overall churn exposure, given that this segment carries the single highest churn rate in the dataset.

---

### 🔴 Priority 2 — Redesign the New Customer Onboarding Experience

**Target:** New Connection & Developing tenure segment (51% & 36% churn, month-to-month)

Build a structured **90-Day Customer Success Program** specifically for new customers. This should include:

- A proactive welcome call or digital onboarding sequence within the first 48 hours
- Guided product education over the first 30 days
- A mid-point check-in at Day 45 to surface and resolve dissatisfaction before it becomes a decision to leave
- A loyalty milestone at Day 90 that rewards the customer for staying and anchors the relationship

The first three months determine whether a customer becomes a long-term asset or a churn statistic. Right now, the business is leaving that window unmanaged.

---

### 🟠 Priority 3 — Incentivise Auto-Pay Enrollment at Signup

**Target:** Electronic check users (45% churn rate)

Make auto-payment enrollment **the default and the obvious choice** from the moment a customer signs up. Offer a meaningful monthly bill discount — even $5 to $10 per month — for customers who enroll in automatic credit card or bank transfer payment. Frame it as a customer benefit, not an administrative preference.

This intervention simultaneously reduces churn risk, improves payment reliability, and decreases the cognitive friction that causes manual payers to actively reconsider their subscription each billing cycle.

---

### 🟠 Priority 4 — Bundle Add-On Services Into Onboarding Packages

**Target:** Customers without Online Security, Tech Support, or other add-ons (42% churn)

Instead of pitching add-on services as upsells after the fact, **embed trial periods into the initial customer offer**. A free 3-month trial of Online Security and Tech Support costs the business very little in marginal terms but dramatically increases the probability that the customer will adopt and retain these services past the trial period.

The data is unambiguous: customers who use add-on services churn at significantly lower rates. The business's job is to get them there.

---

### 🟡 Priority 5 — Investigate and Address the Fiber Optic Value Gap

**Target:** Fiber optic customers (42% churn)

The premium paradox revealed by fiber optic churn rates demands direct investigation. Initiate a dedicated **Voice of Customer program** for fiber optic subscribers that captures:

- Net Promoter Score (NPS) trends over customer lifetime
- Exit survey data from churned fiber optic customers
- Service quality and reliability complaint patterns
- Price sensitivity benchmarking against competing fiber providers

Until the root cause of fiber optic dissatisfaction is isolated, implement interim retention measures: proactive SLA guarantees, dedicated premium support lines, and loyalty pricing for long-tenure fiber customers.

---

### 🟡 Priority 6 — Build a Predictive Churn Scoring Model

**Target:** Entire active customer base

This dashboard is retrospective — it tells us who already left. The strategic evolution is **predictive**. Using the patterns identified in this analysis, build a machine learning model (logistic regression as a baseline, gradient boosting for optimised performance) that assigns each active customer a real-time churn risk score.

Input features should include contract type, payment method, tenure, internet service type, add-on adoption, and monthly charges. The output is a ranked list of at-risk customers that the retention team can work through proactively — reaching out before a customer makes the decision to leave, not after.

---

## 📁 Dataset

- **Source:** [Kaggle — Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- **Records:** 7,043 customers
- **Features:** 21 columns including contract type, payment method, internet service, monthly charges, tenure, add-on services, and churn label
- **Target Variable:** `Churn` (Yes / No)

---

## 🛠️ Tools Used

| Tool | Purpose |
|---|---|
| **Microsoft Power BI** | Dashboard development and data visualisation |
| **Power Query** | Data cleaning and transformation |
| **DAX** | Calculated measures and KPIs |
| **Kaggle** | Dataset source |

---

## 🚀 How to Use

1. Download or clone this repository
2. Open the `.pbix` file in **Microsoft Power BI Desktop**
3. The dataset is embedded — no additional setup required
4. Use the slicers and filters within the dashboard to explore churn patterns by segment, contract type, and service category

> **Note:** Power BI Desktop is free to download from [Microsoft's official site](https://powerbi.microsoft.com/desktop/).

---

## 💡 Key Takeaway

> *Churn in this business is not a product problem — it is a relationship problem. Customers leave when they feel under-committed, under-supported, and under-valued. The data tells us exactly where those gaps are. Addressing them is no longer a guessing game — it is an execution challenge.*

The six recommendations above, if implemented systematically, have the potential to reduce overall churn from 27% to well below 20% within 12 months — recovering a significant portion of the $139K in monthly revenue currently at risk, and compounding that recovery across the full customer lifetime.

---

## 🤝 Connect

If you found this project useful or have feedback, feel free to connect:

- 💼 [LinkedIn](#) *https://www.linkedin.com/in/sohini-bose-6a1599a2/*
- 📧 [Email](#) *shnbose91@gmail.com*

---

*⭐ If this project helped you, consider giving it a star on GitHub!*
