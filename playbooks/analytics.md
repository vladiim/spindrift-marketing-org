# Analytics Division Playbook

**Division:** Analytics
**Brand:** Spindrift — Sparkling Water Made with Real Squeezed Fruit
**Last Updated:** January 2026

---

## Core Responsibility

The Analytics Division is the measurement backbone and truth-teller of Spindrift's marketing organization. We ensure that every dollar spent, every campaign launched, and every strategic decision made is grounded in reliable data and honest interpretation.

In a competitive landscape where Liquid Death raises hundreds of millions on brand hype, LaCroix maintains shelf dominance through distribution muscle, and Topo Chico rides Coca-Cola's infrastructure, Spindrift must be smarter with its resources. Analytics makes "smarter" possible by answering three persistent questions: What is working? Why is it working? What should we do next?

We do not make strategic decisions — that is Strategy's role. But we ensure that strategic decisions are never made on intuition alone.

---

## What We Own

- **Measurement frameworks:** The architecture that defines what we measure, how we measure it, and what "good" looks like across all marketing activities.
- **Attribution modeling:** How we assign credit to touchpoints along the consumer journey — from first Spindrift awareness through trial, repeat purchase, and subscription.
- **Reporting and dashboards:** Weekly, monthly, and quarterly reporting packages for all divisions and leadership, plus self-serve dashboards for division-level operational metrics.
- **Forecasting:** Predictive models for customer acquisition, revenue, channel performance, and seasonal demand patterns.
- **Experimentation design:** Statistical methodology for A/B tests, multivariate tests, and holdout studies. We design the experiment; the executing division (typically Growth or Content) runs it.
- **Consumer and market research coordination:** Managing brand tracker studies, consumer surveys, category research subscriptions (Nielsen/IRI/Circana, Mintel), and ad-hoc research projects.
- **Data infrastructure and governance:** Ensuring data collection is accurate (tracking, tagging, pixel management), data storage is organized, and data access is governed (who can see what, and why).
- **Marketing mix modeling (MMM):** Periodic analysis of how spend across channels and tactics drives incremental revenue, accounting for baseline demand, seasonality, and external factors.

## What We Hand Off

| Deliverable | Receiving Division | Handoff Format |
|---|---|---|
| Strategic performance insights | Strategy | Monthly insights memo with interpreted findings, not just metrics — what does this mean for positioning and planning? |
| Channel performance data | Growth | Weekly dashboards with channel-level metrics; flagged anomalies with hypotheses |
| Content performance data | Content | Bi-weekly content performance report with engagement, traffic, and conversion metrics per content piece and pillar |
| Creative performance data | Creative | Monthly creative performance brief: which messages, visuals, and formats are outperforming/underperforming and why |
| Experiment results | Growth (or requesting division) | Statistical results with confidence levels, business impact estimates, and recommended actions |
| Forecasts | Strategy, Growth, Finance | Quarterly forecasts with scenarios (base, optimistic, conservative) and key assumptions |

**We do NOT own:** Strategic interpretation and decision-making (Strategy), creative direction based on performance data (Creative), channel optimization execution (Growth), or content production adjustments (Content). We illuminate; the other divisions act.

---

## Escalation Triggers

Escalate to Analytics Lead or VP of Marketing when:

1. **Data integrity failure:** Tracking or measurement system produces unreliable data for more than 48 hours — broken pixels, incorrect attribution, misreported conversions, or data pipeline failures. Unreliable data leads to bad decisions, which is worse than no data.
2. **Significant metric deviation:** Any primary KPI (revenue, CAC, ROAS, conversion rate, brand awareness) deviates more than 25% from forecast for 2 consecutive reporting periods without an identified cause. Investigate before escalating if possible, but do not wait more than 1 week to escalate an unexplained deviation.
3. **Attribution model conflict:** Different attribution models (last-touch, multi-touch, MMM) produce contradictory recommendations about channel investment. This requires a methodological discussion, not a data discussion.
4. **Privacy/compliance risk:** A data collection or targeting practice may conflict with CCPA, state privacy laws, platform policies (Apple ATT, Google Privacy Sandbox), or Spindrift's own data ethics standards. When in doubt, stop collecting and escalate.
5. **Research finding that challenges strategy:** Consumer research or brand tracking data reveals a finding that materially contradicts a current strategic assumption — e.g., brand awareness among a key target segment is declining despite increased investment, or Spindrift's "real fruit" positioning is not resonating with an emerging demographic.
6. **Forecast miss exceeding 20%:** Actual results deviate from forecast by more than 20% in either direction. Over-performance requires investigation too — was the forecast wrong, or did something unexpected happen that we should replicate?
7. **Cross-divisional data disagreement:** Two divisions are reporting different numbers for the same metric (e.g., Growth reports 5,000 new customers, Content reports 3,000 email signups from the same campaign, and the numbers don't reconcile). Resolve before conflicting data drives conflicting decisions.

---

## Quality Standards for Outputs

### Weekly Reports
- Must be delivered by end of day Monday for the prior week's performance (Sunday-Saturday).
- Must include: top-level KPI dashboard (revenue, new customers, website traffic, email list size, social followers, subscription count), channel-level performance summary, and a "flags and highlights" section identifying the 3 most notable data points from the week.
- Flags must include a hypothesis, not just a number. "DTC conversion rate dropped 15%" is incomplete. "DTC conversion rate dropped 15%, likely due to the checkout redesign deployed Wednesday — recommend reverting and testing incrementally" is useful.
- Data accuracy standard: all reported numbers must reconcile to source systems within a 2% tolerance. If discrepancies exceed 2%, note them and investigate.

### Monthly Deep-Dive Reports
- Must be delivered by the 10th business day of the following month.
- Must include: full-funnel analysis (awareness through retention), channel-by-channel performance with month-over-month and year-over-year trends, campaign-level performance for any campaigns active during the month, customer cohort analysis (how do customers acquired this month compare to prior cohorts on LTV trajectory?), and competitive context (share of voice, category growth rates).
- Must include an "insights" section (minimum 3 insights) that goes beyond reporting into interpretation. An insight connects data to action.
- Must include a "forecast check" — how did actuals compare to the forecast, and what adjustments are needed?

### Attribution Reports
- Must clearly state the attribution methodology used and its known limitations. There is no perfect attribution model — transparency about limitations builds trust.
- Must present results from at least two attribution approaches (e.g., last-touch + data-driven multi-touch, or multi-touch + MMM) to provide perspective rather than false precision.
- Must include a "confidence level" assessment: high (multiple data sources agree), medium (directional but noisy), or low (insufficient data or conflicting signals).
- Channel-level attribution findings must be accompanied by recommended spend implications and the estimated impact of reallocation.
- Updated quarterly at minimum; refreshed ad-hoc when significant channel mix changes occur.

### Experiment Design Documents
- Must include: hypothesis, test configuration, primary metric, secondary metrics, minimum sample size calculation, expected test duration, statistical significance threshold, and decision rules (what action will be taken for each possible outcome).
- Must be reviewed and approved by the Analytics Lead before any test launches.
- Must specify the "do nothing" baseline — what happens if we do not run this test? This prevents low-value testing.
- Post-test analysis must be completed within 5 business days of test conclusion and include: results, statistical confidence, estimated business impact (annualized), and recommended next steps.

### Forecasts
- Must include three scenarios: base (most likely), optimistic (+15-20% from base), and conservative (-15-20% from base).
- Must list all key assumptions explicitly. Hidden assumptions make forecasts useless when conditions change.
- Must include a sensitivity analysis: which assumptions, if wrong, would most change the forecast outcome?
- Must be updated quarterly and refreshed mid-quarter if actual results deviate from forecast by more than 15%.

---

## Key Workflows

### 1. Weekly Reporting

**Cadence:** Every Monday
**Purpose:** Provide the marketing organization with a consistent, reliable pulse on performance.

**Process:**
1. **Data pull (Monday morning):** Pull data from all source systems: Google Analytics (website), Shopify (DTC transactions), Amazon Seller Central / Vendor Central, email platform (Klaviyo/similar), social media platforms (native analytics + Sprout Social/similar), paid media platforms (Meta Ads Manager, Google Ads, TikTok Ads), and CRM.
2. **Data validation:** Cross-reference key metrics across systems. Ensure transaction counts match between Shopify and GA. Ensure ad spend matches between platform and finance records. Flag discrepancies exceeding 2%.
3. **Dashboard update:** Update the master marketing dashboard with current-week data. Dashboard structure:
   - **Page 1: Executive summary** — Revenue (DTC + retail estimate), new customers, CAC, ROAS, website sessions, email list size, subscription count.
   - **Page 2: Channel performance** — Paid social, paid search, organic social, email, SEO, retail media, sampling. Each with spend, impressions, clicks/sessions, conversions, CPA/ROAS.
   - **Page 3: Content performance** — Top 5 performing pieces of content by engagement, top 5 by conversion, bottom 5 by engagement (to identify what is not working).
   - **Page 4: Competitive pulse** — Share of voice estimate, notable competitor activity (from Strategy's weekly scan).
4. **Flags and highlights:** Identify the 3-5 most notable data points. Write a hypothesis for each. Prioritize anomalies, trend changes, and milestone achievements.
5. **Distribution:** Send the report to all division leads and VP of Marketing by 4pm ET Monday. The report should be digestible in under 10 minutes.

**Output:** Weekly Marketing Performance Report (dashboard + narrative summary).

### 2. Monthly Deep-Dive

**Cadence:** Monthly (delivered by 10th business day)
**Purpose:** Go beyond weekly reporting to identify trends, cohort behaviors, and strategic implications that only emerge over a monthly timeframe.

**Process:**
1. **Full-funnel analysis (Days 1-3):**
   - Map the complete customer journey from awareness to retention with conversion rates at each stage.
   - Compare to prior month and same month prior year.
   - Identify the stage with the largest absolute drop — this is where the most revenue opportunity exists.
   - Segment by channel: do customers from Meta convert differently than customers from Instacart? Do podcast-acquired customers retain better?
2. **Channel deep-dive (Days 3-5):**
   - For each active channel, analyze: spend, volume, efficiency (CPA/ROAS), trend, and comparison to benchmark.
   - Identify channels exhibiting diminishing returns (spend increasing but efficiency declining) — these need optimization or spend capping.
   - Identify channels with untapped headroom (efficiency is strong but spend is low) — these are candidates for Growth's next budget allocation.
3. **Campaign analysis (Days 5-7):**
   - For each campaign that was active during the month, report: impressions, engagement, conversions, cost per conversion, and estimated brand lift (if measured).
   - Compare campaign performance to the creative brief's success metrics. Did the campaign deliver what was promised?
   - Extract creative learnings: which messages, formats, and audiences drove the strongest results? Feed these to Creative Division.
4. **Customer cohort analysis (Days 7-8):**
   - Analyze the current month's acquired customers: acquisition source, first order value, subscription opt-in rate, and early engagement signals.
   - Compare to the prior 3 monthly cohorts on the same metrics.
   - Track existing cohorts' progression: 30-day repeat rate, 60-day repeat rate, 90-day LTV projection.
   - Flag if any cohort is underperforming historical benchmarks — this may indicate traffic quality issues or onboarding experience problems.
5. **Insights and recommendations (Days 8-10):**
   - Write 3-5 insights that connect data to strategic or tactical action.
   - Example insight format: "Observation: TikTok-acquired customers have a 25% higher 60-day repeat rate than Meta-acquired customers. Hypothesis: TikTok's format lets us showcase the real-fruit visual difference more effectively, leading to higher product understanding before first purchase. Recommendation: Reallocate 10% of Meta prospecting budget to TikTok for a 60-day test, with cohort LTV as the primary evaluation metric."
   - Include a forecast check: actuals vs. forecast, with adjustment recommendations.
6. **Stakeholder review:** Present findings to division leads at the monthly marketing review meeting. Facilitate discussion on implications and actions.

**Output:** Monthly Marketing Deep-Dive Report, updated cohort tracking, forecast revision (if needed).

### 3. Attribution Modeling

**Cadence:** Quarterly (full refresh), continuous (monitoring)
**Purpose:** Understand the true incremental contribution of each marketing channel and tactic to Spindrift's revenue.

**Spindrift's Attribution Challenge:**
Spindrift sells through multiple channels (DTC, Amazon, grocery, convenience, club) but only has transaction-level data for DTC and Amazon. Retail sales are measured through syndicated data (Nielsen/Circana) with 4-6 week lag. This means attribution must blend:
- **Digital attribution** (pixel-based, multi-touch) for DTC and Amazon
- **Marketing mix modeling** (econometric) for total business including retail
- **Incrementality testing** (holdout/geo-experiments) for causal validation

**Process:**
1. **Digital attribution maintenance:**
   - Maintain UTM taxonomy and enforce tagging standards across all digital campaigns. UTM audit: monthly.
   - Run a multi-touch attribution model (data-driven or time-decay) for DTC and Amazon. Compare to last-touch as a sanity check.
   - Key output: channel-level CPA and ROAS on a multi-touch basis, with comparison to last-touch.
   - Known limitation: iOS ATT opt-out rates (~75%) mean that Meta and other app-based channels are likely under-credited in pixel-based attribution. Supplement with Meta's Conversion API and aggregate measurement tools.

2. **Marketing mix modeling (quarterly):**
   - Work with an MMM partner or internal data science resource to model the relationship between marketing spend (by channel), base demand, seasonality, pricing, competitive activity, and total revenue (DTC + retail).
   - Key output: channel-level marginal ROI curves — where is the next dollar of spend most productive?
   - Lag the model by one quarter to incorporate retail syndicated data.
   - Validate MMM findings against digital attribution and incrementality tests. Directional agreement across methods builds confidence.

3. **Incrementality testing (2-4 per year):**
   - Design and execute geo-based or audience-based holdout experiments to measure the true incremental impact of specific channels or campaigns.
   - Example: Pause all paid social in 3 matched DMAs for 4 weeks. Measure DTC and retail sales impact vs. control DMAs. This provides causal evidence that supplements correlational attribution models.
   - Prioritize incrementality tests for the highest-spend channels and any channel where digital attribution and MMM disagree.

4. **Attribution synthesis (quarterly):**
   - Combine findings from digital attribution, MMM, and incrementality tests into a unified view.
   - Present a "confidence-weighted" channel performance table: for each channel, show the CPA/ROAS range across methods, the confidence level, and the recommended spend direction (increase, maintain, decrease, test further).
   - Distribute to Strategy (for planning) and Growth (for execution).

**Output:** Quarterly Attribution Report, channel-level confidence-weighted performance table, incrementality test results.

### 4. Experiment Design

**Cadence:** Continuous — support all divisions' testing needs
**Purpose:** Ensure that every experiment Spindrift runs is methodologically sound and produces actionable results.

**Process:**
1. **Intake:**
   - Receive test requests from Growth (channel/funnel tests), Creative (concept/message tests), Content (format/cadence tests), or Strategy (pricing/positioning tests).
   - Evaluate each request for: clarity of hypothesis, testability, potential business impact, and resource requirements.
   - Reject or revise requests that are untestable (no measurable outcome), trivial (impact too small to matter), or duplicative (we already know the answer from prior tests).

2. **Design:**
   - Define the statistical framework:
     - **Sample size:** Calculate required sample per variant using the baseline conversion rate, minimum detectable effect (MDE), significance level (alpha = 0.05), and power (1 - beta = 0.80). For Spindrift's DTC, a 10% relative lift on a 3% conversion rate with 80% power requires ~14,500 visitors per variant.
     - **Duration:** Minimum 7 days for any test to capture day-of-week effects. Extend for tests with lower traffic or smaller expected effects.
     - **Segmentation:** Define the test population and any exclusion criteria. Ensure test and control populations are comparable.
   - Document the experiment design using the standardized experiment design template.
   - Review with the requesting division to ensure the design answers their actual question.

3. **Monitoring:**
   - Set up automated monitoring for data quality issues (sample ratio mismatch, tracking failures, audience contamination).
   - Conduct a mid-test health check: are we on pace for the planned sample size? Is the randomization holding? Are there any external confounds (e.g., a PR event that affects one variant's audience differently)?
   - Do NOT peek at results to make early calls. Sequential testing methods (if used) must be pre-specified, not applied retroactively to justify early stopping.

4. **Analysis:**
   - Run the pre-specified statistical test. Report the point estimate, confidence interval, and p-value.
   - For business interpretation: translate the statistical result into estimated revenue impact. "Variant B increased conversion by 12% (95% CI: 4%-20%), which at current traffic would generate approximately $XX,000 in additional annual revenue."
   - Assess secondary metrics for unintended consequences (e.g., a conversion rate increase that is accompanied by a decrease in average order value or increase in return rate).
   - Check for segment-level differences: did the treatment effect vary by audience, device, or geography? This can reveal opportunities for personalization.

5. **Documentation and learning:**
   - Log the experiment in the centralized experiment repository with: hypothesis, design, results, decision, and learnings.
   - Tag experiments by category (channel, creative, funnel, pricing, product) for pattern analysis.
   - Quarterly: review the experiment repository for meta-patterns. Are there consistent learnings that should become permanent operating principles? (e.g., if real-fruit close-up imagery has won 8 out of 10 creative tests, stop testing it — it is a proven principle.)

**Output:** Experiment design document, experiment results report, updated experiment repository.

---

## Division Operating Rhythm

| Activity | Frequency | Participants |
|---|---|---|
| Data quality check | Daily (automated + manual review) | Analytics team |
| Weekly report production | Monday | Analytics team |
| Test monitoring review | Twice weekly (Tue/Thu) | Analytics lead + relevant test owner |
| Cross-divisional sync | Bi-weekly (Thursday) | All division leads |
| Monthly deep-dive production | First 10 business days of month | Analytics team |
| Monthly deep-dive presentation | Second or third week of month | All division leads + leadership |
| Attribution model refresh | Quarterly | Analytics lead + data science |
| Forecast update | Quarterly (mid-quarter refresh if needed) | Analytics + Strategy + Finance |
| Experiment repository review | Quarterly | Analytics team + all divisions |
| Measurement framework audit | Semi-annual | Analytics lead + VP Marketing |

---

## Spindrift Measurement Framework

### Tier 1: Business Outcomes (reported monthly, tracked weekly)
| Metric | Definition | Current Benchmark | Target |
|---|---|---|---|
| Total revenue (DTC + Amazon) | Gross revenue from owned digital channels | Track from Shopify + Amazon | 20% YoY growth |
| Retail revenue (estimated) | Revenue from grocery/convenience/club channels via Nielsen/Circana | Track from syndicated data | 15% YoY growth |
| New customer count | Unique first-time purchasers (DTC + Amazon) | Track from CRM | 25% YoY growth |
| Customer LTV (12-month) | Average revenue per customer in first 12 months | Track from cohort analysis | $45-55 |
| Subscription count | Active Spindrift subscriptions | Track from Shopify/subscription platform | 30% YoY growth |

### Tier 2: Marketing Efficiency (reported weekly)
| Metric | Definition | Target |
|---|---|---|
| Blended CAC | Total marketing spend / new customers acquired | <$18 (first purchase) |
| Blended ROAS | Revenue / ad spend (on 90-day LTV basis) | >3.0x |
| Email revenue per send | Revenue attributed to email / number of emails sent | >$0.15 |
| Organic traffic share | Organic sessions / total sessions | >40% |
| Subscription conversion rate | Subscribers / first-time purchasers | >10% |

### Tier 3: Brand Health (reported quarterly)
| Metric | Definition | Source |
|---|---|---|
| Aided brand awareness | % of sparkling water consumers who recognize Spindrift | Brand tracker survey |
| Unaided brand awareness | % of sparkling water consumers who name Spindrift unprompted | Brand tracker survey |
| "Real fruit" attribute ownership | % who associate "made with real fruit" with Spindrift (vs. competitors) | Brand tracker survey |
| Net Promoter Score | Likelihood to recommend (scale -100 to 100) | Post-purchase survey |
| Social sentiment score | Positive / (positive + negative) mentions | Social listening tool |

### Tier 4: Operational Metrics (reported per-division, as needed)
Each division has specific operational metrics (see individual playbooks). Analytics ensures these metrics are accurately tracked and accessible via self-serve dashboards.

---

## Data Stack and Tools

| Function | Tool | Owner |
|---|---|---|
| Web analytics | Google Analytics 4 | Analytics |
| E-commerce | Shopify Analytics + custom reports | Analytics |
| Email analytics | Klaviyo (or equivalent) | Content (operational), Analytics (reporting) |
| Social analytics | Sprout Social + native platform analytics | Content (operational), Analytics (reporting) |
| Paid media | Meta Ads Manager, Google Ads, TikTok Ads Manager | Growth (operational), Analytics (reporting) |
| Retail data | Nielsen/Circana, retailer portals | Analytics |
| Attribution | Triple Whale / Northbeam (or equivalent DTC attribution) | Analytics |
| MMM | Internal model or partner (Recast, Measured) | Analytics |
| Dashboards | Looker / Tableau / Google Data Studio | Analytics |
| Experimentation | Optimizely / VWO (web), platform-native (paid media) | Analytics (design), Growth/Content (execution) |
| Survey/Research | Typeform, SurveyMonkey, research partner | Analytics |
| Data warehouse | BigQuery / Snowflake | Analytics + Engineering |

---

## Appendix: Experiment Repository Template

| Field | Description |
|---|---|
| Experiment ID | Auto-incrementing (EXP-001, EXP-002, etc.) |
| Date started | YYYY-MM-DD |
| Date concluded | YYYY-MM-DD |
| Requesting division | Strategy / Creative / Growth / Content |
| Category | Channel / Creative / Funnel / Pricing / Product |
| Hypothesis | "We believe [change] will [impact metric] because [rationale]" |
| Test configuration | Control description, variant(s) description, audience, channel |
| Primary metric | The single metric used to determine success |
| Secondary metrics | Additional metrics monitored for unintended effects |
| Sample size (planned) | Per variant |
| Sample size (actual) | Per variant |
| Duration (planned) | Days |
| Duration (actual) | Days |
| Result | Winner (Control / Variant A / Variant B / Inconclusive) |
| Statistical confidence | p-value and confidence interval |
| Effect size | Absolute and relative change in primary metric |
| Business impact (estimated) | Annualized revenue/cost impact |
| Decision | Implement / Iterate / Abandon |
| Key learnings | What did we learn beyond the primary result? |
| Tags | For pattern analysis (e.g., "real-fruit-imagery," "pricing," "TikTok") |
