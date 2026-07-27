# SaaS KPI Dictionary: Sales, Marketing & Customer Experience

## Purpose
A shared reference for the metrics that matter most in a $50M–$2B ARR SaaS business, with a consistent definition, formula, and benchmark for each — so Sales, Marketing, and CX are working from the same vocabulary rather than three functions quoting three slightly different numbers with the same name. Pairs with the [Segmentation Framework](segmentation-framework.md), [Sales Forecasting](sales-forecasting.md), and [Inspection Cadence](inspection-cadence.md) docs — this is the glossary those frameworks assume.

**How to read each entry:** Definition (what it means) → Formula (how it's calculated) → Why It Matters (what decision it informs) → Benchmark (illustrative range for $50M–$2B SaaS — validate against your own historicals before treating as a target) → Typical Owner.

---

## 1. Sales KPIs

### Pipeline Generation (PipeGen)
- **Definition:** New qualified pipeline created in a period.
- **Formula:** `Sum of new opportunity value created in period`
- **Why It Matters:** Leading indicator of future bookings; the earliest place a future miss becomes visible.
- **Benchmark:** Enough new pipeline each quarter to maintain 3–4x coverage on next-quarter quota.
- **Owner:** Sales (with Marketing co-ownership of sourced pipeline — see Section 2).

### Pipeline Coverage Ratio
- **Definition:** How many multiples of remaining quota are sitting in open pipeline.
- **Formula:** `Open Pipeline ÷ Remaining Quota`
- **Why It Matters:** The standard "will we hit the number" gut check — but should always be read alongside the weighted version below.
- **Benchmark:** 3–4x, varies by segment (Enterprise typically needs higher coverage than SMB due to lower win rates).
- **Owner:** Sales Ops / Sales Leadership.

### Stage-Weighted Pipeline Coverage
- **Definition:** Pipeline coverage adjusted for the historical win rate of each stage, rather than treating all open pipeline as equally likely to close.
- **Formula:** `Σ (Pipeline in Stage × Stage Win Rate) ÷ Remaining Quota`
- **Why It Matters:** A raw coverage ratio can look healthy while being full of early-stage deals unlikely to close this period — the weighted view catches that.
- **Benchmark:** ~1.0–1.2x (since it's already win-rate-adjusted, it should sit much closer to 1x than raw coverage).
- **Owner:** Sales Ops.

### Win Rate
- **Definition:** Share of qualified opportunities that close won.
- **Formula:** `Closed Won Opportunities ÷ (Closed Won + Closed Lost Opportunities)`
- **Why It Matters:** Core efficiency signal; segment/vertical/competitor cuts reveal where the motion is or isn't working.
- **Benchmark:** 20–30% for Enterprise/complex B2B; 30–45% for Mid-Market/SMB — highly motion-dependent.
- **Owner:** Sales Leadership.

### Average Deal Size (ACV)
- **Definition:** Average annual contract value of closed-won deals.
- **Formula:** `Total New ARR Closed ÷ Number of Deals Closed`
- **Why It Matters:** Tracks segment mix shift and pricing/packaging health; a falling ACV alongside a rising deal count can signal down-market drift.
- **Benchmark:** Highly segment-dependent — track trend more than absolute value.
- **Owner:** Sales Leadership / Finance.

### Sales Cycle Length
- **Definition:** Average time from opportunity creation (or MQL, depending on definition used) to closed-won.
- **Formula:** `Average (Close Date − Opportunity Create Date)`
- **Why It Matters:** Directly drives forecasting accuracy and capacity planning; lengthening cycles often precede a coverage or win-rate problem.
- **Benchmark:** 30–60 days SMB; 90–180+ days Enterprise.
- **Owner:** Sales Ops.

### Quota Attainment
- **Definition:** Share of reps hitting quota, and how much of quota the average rep achieves.
- **Formula:** `Reps at ≥100% Quota ÷ Total Quota-Carrying Reps` (and `Actual Bookings ÷ Quota` per rep)
- **Why It Matters:** The health check on whether territory design and quota-setting (see Territory Planning, Capacity Model) are actually working.
- **Benchmark:** 60–70% of reps at or above quota is a commonly cited healthy target; much lower suggests territory or quota design issues, much higher can suggest quotas are set too low.
- **Owner:** Sales Leadership / Sales Ops.

### New ARR / New Bookings
- **Definition:** New annual recurring revenue contracted in a period, excluding renewals.
- **Formula:** `Sum of ARR from new and expansion contracts signed in period`
- **Why It Matters:** The headline number most forecast and QBR conversations are ultimately about.
- **Benchmark:** N/A — set against company growth targets.
- **Owner:** Sales Leadership / Finance.

### Contracted ARR (cARR)
- **Definition:** Total ARR under contract at a point in time, including future-dated starts not yet live.
- **Formula:** `Live ARR + Signed-Not-Yet-Live ARR`
- **Why It Matters:** Distinguishes "sold" from "live and billing" — important in businesses with ramped or delayed-start contracts.
- **Benchmark:** N/A — track cARR vs. live ARR gap as a leading indicator of near-term revenue recognition.
- **Owner:** Finance / RevOps.

### Forecast Accuracy
- **Definition:** How close the Commit-category forecast was to actual closed bookings.
- **Formula:** `1 − (|Actual − Forecast| ÷ Forecast)`
- **Why It Matters:** The core scorecard for whether the forecasting process (MEDDICC-based categorization, manager forecast vs. roll-up) is actually working.
- **Benchmark:** ±5–10% at the Commit category is a common target for a mature forecasting process.
- **Owner:** Sales Ops.

### Rep Productivity (Ramped)
- **Definition:** Average bookings per fully-ramped, quota-carrying rep.
- **Formula:** `Total Bookings from Ramped Reps ÷ Number of Ramped Reps`
- **Why It Matters:** Core input to the Capacity Model — determines how many reps are needed to hit a target.
- **Benchmark:** Segment-specific; validate against your own historical attainment rather than external benchmarks.
- **Owner:** Sales Ops.

### Ramp Time to Productivity
- **Definition:** Time for a new rep to reach full quota-carrying productivity.
- **Formula:** `Average months from hire date to first quarter at ≥100% of mature-rep quota pace`
- **Why It Matters:** Directly feeds the ramp curve assumption in the Capacity Model; underestimating this creates a hiring plan that's short of what's actually needed.
- **Benchmark:** 3–6 months SMB/Mid-Market; 6–12 months Enterprise.
- **Owner:** Sales Enablement / Sales Ops.

---

## 2. Marketing KPIs

### Marketing Qualified Lead (MQL)
- **Definition:** A lead that has met a defined engagement/fit threshold indicating readiness for sales follow-up.
- **Formula:** Rule-based or scored threshold (varies by org) applied to raw leads.
- **Why It Matters:** Top of the funnel volume signal — but only useful alongside the conversion rates below it, not in isolation.
- **Benchmark:** N/A in absolute terms — track MQL→SQL conversion instead of MQL volume alone.
- **Owner:** Marketing.

### Sales Qualified Lead (SQL)
- **Definition:** An MQL that Sales has accepted as worth actively working.
- **Formula:** Count of leads passing Sales acceptance criteria.
- **Why It Matters:** The real handoff point between Marketing and Sales — SQL definitions being loosely enforced is one of the most common sources of Sales/Marketing friction.
- **Benchmark:** N/A — track MQL-to-SQL conversion rate (typically 20–40%) as the health signal.
- **Owner:** Marketing / Sales (jointly defined).

### Sales Qualified Opportunity (SQO)
- **Definition:** An SQL that has converted into a working sales opportunity with an associated pipeline value.
- **Formula:** Count of SQLs that become opportunities.
- **Why It Matters:** First point where Marketing-sourced activity has a dollar value attached to it.
- **Benchmark:** 40–60% SQL-to-SQO conversion is a reasonable range, highly motion-dependent.
- **Owner:** Marketing / Sales.

### Marketing-Sourced Pipeline %
- **Definition:** Share of total open pipeline where Marketing generated the original lead.
- **Formula:** `Marketing-Sourced Pipeline ÷ Total Open Pipeline`
- **Why It Matters:** The clearest, least-disputable measure of Marketing's revenue contribution — as distinct from "influenced" pipeline (below), which is a softer claim.
- **Benchmark:** Varies enormously by motion — PLG/inbound-led businesses often see 50%+, outbound-led Enterprise businesses often see 20–30%.
- **Owner:** Marketing / RevOps.

### Marketing-Influenced Pipeline %
- **Definition:** Share of pipeline that Marketing touched at any point in the buying journey, regardless of source.
- **Formula:** `Pipeline with ≥1 Marketing touchpoint ÷ Total Pipeline`
- **Why It Matters:** Useful for understanding content/campaign reach, but should never substitute for Sourced % in a contribution conversation — it's a much lower bar to clear.
- **Benchmark:** Often 60–90%+ — precisely because it's an easy bar to clear, treat with proportionate skepticism in QBRs.
- **Owner:** Marketing.

### Customer Acquisition Cost (CAC)
- **Definition:** Fully-loaded cost to acquire one new customer.
- **Formula:** `(Total Sales + Marketing Spend in Period) ÷ New Customers Acquired in Period`
- **Why It Matters:** Core unit economics input; rising CAC without rising deal size is an efficiency red flag.
- **Benchmark:** Track trend and CAC Payback (below) more than an absolute external benchmark.
- **Owner:** Marketing / Finance (jointly).

### CAC Payback Period
- **Definition:** Time required for the gross margin from a new customer to repay the CAC spent acquiring them.
- **Formula:** `CAC ÷ (Average Monthly Recurring Revenue per Customer × Gross Margin %)`
- **Why It Matters:** One of the most watched efficiency metrics by investors and boards at this ARR stage.
- **Benchmark:** 12–18 months is commonly considered healthy; 5–7 months is best-in-class.
- **Owner:** Finance / Marketing.

### Cost per MQL / Cost per SQL
- **Definition:** Marketing spend divided by MQLs or SQLs generated in a period.
- **Formula:** `Marketing Spend ÷ MQLs (or SQLs) Generated`
- **Why It Matters:** Campaign and channel efficiency comparison — most useful cut by channel/campaign, not as a single company-wide number.
- **Benchmark:** Highly channel- and industry-dependent — benchmark against your own channel mix over time.
- **Owner:** Marketing (Demand Gen).

### Marketing ROI / Pipeline-to-Spend Ratio
- **Definition:** Pipeline (or closed revenue) generated per dollar of marketing spend.
- **Formula:** `Marketing-Sourced Pipeline (or Revenue) ÷ Marketing Spend`
- **Why It Matters:** The budget-defense number — ties spend directly to a revenue outcome rather than an activity metric.
- **Benchmark:** Varies by channel and attribution model; track directionally, not against a single external number.
- **Owner:** Marketing / Finance.

---

## 3. Customer Experience (CX) / Customer Success KPIs

### Gross Revenue Retention (GRR)
- **Definition:** Share of starting-period ARR retained, excluding any expansion — the "how much did we keep" number.
- **Formula:** `(Starting ARR − Downgrades − Churned ARR) ÷ Starting ARR`
- **Why It Matters:** Purest measure of base retention; unlike NRR, can't be masked by strong expansion.
- **Benchmark:** 90%+ is generally considered healthy for mid-market/enterprise SaaS; below 85% signals a real retention problem.
- **Owner:** CX / Customer Success.

### Net Revenue Retention (NRR)
- **Definition:** Share of starting-period ARR retained including expansion, downgrades, and churn.
- **Formula:** `(Starting ARR + Expansion − Downgrades − Churned ARR) ÷ Starting ARR`
- **Why It Matters:** One of the single most-watched SaaS metrics at this scale — reflects both retention and account-growth motion in one number.
- **Benchmark:** 100–110% is solid; 110–120%+ is best-in-class for enterprise-focused SaaS.
- **Owner:** CX / Customer Success (with Sales for expansion).

### Logo Churn Rate
- **Definition:** Share of customers (by count, not revenue) lost in a period.
- **Formula:** `Customers Churned in Period ÷ Customers at Start of Period`
- **Why It Matters:** Revenue-weighted metrics (GRR/NRR) can hide a high volume of small-account churn — logo churn surfaces that separately.
- **Benchmark:** <10% annually is often considered healthy for SMB-heavy bases; enterprise-heavy bases should be materially lower.
- **Owner:** CX / Customer Success.

### Revenue Churn Rate
- **Definition:** Share of ARR lost to cancellations in a period (excludes downgrades, which GRR captures separately).
- **Formula:** `Churned ARR in Period ÷ Starting ARR`
- **Why It Matters:** The dollar-weighted counterpart to logo churn — reveals whether churn is concentrated in large or small accounts.
- **Benchmark:** <5–8% annually is a common healthy range for mid-market/enterprise SaaS.
- **Owner:** CX / Finance.

### Expansion Revenue / Expansion Rate
- **Definition:** Additional ARR generated from existing customers (upsell, cross-sell, seat growth) in a period.
- **Formula:** `Expansion ARR in Period ÷ Starting ARR`
- **Why It Matters:** The growth engine NRR depends on; low expansion alongside acceptable NRR usually means retention is fine but the account-growth motion isn't working.
- **Benchmark:** 10–30% of NRR uplift commonly comes from expansion in healthy enterprise SaaS motions.
- **Owner:** CX / Sales (Account Management).

### Customer Health Score
- **Definition:** A composite score (usage depth, support ticket volume/severity, engagement, sentiment) indicating renewal/expansion likelihood.
- **Formula:** Weighted composite, org-specific — commonly blends product usage, support signals, and relationship/engagement data.
- **Why It Matters:** Leading indicator for renewal risk — should trigger proactive CX intervention well before a renewal date, not just at it.
- **Benchmark:** N/A (org-specific scoring) — track the score's correlation with actual churn/expansion outcomes to validate it's predictive.
- **Owner:** CX / Customer Success.

### Renewal Rate
- **Definition:** Share of contracts up for renewal in a period that actually renew.
- **Formula:** `Contracts Renewed ÷ Contracts Up for Renewal`
- **Why It Matters:** A more contract-cycle-driven cousin of GRR/logo churn — useful for renewal capacity and pipeline coverage planning specifically.
- **Benchmark:** 85–95%+ depending on segment and contract length.
- **Owner:** CX / Customer Success.

### Renewal Pipeline Coverage
- **Definition:** Ratio of renewals currently tracking to close (secured/committed) against total renewals due in the period.
- **Formula:** `Secured/Committed Renewal ARR ÷ Total Renewal ARR Due`
- **Why It Matters:** The CX equivalent of Sales pipeline coverage — an early warning system for renewal shortfall.
- **Benchmark:** Should approach 1.0x well before the renewal period closes; large ongoing gaps late in the period indicate at-risk accounts aren't being resolved in time.
- **Owner:** CX / Customer Success.

### Time to Value (TTV)
- **Definition:** Time from contract signature to the customer realizing the core value/outcome of the product.
- **Formula:** `Date of first defined value milestone − Contract Signature Date`
- **Why It Matters:** Strongly correlated with both early churn risk and expansion readiness — slow TTV is one of the most common root causes of first-year churn.
- **Benchmark:** Highly product-dependent — track trend and correlation to churn rather than an external benchmark.
- **Owner:** CX / Onboarding.

### Net Promoter Score (NPS) / CSAT
- **Definition:** Customer-reported satisfaction/loyalty metrics — NPS (likelihood to recommend) and CSAT (satisfaction with a specific interaction).
- **Formula:** `NPS = % Promoters − % Detractors` (survey-based, 0–10 scale); `CSAT = % positive responses to a satisfaction survey`
- **Why It Matters:** Sentiment leading indicators — most useful tracked over time and cut by segment/account, not as a single point-in-time company score.
- **Benchmark:** NPS 30–50 is commonly considered good for B2B SaaS; 50+ is excellent. CSAT benchmarks vary by interaction type.
- **Owner:** CX.

### CS-to-ARR Ratio (Coverage)
- **Definition:** How much ARR each CSM/Customer Success headcount is responsible for.
- **Formula:** `Total ARR under CS coverage ÷ Number of CSMs`
- **Why It Matters:** The CX equivalent of sales territory capacity — too high a ratio means proactive health management becomes reactive firefighting.
- **Benchmark:** Widely variable by segment — Enterprise CSMs often cover $2–5M ARR each; SMB/tech-touch or pure digital-touch models can cover far more.
- **Owner:** CX Leadership.

---

## 4. Cross-Functional / Company-Level KPIs

These sit above any single function but depend on Sales, Marketing, and CX inputs together — they're the numbers a QBR ultimately has to reconcile.

### LTV:CAC Ratio
- **Definition:** Ratio of a customer's lifetime value to the cost of acquiring them.
- **Formula:** `Customer LTV ÷ CAC`, where `LTV = (Average Revenue per Account × Gross Margin %) ÷ Revenue Churn Rate`
- **Why It Matters:** The headline unit economics health check — ties Sales/Marketing acquisition efficiency to CX retention performance in a single ratio.
- **Benchmark:** 3:1 or higher is a commonly cited healthy target; below 1:1 means the business loses money on every customer acquired.
- **Owner:** Finance (inputs from Sales, Marketing, CX).

### Rule of 40
- **Definition:** A combined growth-plus-profitability health check.
- **Formula:** `YoY Revenue Growth Rate % + Profit Margin %` (commonly EBITDA or FCF margin)
- **Why It Matters:** A single number investors use to judge whether growth is being bought unsustainably or achieved efficiently.
- **Benchmark:** ≥40% combined is the named target; well below it invites scrutiny of either growth or efficiency (or both).
- **Owner:** Finance / Executive team.

### Magic Number
- **Definition:** Sales efficiency metric relating new ARR generated to the sales & marketing spend that generated it.
- **Formula:** `(Current Quarter ARR − Prior Quarter ARR) × 4 ÷ Prior Quarter Sales & Marketing Spend`
- **Why It Matters:** A quick efficiency gut-check on whether increased S&M spend is translating into proportionate new ARR.
- **Benchmark:** >0.75 is generally considered efficient; >1.0 suggests room to invest more aggressively in growth.
- **Owner:** Finance / RevOps.

### Burn Multiple
- **Definition:** Net cash burned per dollar of net new ARR added.
- **Formula:** `Net Cash Burn ÷ Net New ARR`
- **Why It Matters:** A capital-efficiency lens on growth, increasingly emphasized in board reporting since the shift toward efficient growth.
- **Benchmark:** <1.0x is considered excellent; 1–2x is reasonable; well above 2x invites scrutiny.
- **Owner:** Finance.

### ARR Growth Rate
- **Definition:** Year-over-year growth in total annual recurring revenue.
- **Formula:** `(Current Period ARR − Prior Period ARR) ÷ Prior Period ARR`
- **Why It Matters:** The single number everything else in this dictionary ultimately rolls up to explain.
- **Benchmark:** Expectations compress with scale — 40–60%+ is common near $50M ARR; 20–30% is more typical approaching $1–2B ARR.
- **Owner:** Executive team / Finance.

---

## 5. Notes on Using This Dictionary

- **Benchmarks are illustrative, not prescriptive.** Every range above should be validated against your own historical data (the same principle used throughout the Segmentation, Territory Planning, and Sales Forecasting frameworks) before being adopted as a target.
- **Definitions should be locked centrally, not per-team.** The single most common cause of Sales/Marketing/CX metric disputes is each function quietly using a slightly different formula for the "same" KPI (MQL definitions and NRR calculation methods are the two most frequent offenders) — Sales Ops/RevOps should own the canonical formula for each.
- **Cadence matters as much as definition.** Pair this dictionary with the Inspection Cadence framework: pipeline coverage and forecast accuracy are weekly/monthly metrics; NRR, Rule of 40, and Magic Number are quarterly-or-slower metrics. Reviewing a slow-moving metric weekly (or a fast-moving one only quarterly) undermines its usefulness either way.
