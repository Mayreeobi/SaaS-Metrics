# SaaS Business Health Analysis

> **Multi-dimensional business health analysis using Tableau**.
> Tracking revenue growth, customer acquisition efficiency, retention, and plan tier unit economics across a 27-month SaaS dataset.

[View Live Dashboard](https://public.tableau.com/app/profile/chinyere.obi8867/viz/SaaSMetricsViz/ExecutiveOverview) | [Dashboard snippet](https://github.com/Mayreeobi/SaaS-Metrics/blob/main/Executive%20Overview.png)


---

## Table of Contents

- [Situation](#situation)
- [Task](#task)
- [Action](#action)
- [Result](#result)
- [Insights & Recommendations](#insights--recommendations)
- [Tools & Stack](#tools--stack)

---

## Situation

A fast-growing SaaS company had no unified view of its business health. Revenue data lived in one source, customer data in another, and tier breakdowns came in quarterly while overall metrics were monthly - making it nearly impossible to answer the questions that actually drive decisions.

**The core business questions that had no clear answers:**

| Area | Question |
|------|----------|
| Revenue | Is MRR growth coming from new customers, expansion, or are we just retaining well? |
| Acquisition | Is our sales and marketing spend actually paying off - and getting more efficient? |
| Retention | Which customer segments churn, and how bad is it really? |
| Segmentation | Which plan tier has the best unit economics - where should we invest? |
| Planning | Where should the next S&M budget dollar go? |

---

## Task

Build a **4-tab Tableau dashboard** that gives stakeholders a single source of truth; covering revenue trajectory, acquisition efficiency, retention trends, and tier-level unit economics. Every view needed to be actionable, not just informational.

### Dashboard Structure

| Tab | Purpose |
|-----|---------|
| **Executive Overview** | KPI snapshot: MRR, ARR, customers, MRR growth trend, net new MRR waterfall, churn rate, LTV:CAC, CAC payback |
| **Customer Acquisition** | New customers by month, CAC trend, trial funnel (started → converted), Magic Number chart, growth rate % |
| **Revenue & Retention** | MRR composition (new vs. expansion vs. churned), churn rate trend, ARPU over time, customer lifetime value |
| **Plan Tier Analysis** | Distribution, revenue share, churn, ARPU, and LTV:CAC by tier (Starter / Pro / Enterprise) |

### Calculated Fields

```
// Net New MRR
[New MRR] + [Expansion MRR] - [Churned MRR]

// ARR
[Total MRR] * 12

// Churn Rate %
([Churned Customers] / [Total Customers]) * 100

// ARPU
[Total MRR] / [Total Customers]

// Trial Conversion Rate %
([Trials Converted] / [Trials Started]) * 100

// Customer Lifetime (months)
1 / ([Churn Rate %] / 100)

// LTV
[ARPU] * [Customer Lifetime]

// LTV:CAC Ratio
[LTV] / [CAC]

// CAC Payback Period (months)
[CAC] / [ARPU]

// Magic Number (Sales Efficiency)
[Net New MRR] / [Sales & Marketing Spend]

```

---

## Action

### Data Architecture

The first challenge was structural: two datasets at different granularities had to be unified before a single dashboard could work across all tabs.

- Standardized the monthly metrics dataset (27 months: Jan 2023 - Mar 2025) and the quarterly tier breakdown to a shared time dimension
- Mapped MRR components: new, expansion, churned - to enable waterfall decomposition in Tableau
- Created all 11 derived metrics as Tableau calculated fields to keep source data clean
- Built tier-level aggregations for Starter, Pro, and Enterprise to enable side-by-side unit economics comparison


---

## Result

### Top-Line Growth (27 Months)

| Metric | Start (Jan 2023) | End (Mar 2025) | Change |
|--------|-----------------|----------------|--------|
| MRR | $42.6K | $593.9K | +1,294% (14×) |
| ARR | $511K | $7.1M | +1,293% |
| Customers | 118 | 1,224 | +10× |
| New customers/month | 18 | 98 | +5.4× |
| Net New MRR/month | $7.6K | $35.1K | +4.6× |

### Unit Economics

| Metric | Start | Current | Benchmark | Status |
|--------|-------|---------|-----------|--------|
| LTV:CAC Ratio | 24× | **48×** | 3 - 5× | ✅ Exceptional |
| Monthly Churn | 1.67% | **2.12%** | 2 - 5% | ✅ Good |
| CAC | $420 | **$344** |  -   | ✅ Improving |
| CAC Payback |   -   | **8 - 10 mo** | 12 - 18 mo | ✅ Excellent |
| Magic Number |  -   | **1.0 - 1.2** | >0.75 | ✅ Excellent |
| Trial Conversion |  -   | **31 - 32%** | 20 - 30% | ✅ Good |
| ARPU | $360 | **$485** |  -   | ✅ +35% |

### Plan Tier Breakdown (Mar 2025)

| Metric | Starter | Pro | Enterprise |
|--------|---------|-----|------------|
| Customers | 598 (49%) | 510 (42%) | 116 (9%) |
| MRR | $119.6K (17%) | $306K (42%) | $295K (41%) |
| ARPU | $200/mo | $600/mo | $2,543/mo |
| Monthly Churn | 2.01% | 0.59% | 0% |

> **Key finding:** Enterprise is 9% of customers but 41% of revenue with zero churn. Pro has the best risk-adjusted unit economics. Starter is the high-volume acquisition funnel that feeds upgrades; it's doing its job.

---

## Insights & Recommendations

**Business Health Score: 9/10** - Beating benchmarks across the board.

<details>
<summary><strong>Insight 1: The Expansion Inflection Point</strong></summary>

Around month 18–20 (mid-2024), expansion MRR began consistently exceeding new MRR. This is the classic land-and-expand signal; existing customers are growing their spend faster than the business is acquiring new ones. Expansion revenue has near-zero CAC, so when it outpaces new acquisition you get compounding growth without proportional cost increase.

**The land-and-expand motion is working organically. It just needs to be formalized.**

</details>

<details>
<summary><strong>Insight 2: CAC Is Falling While Volume Is Rising</strong></summary>

CAC dropped from $420 to $344 while new customers per month grew from 18 to 98. This combination: lower cost, higher volume, means repeatable acquisition channels have been found. The Magic Number of 1.0–1.2 is the clearest signal that more S&M spend will generate positive returns.

**This is a green light to invest more in acquisition. You've found PMF.**

</details>

<details>
<summary><strong>Insight 3: Enterprise Is the Hidden Engine</strong></summary>

Enterprise grew from 6 to 116 customers, generates 41% of revenue from 9% of the base, and has zero churn. It is currently underfunded relative to its economic contribution — it's sharing sales and success resources with tiers that generate a fraction of the value.

**This tier deserves a dedicated motion, not shared resources.**

</details>

<details>
<summary><strong>Insight 4: Pro Is the Underappreciated Sweet Spot</strong></summary>

Pro has the best risk-adjusted unit economics: $600 ARPU, sub-1% monthly churn, and strong growth. Every Starter-to-Pro conversion is worth roughly $4,800/year in incremental ARR at zero additional acquisition cost.

**Pro is where the business compounds. Invest in the upgrade path.**

</details>

<details>
<summary><strong>Insight 5: Churn Has Stabilized, But Not Improved</strong></summary>

After peaking at 2.68% in mid-2023 (normal while the business was still finding product-market fit), churn settled at 2.12%. That's acceptable for SMB SaaS, but it hasn't moved in 6 months. At current scale, each 0.1% reduction in monthly churn is worth roughly $60K in retained ARR annually.

**The floor has been found. Now it needs to be lowered.**

</details>

---

### Recommendations

#### Immediate (Next 30 Days)

**1. Accelerate Enterprise Sales**
- Hire 2 – 3 dedicated Enterprise AEs
- Build white-glove onboarding to reinforce stickiness at this tier
- Commission case studies from existing Enterprise accounts
- 📈 *Expected impact: +20 - 30 Enterprise customers over 12 months = +$600K–$900K ARR*

**2. Optimize Trial-to-Paid Conversion**
- A/B test trial length: 7-day vs. 14-day vs. 30-day
- Implement sales-assisted trials for high-intent signups (identified via usage signals)
- Add in-app activation milestones that guide users to the "aha moment" faster
- 📈 *Expected impact: 31% → 35% = ~20 extra customers/month = +$120K ARR*

**3. Formalize the Starter → Pro Upgrade Path**
- Build usage-based triggers: when a Starter account hits defined limits, surface a Pro upgrade prompt
- Run a targeted upgrade campaign to Starter customers who have been active for 90+ days
- Build a feature comparison tool showing exactly what Pro unlocks
- 📈 *Expected impact: convert 10% of Starter base to Pro = +$240K ARR at zero acquisition cost*

#### Short-Term (3 - 6 Months)

**4. Invest in Customer Success for Expansion Revenue**
- Hire 2–3 CSMs focused on expansion, not just retention
- Implement a systematic QBR process for all Pro and Enterprise accounts
- Build expansion playbooks: when to upsell, upgrade, and cross-sell
- 📈 *Expected impact: Expansion MRR from $8.4K → $15K/month = +$80K ARR*

**5. Double Down on Acquisition Channels That Work**
- Analyze channel-level CAC to identify the performers
- Allocate 60–70% of budget to proven channels; keep 30–40% for testing
- Increase total S&M spend 30–50%; the 48× LTV:CAC makes this strongly ROI-positive
- 📈 *Expected impact: add 50–75 more customers/month while maintaining or improving CAC*

**6. Target Starter Churn Specifically**
- Run exit surveys to identify the top churn reasons for Starter accounts
- Improve self-serve onboarding, Starter users likely have the least support access
- Evaluate whether Starter pricing is attracting low-intent customers
- 📈 *Expected impact: Starter churn 2.01% → 1.5% = retain 36 more customers/year*

#### Long-Term (6 - 12 Months)

- **Partner/reseller program**: expand reach without proportionally increasing CAC (target: 15–25% of new customers via partners within 12 months)
- **Formalize land-and-expand** with seats-based pricing and collaboration features that encourage viral growth within accounts
- **International expansion** starting with English-speaking markets (UK, Australia, Canada) - the fundamentals are strong enough to support geographic scaling

---

### Risks to Monitor

| Risk | Signal to Watch | Mitigation |
|------|----------------|------------|
| Churn plateau | Churn ticks back up as scale increases | Invest in CS team; track usage drops and support ticket volume as leading indicators |
| Enterprise concentration | Over-dependence on a handful of large accounts | Diversify Enterprise base; assign dedicated CSMs; implement health scores |
| Market saturation | CAC rising, conversion falling, longer sales cycles | Expand TAM via new verticals or geographies before this happens |
| Competitive pressure | Unexplained conversion drops or churn spikes | Build moats through integrations and network effects; double down on CS |

---

### Financial Projections (If Recommendations Executed)

| Metric | Current (Mar 2025) | 12-Month Projection |
|--------|--------------------|---------------------|
| MRR | $594K | $950K - $1.1M |
| ARR | $7.1M | $11.4M - $13.2M |
| Customers | 1,224 | 2,000 - 2,200 |
| Churn Rate | 2.12% | 1.8% - 1.9% |
| LTV:CAC | 66.5× | 55× - 60× |
| Enterprise % | 9% | 12% - 15% |

> Conservative scenario: **60% YoY growth to $11.4M ARR**  
> Aggressive scenario: **85% YoY growth to $13.2M ARR**  
> Both are achievable given current trajectory and unit economics.

---

## Tools & Stack

| Layer | Tool |
|-------|------|
| Visualization | Tableau |
| Data Preparation | Excel / CSV |
| Calculated Metrics | Tableau Calculated Fields |


---

*Chinyere Obi · Data Analyst · [Portfolio](https://chinyereobi.netlify.app) · [LinkedIn](https://www.linkedin.com/in/chinyere-obi/) · [Tableau](https://public.tableau.com/app/profile/chinyere.obi8867/vizzes)*




