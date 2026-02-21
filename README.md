# SaaS Metrics Dashboard: Key Insights & Recommendations


## CHALLENGE
You need to analyze SaaS business health across multiple dimensions:
- Track revenue growth (MRR/ARR trends)
- Understand customer acquisition efficiency (CAC, LTV:CAC)
- Monitor revenue and churn by plan tier
- Make data-driven decisions on where to invest S&M budget

The data is split across two sources with different granularities (monthly overall metrics vs quarterly tier breakdowns), making it challenging to get a unified view of business performance.

## ACTION
Build a multi-tab Tableau dashboard that answers key business questions:

### Dashboard Structure (4 main views)

**1. Executive Overview**
- Current MRR, ARR, total customers (big number KPIs)
- MRR growth trend line (monthly)
- Net new MRR waterfall (new + expansion - churn)
- Quick health metrics: churn rate, LTV:CAC ratio, CAC payback period

**2. Customer Acquisition**
- New customers by month (bar chart)
- CAC vs LTV trend over time
- Trial Conversion Rate
- Sales efficiency: Magic Number chart (net new MRR / S&M spend)

**3. Revenue & Retention**
- MRR composition: new vs expansion vs churned (stacked area)
- Churn rate % trend
- ARPU trend
- Customer lifetime value over time
- Revenue retention analysis

**4. Plan Tier Analysis**
- Customer distribution by tier (pie or bar)
- MRR by tier over time (stacked area)
- Churn rate comparison across tiers
- ARPU by tier


## RESULT

**Business insights you'll be able to extract:**

1. **Is the business healthy?**
   - LTV:CAC ratio trending up from 24x to 48x (target: >3x) ✅
   - Churn stabilizing around 2.1-2.5% (good for SMB SaaS)
   - CAC decreasing from $420 to $344 (improving efficiency)

2. **Where is growth coming from?**
   - New customer acquisition accelerating (18 → 98 per month)
   - Expansion MRR growing faster than new MRR (land-and-expand working)
   - Enterprise tier growing fastest (6 → 116 customers)

3. **Which tier should we focus on?**
   - Enterprise: $2,500 ARPU, 0% churn, but high CAC
   - Pro: $600 ARPU, <1% churn, best efficiency
   - Starter: $200 ARPU, 2-3% churn, but volume play

4. **What actions to take?**
   - Double down on Pro tier (best LTV:CAC)
   - Use Starter as lead gen funnel to Pro
   - Optimize Enterprise sales process (high CAC)
   - Expansion MRR is healthy - invest in customer success

5. **Financial trajectory**
   - MRR grew from $42K → $594K (27 months)
   - ARR reached $7.1M
   - Customer base 10x'd (118 → 1,224)
   - Unit economics improving across all metrics

## Executive Summary

**Business Health Score: Excellent (9/10)**

Over the 27-month period (Jan 2023 - Mar 2025), this SaaS business has demonstrated exceptional growth with continuously improving unit economics. MRR grew 14x from $42.6K to $593.9K, while customer count increased 10x from 118 to 1,224. Most importantly, efficiency metrics are trending in the right direction across the board.

---

## 🎯 Key Insights by Category

### 1. Revenue Growth & Scale

**What the data shows:**
- **MRR:** $42.6K → $593.9K (1,294% growth)
- **ARR:** $511K → $7.1M (1,293% growth)
- **Net New MRR acceleration:** Started at $7.6K/month, now at $35.1K/month
- **Expansion MRR overtook New MRR** in Q3 2024 (critical inflection point)

**Why this matters:**
- Revenue growth is not just from new customer acquisition
- Existing customers are expanding their usage and upgrading plans
- This indicates strong product-market fit and customer success

**The turning point:**
Around month 18-20 (mid-2024), expansion MRR began consistently exceeding $6K/month while maintaining lower churn, signaling the business entered a mature, efficient growth phase.

---

### 2. Customer Acquisition Efficiency

**What the data shows:**
- **CAC declining:** $420 → $344 (18% improvement)
- **CAC is dropping while customer acquisition is accelerating**
- New customers per month: 18 → 98 (5.4x increase)
- Trial conversion stable: ~31-32% consistently

**Why this matters:**
- You're getting better at acquiring customers for less money
- Marketing and sales processes are becoming more efficient
- Word-of-mouth and product-led growth are likely contributing

**Magic Number (Sales Efficiency):**
- Averaging 1.0-1.2 in recent months
- Benchmark: >0.75 is excellent
- **Status: Well above benchmark** ✅

**Recommendation:**
This is a green light to invest more in customer acquisition. When CAC is declining while volume increases, you've found repeatable, scalable channels.

---

### 3. Unit Economics (The Most Critical Metrics)

**LTV:CAC Ratio:**
- Started: 24x
- Current: 48x
- Benchmark: 3x+ is healthy, 5x+ is excellent
- **Status: Exceptionally strong** ✅✅✅

**What this means:**
For every $1 spent acquiring a customer, you're getting back $48 in lifetime value. This is extraordinarily high and indicates:
- Very low churn
- High ARPU relative to acquisition cost
- Long customer lifetimes
- Sustainable, profitable growth

**ARPU Trend:**
- $360 → $485 (35% increase)
- Growing steadily without major jumps
- Driven by expansion revenue and tier upgrades

**Customer Lifetime:**
- 28 months → 33+ months
- Customers are staying longer as the product matures
- Indicates increasing stickiness

---

### 4. Churn Analysis

**Monthly Churn Rate:**
- Started: 1.67%
- Peaked: 2.68% (mid-2023)
- Current: 2.12%
- Trend: **Improving and stabilizing**

**Why the early spike matters:**
The churn increase in months 6-10 is normal for early-stage SaaS. You were likely:
- Finding product-market fit
- Churning out bad-fit customers
- Learning who your ideal customer is

**Current state:**
2.12% monthly churn = ~25% annual churn, which is:
- Good for SMB SaaS (benchmark: 20-30%)
- Excellent given the customer count has 10x'd
- Improving (down from 2.5% six months ago)

**Revenue churn vs customer churn:**
Your churned MRR is growing slower than your customer base, suggesting:
- Smaller accounts churn more
- Higher-value accounts stick around
- You're moving upmarket successfully

---

### 5. Plan Tier Performance

**Customer Distribution (Mar 2025):**
- **Starter:** 598 customers (49%)
- **Pro:** 510 customers (42%)
- **Enterprise:** 116 customers (9%)

**Revenue Distribution (Mar 2025):**
- **Starter:** $119.6K MRR (17%)
- **Pro:** $306K MRR (42%)
- **Enterprise:** $295K MRR (41%)

**🔥 Critical Insight:**
Enterprise is only 9% of customers but generates 41% of revenue. This is the classic power law distribution you want to see.

**ARPU by Tier:**
- **Starter:** $200/month (fixed pricing)
- **Pro:** $600/month (fixed pricing)
- **Enterprise:** $2,543/month (custom contracts)

**Churn by Tier (Mar 2025):**
- **Starter:** 2.01% monthly churn
- **Pro:** 0.59% monthly churn
- **Enterprise:** 0% monthly churn

**What this tells us:**

1. **Starter is a volume play and lead gen funnel**
   - Highest customer count
   - Lowest ARPU
   - Highest churn
   - Purpose: Acquire customers cheaply, upgrade them later

2. **Pro is the sweet spot**
   - Best balance of ARPU and churn
   - Growing fastest in absolute numbers
   - Likely where most Starter users upgrade to
   - Most predictable revenue

3. **Enterprise is the profit center**
   - Highest ARPU by far ($2,543 vs $600)
   - Zero churn (incredible stickiness)
   - Growing rapidly (6 → 116 customers)
   - Likely has longer sales cycles and higher CAC

---

### 6. Growth Trajectory & Momentum

**Customer Growth Rate:**
- Q1 2023: +18-25 customers/month
- Q4 2024: +80-98 customers/month
- **4x acceleration in customer acquisition velocity**

**Revenue Growth Rate:**
- Early 2023: ~15-20% MoM
- Late 2024: ~7-10% MoM
- Slowing percentage but increasing absolute dollars (normal and healthy)

**The Rule of 40:**
Even at just 10% MoM growth, you'd score 120% annualized, far exceeding the 40% benchmark for healthy SaaS companies.

---

### 7. Trial Funnel Performance

**Trials started:** 110 → 572 (5.2x increase)
**Conversion rate:** Stable at 31-32%

**What this means:**
- Top of funnel is growing (good marketing)
- Conversion rate hasn't degraded (good product)
- You're maintaining quality while scaling quantity

**Opportunity:**
Even a 5% improvement in trial conversion (31% → 36%) would add significant MRR without increasing CAC. Small optimization here = big impact.

---

## 📊 Comparative Benchmarks

| Metric | Your Business | Industry Benchmark | Status |
|--------|---------------|-------------------|--------|
| LTV:CAC Ratio | 48x | 3-5x | ⭐️ Exceptional |
| Monthly Churn | 2.12% | 2-5% | ✅ Good |
| Magic Number | 1.0-1.2 | >0.75 | ✅ Excellent |
| CAC Payback | 8-10 months | 12-18 months | ⭐️ Excellent |
| Trial Conversion | 31% | 20-30% | ✅ Good |
| ARPU Growth | 35% over 27mo | 10-20%/year | ✅ Strong |

**Overall Assessment:** You're beating benchmarks across the board.

---

## 🚀 Strategic Recommendations

### Immediate Actions (Next 30 Days)

**1. Accelerate Enterprise Sales**
- **Why:** 0% churn, $2,543 ARPU, 41% of revenue from only 9% of customers
- **How:**
  - Hire 2-3 dedicated enterprise AEs
  - Create enterprise-specific marketing content
  - Build out case studies from existing Enterprise customers
  - Implement a white-glove onboarding process
- **Expected impact:** 20-30 new Enterprise customers over 12 months = +$600K-900K ARR

**2. Optimize Trial-to-Paid Conversion**
- **Why:** 31% is good but not great; 5% improvement = significant MRR gain
- **How:**
  - Add product-led growth features (in-app prompts, activation milestones)
  - Implement sales-assisted trials for high-intent users
  - A/B test trial length (7 days vs 14 days vs 30 days)
  - Add live onboarding webinars during trial period
- **Expected impact:** 31% → 35% = ~20 extra customers per month = $120K ARR

**3. Formalize the Starter → Pro Upgrade Path**
- **Why:** Pro has best unit economics; Starter is the feeder
- **How:**
  - Create usage-based triggers (when Starter hits certain limits, auto-suggest Pro)
  - Offer limited-time upgrade incentives
  - Build feature comparison tool showing Pro benefits
  - Sales outreach to Starter customers hitting limits
- **Expected impact:** Convert 10% of Starter base to Pro = +$240K ARR

---

### Short-Term Strategy (3-6 Months)

**4. Invest Heavily in Customer Success**
- **Why:** Expansion MRR is already strong ($8.4K/month); you can 2x this
- **How:**
  - Hire 2-3 CSMs focused on expansion
  - Create a systematic QBR process for Pro and Enterprise
  - Build expansion playbooks (when to upsell, cross-sell, upgrade)
  - Implement NPS surveys to identify expansion opportunities
- **Expected impact:** Expansion MRR from $8.4K → $15K/month = +$80K ARR

**5. Double Down on Acquisition Channels That Work**
- **Why:** CAC is dropping while volume increases = you've found PMF
- **How:**
  - Analyze which channels have lowest CAC
  - Allocate 60-70% of budget to proven channels
  - Keep 30-40% for testing new channels
  - Increase S&M spend by 30-50% (you can afford it with 48x LTV:CAC)
- **Expected impact:** Maintain or improve CAC while adding 50-75 more customers/month

**6. Address Starter Churn Specifically**
- **Why:** 2% churn is fine overall, but Starter at 2.01% is dragging average down
- **How:**
  - Improve onboarding for Starter users
  - Add more self-service resources
  - Identify common churn reasons via exit surveys
  - Consider price positioning (maybe Starter is too cheap, attracting wrong customers)
- **Expected impact:** Reduce Starter churn from 2.01% → 1.5% = retain 36 more customers/year

---

### Long-Term Strategy (6-12 Months)

**7. Launch a Partner/Reseller Program**
- **Why:** Expand reach without proportionally increasing CAC
- **How:**
  - Identify complementary products/services
  - Create attractive partner margins (20-30%)
  - Build partner portal and training materials
  - Focus on partners who serve your ICP
- **Expected impact:** 15-25% of new customers via partners within 12 months

**8. Develop a Land-and-Expand Motion**
- **Why:** You're already doing this organically; formalize it
- **How:**
  - Create "seats-based" pricing for teams
  - Build features that encourage viral growth (collaboration, sharing)
  - Offer team/department pilots in Enterprise accounts
  - Track account penetration and expansion over time
- **Expected impact:** Increase average customer lifetime to 36+ months, ARPU to $550+

**9. Consider International Expansion**
- **Why:** Your fundamentals are strong; ready to scale geographically
- **How:**
  - Start with English-speaking markets (UK, Australia, Canada)
  - Localize pricing and payment methods
  - Hire regional sales/marketing talent
  - Ensure product supports multi-currency and regional compliance
- **Expected impact:** 20-30% revenue boost from new geos in year 2

---

## ⚠️ Risks to Monitor

### 1. Churn Stabilization vs Reduction
**Risk:** Churn has stabilized at 2.1% but not improving further
**Watch for:** If churn starts creeping back up as you scale
**Mitigation:** Invest in CS team, improve onboarding, track leading indicators (usage metrics, support tickets)

### 2. Enterprise Concentration Risk
**Risk:** As Enterprise grows to 50%+ of revenue, losing 1-2 big accounts hurts more
**Watch for:** Over-dependence on handful of Enterprise customers
**Mitigation:** Diversify Enterprise base, implement health scores, assign dedicated CSMs

### 3. Market Saturation
**Risk:** Customer acquisition could slow as you penetrate your TAM
**Watch for:** CAC starting to rise, lower trial conversion, longer sales cycles
**Mitigation:** Expand TAM (new verticals, geographies, use cases)

### 4. Competitive Pressure
**Risk:** Competitors could compress pricing or steal market share
**Watch for:** Decreasing trial conversions, increasing churn, pressure to lower prices
**Mitigation:** Differentiate on features, double down on customer success, build moats (integrations, network effects)

---

## 🎯 90-Day Action Plan

### Month 1: Foundation
- [ ] Hire first Enterprise AE
- [ ] Launch trial conversion A/B tests
- [ ] Implement basic health scoring for Enterprise customers
- [ ] Analyze channel-level CAC to find winners

### Month 2: Execution
- [ ] Begin sales-assisted trial pilot
- [ ] Create Starter → Pro upgrade campaign
- [ ] Launch first Enterprise case study
- [ ] Hire first dedicated CSM focused on expansion

### Month 3: Scale
- [ ] Increase S&M spend by 30% in best-performing channels
- [ ] Roll out winning trial conversion optimizations
- [ ] Implement QBR process for top 25 Enterprise accounts
- [ ] Measure and report on all initiatives

**Expected Results After 90 Days:**
- +15-20 Enterprise customers
- Trial conversion up 2-3%
- 20-30 Starter → Pro upgrades
- Expansion MRR up 20%
- **Total impact: +$200-250K in new ARR**

---

## 💰 Financial Projections

**If you execute these recommendations:**

| Metric | Current (Mar 2025) | 12 Months (Projected) |
|--------|-------------------|----------------------|
| MRR | $594K | $950K - $1.1M |
| ARR | $7.1M | $11.4M - $13.2M |
| Customers | 1,224 | 2,000 - 2,200 |
| Churn Rate | 2.12% | 1.8% - 1.9% |
| LTV:CAC | 48x | 40x - 45x (still excellent) |
| Enterprise % | 9% | 12% - 15% |

**Conservative scenario:** 60% YoY growth to $11.4M ARR
**Aggressive scenario:** 85% YoY growth to $13.2M ARR

Both scenarios are achievable given your current trajectory and unit economics.

---

## 🏆 What You're Doing Right

**Celebrate these wins:**

1. **Unit economics are world-class** - 48x LTV:CAC is exceptional
2. **Expansion revenue is working** - Customers are growing with you
3. **Enterprise motion is strong** - 0% churn, growing rapidly
4. **CAC is improving at scale** - Getting more efficient, not less
5. **Product-market fit is clear** - All indicators point to PMF
6. **Healthy tier distribution** - Not over-dependent on any one tier
7. **Trial funnel is consistent** - Quality remains high as you scale

**The bottom line:** This business is firing on all cylinders. The foundation is strong. Now it's time to pour fuel on the fire and scale aggressively.

---

## 📞 Questions to Ask Your Team

Before implementing recommendations, gather this context:

1. **What's our current CAC by acquisition channel?** (Helps prioritize S&M spend)
2. **What % of Starter customers upgrade to Pro?** (Identifies upgrade friction)
3. **What's the average sales cycle for Enterprise?** (Informs hiring and capacity planning)
4. **What are the top 3 reasons customers churn?** (Guides retention initiatives)
5. **What features drive the most expansion revenue?** (Helps product roadmap)
6. **How many sales/marketing people do we have?** (Identifies capacity constraints)
7. **What's our current cash burn rate?** (Determines how aggressive to be with growth investments)

---

## Final Thoughts

You have a **rare combination**: explosive growth, improving efficiency, and strong unit economics. Most companies have to choose between growth and profitability. You can have both.

**The biggest risk right now is not being aggressive enough.** With 48x LTV:CAC and declining CAC, you should be investing heavily in growth. This is the time to step on the gas, not pump the brakes.

**Recommended investment areas (in priority order):**
1. Enterprise sales team (immediate ROI)
2. Customer success for expansion (high ROI, fast payback)
3. Marketing for customer acquisition (proven channels)
4. Product features that reduce churn (long-term value)

**Six months from now, you should be looking at:**
- $800K+ MRR
- 1,600+ customers
- 150+ Enterprise customers
- <2% churn rate
- Still 40x+ LTV:CAC

You've built something special. Now go scale it.
