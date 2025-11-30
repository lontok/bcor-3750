# IRPM Framework Reference

## Framework Structure

The IRPM Framework must be applied to EVERY analysis component in Milestone 1. This framework ensures students connect data findings to business actions and measurable outcomes.

```
┌─────────────────────────────────────────────────────────────┐
│ I - INSIGHT: What did you discover?                         │
│     → The data-driven finding or pattern you observed       │
│                                                              │
│ R - RECOMMENDATION: What should stakeholder do?             │
│     → Specific, actionable advice based on the insight      │
│                                                              │
│ P - PREDICTION: What outcome do you expect?                 │
│     → Quantifiable result if recommendation is followed     │
│                                                              │
│ M - METHOD: How did you analyze the data?                   │
│     → Steps, Excel functions/tools, reasoning               │
└─────────────────────────────────────────────────────────────┘
```

## Minimum IRPM Cycles Required (Milestone 1)

Students must complete IRPM for **6 analysis components**:
1. Descriptive Statistics - Central Tendency
2. Descriptive Statistics - Variability
3. Strategic Dashboard - ONE chart
4. Diagnostic PivotTable #1
5. Diagnostic PivotTable #2
6. Operational Dashboard - ONE chart

## Complete Examples

### Example 1: Central Tendency Analysis

**I - INSIGHT:**
"Typical delivery time is 4.2 days (median), not 5.1 days (mean skewed by outliers)"

**R - RECOMMENDATION:**
"Use median (4.2 days) as the performance benchmark instead of mean when setting targets and evaluating performance"

**P - PREDICTION:**
"Setting realistic targets based on median will improve on-time performance within 3 months as teams focus on achievable goals"

**M - METHOD:**
"Used Excel's Descriptive Statistics tool (Data Analysis ToolPak) to calculate mean (5.1), median (4.2), and mode for the Delivery_Time column across 1,247 orders. Identified outliers (delivery times >10 days) that skewed the mean upward."

---

### Example 2: Variability Analysis

**I - INSIGHT:**
"Delivery times vary wildly (standard deviation = ±2.8 days), creating unpredictable customer experience. Coefficient of variation is 67%, indicating high inconsistency."

**R - RECOMMENDATION:**
"Implement standardized fulfillment procedures and assign specific time slots for each warehouse to reduce variability by 40%"

**P - PREDICTION:**
"Reducing delivery time variability will decrease customer complaints and improve repeat purchase rate"

**M - METHOD:**
"Used Excel's Descriptive Statistics tool to calculate standard deviation (2.8 days), variance (7.84), and range (12 days). Calculated coefficient of variation (std dev / mean = 2.8 / 4.2 = 67%) to assess relative variability."

---

### Example 3: Diagnostic PivotTable (Root Cause Analysis)

**I - INSIGHT:**
"East Region accounts for 65% of late deliveries (>5 days) despite representing only 35% of total orders. Average delivery time in East Region is 7.3 days vs. 3.1 days in other regions."

**R - RECOMMENDATION:**
"Hire 2 additional warehouse staff in East Region and reassign 30% of East Region orders to the Central Region warehouse to reduce backlog"

**P - PREDICTION:**
"These changes will reduce East Region average delivery time and cut late deliveries significantly within 2 months"

**M - METHOD:**
"Created PivotTable with Region in Rows and Average of Delivery_Time in Values. Added conditional formatting (color scale) to highlight worst performers. Used Slicer to filter by Order_Status = 'Late' to identify regional patterns."

---

### Example 4: Strategic Dashboard - Trend Chart

**I - INSIGHT:**
"Order volume peaked in Q2 (April-June) at 450 orders/month, then declined 35% to 290 orders/month in Q3 despite stable pricing and no competitor changes"

**R - RECOMMENDATION:**
"Launch marketing campaign targeting lapsed customers from Q2 and investigate Q3 customer satisfaction drop"

**P - PREDICTION:**
"Reactivating lapsed Q2 customers will increase Q4 order volume significantly compared to Q3"

**M - METHOD:**
"Created line chart in Strategic Dashboard showing Order_Count by Month (Jan-Sept). Used COUNTIFS formula to count orders by month. Added trendline to visualize decline pattern."

---

### Example 5: Operational Dashboard - Root Cause Breakdown

**I - INSIGHT:**
"Morning shift (6am-2pm) has 2x higher defect rate (8.2%) compared to afternoon shift (3.9%), with 73% of defects occurring before 10am"

**R - RECOMMENDATION:**
"Add quality checkpoints at 8am and 9am for morning shift, and provide additional training on equipment warmup procedures"

**P - PREDICTION:**
"Enhanced quality controls will reduce morning shift defect rate and save money on rework costs within 4 weeks"

**M - METHOD:**
"Created bar chart in Operational Dashboard comparing Defect_Rate by Shift (Rows: Shift, Values: Average of Defect_Rate). Added second PivotTable breaking down by Hour to identify 6am-10am spike pattern."

## Common Mistakes to Avoid

### ❌ POOR Examples:

**Weak Insight:**
"The mean is 5.1 days"
- Problem: States a number without interpretation

**Generic Recommendation:**
"Improve delivery times"
- Problem: Not specific or actionable

**Vague Prediction:**
"Things will get better"
- Problem: Not quantifiable or measurable

**Incomplete Method:**
"I used Excel"
- Problem: No detail on specific functions or steps

---

### ✅ STRONG Examples:

**Strong Insight:**
"Typical delivery time is 4.2 days (median), not 5.1 days (mean skewed by 15% of orders taking >10 days)"
- Why: Interprets what the number means AND explains the pattern

**Specific Recommendation:**
"Use median (4.2 days) as performance benchmark when setting team targets and evaluating warehouse efficiency"
- Why: Exact action for specific stakeholder decision

**Quantifiable Prediction:**
"Setting realistic 4.2-day targets (vs current 5.1-day targets) will improve on-time performance from 68% to 82% within 3 months"
- Why: Measurable outcome with timeframe

**Detailed Method:**
"Used Excel's Descriptive Statistics tool (Data → Data Analysis → Descriptive Statistics) on Delivery_Time column for 1,247 orders, calculated mean (5.1), median (4.2), mode (3.0), std dev (2.8), and identified outliers >10 days"
- Why: Specific tools, functions, data, and reasoning

## IRPM Validation Checklist (for Interview Coach)

When a student presents an analysis component, validate ALL four elements:

**✅ INSIGHT:**
- [ ] States a clear finding from the data
- [ ] Interprets what it means (not just a number)
- [ ] Connects to business context

**✅ RECOMMENDATION:**
- [ ] Specific action for the stakeholder
- [ ] Actionable (stakeholder can implement it)
- [ ] Connected directly to the insight

**✅ PREDICTION:**
- [ ] Quantifiable outcome expected
- [ ] Includes timeframe when possible
- [ ] Realistic and defendable

**✅ METHOD:**
- [ ] Describes Excel functions/tools used
- [ ] Explains data used and why
- [ ] Shows analytical reasoning

## Interview Questioning Strategy (IRPM)

### If student provides incomplete IRPM:

**Student says:** "My central tendency analysis showed the average delivery time is 5.1 days"

**Coach prompts:**
1. "Okay, you've told me the number. What's your INSIGHT - what does 5.1 days mean for your stakeholder?"
2. [After insight] "Good. Now what's your RECOMMENDATION - what should [stakeholder name] DO with this information?"
3. [After recommendation] "And what PREDICTION do you make - what measurable outcome will happen if they follow your advice?"
4. [After prediction] "Finally, walk me through your METHOD - how exactly did you calculate this in Excel?"

### If student struggles with a specific component:

**For Insight** (if they just state a number):
- "What pattern or finding did you discover in the data?"
- "What does that number tell you about the business situation?"

**For Recommendation** (if too generic):
- "Be specific - what exact action should [stakeholder name] take?"
- "If you were sitting in a meeting with your stakeholder right now, what would you tell them to do tomorrow?"

**For Prediction** (if not quantifiable):
- "Put a number on it - how much improvement do you expect?"
- "In 3 months, what metric will show this worked?"

**For Method** (if incomplete):
- "Walk me through the Excel steps - what did you click, what formulas did you use?"
- "How did you get from the raw data to this finding?"

## Template for Students

Students can use this template structure for EACH of the 5 required components:

```
Component: [Central Tendency / Variability / Strategic Chart / Pivot 1 / Pivot 2]

I - INSIGHT:
[One sentence describing the key finding and what it means]

R - RECOMMENDATION:
[One sentence with specific action for stakeholder]

P - PREDICTION:
[One sentence with quantifiable expected outcome]

M - METHOD:
[2-3 sentences describing Excel tools, data used, and steps taken]
```

## Integration with Interview Assessment

The IRPM Framework directly maps to interview rubric dimensions:

**Depth of Understanding (40%):**
- Tests: Can they explain METHOD and defend analytical choices?

**Business Acumen (30%):**
- Tests: Quality of INSIGHT and RECOMMENDATION - do they connect to business problems?

**Communication Skills (20%):**
- Tests: Can they articulate all 4 components clearly and logically?

**Synthesis & Progression (10%):**
- Tests: Do INSIGHTs build on each other across components?

---

**Source References:**
- Study Guide lines 85-101 (IRPM Framework definition)
- Study Guide lines 105-115 (Analysis Coverage Table with IRPM requirements)
- Project Requirements lines 578-582 (Descriptive Statistics requirements)
- Project Requirements lines 584-608 (Diagnostic Analytics requirements)
