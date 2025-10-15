# Milestone 1 Requirements Excerpt
## For BCOR 3750 Midterm Interview Practice

This document contains the essential Milestone 1 requirements students need to understand for their midterm interview.

---

## Milestone 1: Descriptive & Diagnostic Analytics

**Due: Monday, October 20, 2025 by 8:00 AM**
**Weight: 15% of final grade**

### What You're Answering:
- **Descriptive**: "What happened?" - Summary, trends, patterns
- **Diagnostic**: "Why did it happen?" - Root cause analysis

---

## Project Foundation (Required for Interview)

### 1. Job Description
- Real, currently posted job in operations/supply chain management
- Entry-level position (analyst, coordinator, specialist roles)
- Saved as PDF

### 2. Operations Management Decision Area
Select ONE from:
1. Design of Goods & Services
2. Quality Management
3. Process & Capacity Design
4. Location Strategy
5. Layout Strategy
6. Human Resources & Job Design
7. Supply Chain Management
8. Inventory Management
9. Scheduling
10. Maintenance

### 3. Stakeholder
- Specific job title from job posting or related role
- Real person found on LinkedIn (when possible)
- Documented: name, title, company, LinkedIn URL, 2-3 key responsibilities

### 4. Problem Statement
**Required Format:**
> "[Stakeholder] at [Company] is facing [problem] which is causing [impact]."

**Must include:**
- Specific stakeholder and company
- Measurable challenge
- Business impact (why this matters)
- Current state (what's not working)
- Addressable through descriptive and diagnostic analytics

---

## Data Requirements

### Data Dictionary
**Required worksheet: Data_Dictionary**

Columns:
1. **Column Name**: Exact field name from dataset
2. **Data Type**: Text, Number, Date, Boolean, etc.
3. **Notes**: Additional context (valid ranges, formats, business rules, categories)

### Data Quality Assessment
**Required worksheet: Data_Cleaning_Log**

Must document minimum **3 different types** of data quality issues using the **Data Quality Framework**:

**5-Step Framework:**
1. **Identify** the data quality issue (what type?)
2. **Assess** the business ramification (why does this matter?)
3. **Analyze** the root cause (why did this occur?) - hypothetical reason
4. **Decide** on best option (Remove / Update / Do Nothing)
5. **Fix** the issue, if applicable (implement decision)

**Data Quality Dimensions:**
- Availability, Accuracy, Completeness, Consistency, Validity, Uniqueness, Timeliness

**Cleaning Log Columns:**
- Column (field with issue)
- Issue (type of data quality issue)
- Ramification (business impact)
- Root Cause (hypothetical reason)
- Decision (Update/Remove/Do Nothing)
- File Fix Method (how you fixed it)
- Preventative Measure (how to prevent in future)

---

## Analysis Requirements

### Descriptive Statistics
**Required worksheet: Descriptive_Statistics**

Analyze **primary metric of interest** (key metric related to problem statement)

**Must include:**
- All measures of central tendency (mean, median, mode)
- All variability measures (standard deviation, range, coefficient of variation)
- Histogram showing distribution
- Supports Slides 5-7 (Primary Metric Definition, Central Tendency Insight, Variability Insight)

### Diagnostic Analytics
**Required worksheet: Diagnostic_Pivot_Tables**

**Minimum 2 pivot tables**, each with:
- **Structure:** Row labels (1+ categorical variable), Values (numeric metric with aggregation)
- **Enhancements:** Pivot chart, at least one slicer, conditional formatting, professional formatting

### Dashboards

**Two dashboards required:**

**Dashboard #1: Strategic Dashboard (For Executives)**
- Purpose: High-level view of what happened
- Audience: Executives needing quick insights
- **Required Components:**
  - At least 2 scorecards (KPIs with comparisons)
  - 1 line chart (trend over time)
  - 1 bar chart (high-level comparison)
  - At least 1 slicer/filter
  - Cross-filtering enabled (if tool supports)

**Dashboard #2: Operational Dashboard (For Operations Staff)**
- Purpose: Detailed view for root cause analysis
- Audience: Operations managers/analysts for tactical decisions
- **Required Components:**
  - At least 2 scorecards (operational KPIs with comparisons)
  - 1 line chart (time-based patterns)
  - 1 bar chart (operational dimensions comparison)
  - At least 1 slicer/filter
  - Cross-filtering enabled (if tool supports)

**Dashboard Options:**
- Option 1: Excel dashboards (within workbook)
- Option 2: External tools (Tableau, Power BI, Looker Studio) - must be publicly accessible

---

## IRPM Framework (CRITICAL)

**Must be applied to EVERY analysis component (5 minimum cycles):**

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

**5 Required IRPM Cycles:**
1. Descriptive Statistics - Central Tendency
2. Descriptive Statistics - Variability
3. Strategic Dashboard - ONE chart (Scorecard, Trend, OR Breakdown)
4. Diagnostic PivotTable #1
5. Diagnostic PivotTable #2 OR Operational Dashboard - ONE chart

---

## Slide Deck Requirements (Minimum 15 slides)

### Critical Rule: Excel vs. Slides
- **Excel workbook**: Technical analysis ONLY (calculations, tables, charts, dashboards)
  - **NO interpretation text in Excel** - no text boxes or cells explaining patterns
- **Slide deck**: THE ONLY place for ALL insights, interpretations, and business implications

### Slide Structure

**Slide 1: Project Overview**
- Job description and company
- Why I selected this job (2 bullets)
- Stakeholder (name/title)
- Problem statement in required format

**Slide 2: Operations Management Decision Area**
- Decision Area Name (bold)
- 2-3 sentence justification explaining alignment with job

**Slide 3: Dataset Overview**
- **Takeaway title** (not "Dataset Overview" - state the value)
- Visual: Table with data source, time period, records, key variables, granularity
- Two bullets: Relevance (connection to job/problem), Scope (what can be analyzed)

**Slide 4: Data Quality Improvements**
- **Takeaway title** (state impact, not "Data Quality")
- Visual: Table of top 3 issues (Column Name | Issue Type | Records Affected | Decision)
- Two bullets: Impact (how cleaning improves reliability), Confidence (why stakeholder can trust insights)

**Slide 5: Primary Metric Definition**
- **Takeaway title** (why this metric matters)
- Visual: Metric name and definition (title card style)
- Two bullets: Why it matters (connection to problem), Decision support (how measuring helps)

**Slides 6-7: Descriptive Statistics (IRPM Required)**

**Slide 6: Central Tendency Insight**
- **Takeaway title** = THE INSIGHT (not "Central Tendency Analysis")
- Visual: Selected measure in large font OR statistics table screenshot
- Two bullets: **Recommendation** (action for stakeholder), **Prediction** (expected outcome)

**Slide 7: Variability Insight**
- **Takeaway title** = THE INSIGHT (not "Variability Analysis")
- Visual: Variability measure in large font OR histogram/stats screenshot
- Two bullets: **Recommendation** (action for stakeholder), **Prediction** (expected outcome)

**Slides 8-9: Diagnostic PivotTables (IRPM Required)**

**Slide 8: Diagnostic Pivot Table #1 Insight**
- **Takeaway title** = ROOT CAUSE INSIGHT
- Visual: Screenshot of ONE specific chart from Pivot Table #1
- Two bullets: **Recommendation** (action for root cause), **Prediction** (expected improvement)

**Slide 9: Diagnostic Pivot Table #2 Insight**
- **Takeaway title** = ROOT CAUSE INSIGHT
- Visual: Screenshot of ONE specific chart from Pivot Table #2
- Two bullets: **Recommendation** (action for root cause), **Prediction** (expected improvement)

**Slides 10-12: Strategic Dashboard (IRPM Required for ONE chart)**

**Slide 10: Strategic Dashboard - Scorecard Insight**
- **Takeaway title** = THE INSIGHT
- Visual: Screenshot of ONE scorecard
- Two bullets: **Recommendation**, **Prediction**

**Slide 11: Strategic Dashboard - Trend Insight**
- **Takeaway title** = THE INSIGHT
- Visual: Screenshot of ONE line chart
- Two bullets: **Recommendation**, **Prediction**

**Slide 12: Strategic Dashboard - Breakdown Insight**
- **Takeaway title** = THE INSIGHT
- Visual: Screenshot of ONE bar/column chart
- Two bullets: **Recommendation**, **Prediction**

**Slides 13-15: Operational Dashboard (IRPM Required for ONE chart)**

**Slide 13: Operational Dashboard - Scorecard Insight**
- **Takeaway title** = DIAGNOSTIC INSIGHT
- Visual: Screenshot of ONE scorecard
- Two bullets: **Recommendation**, **Prediction**

**Slide 14: Operational Dashboard - Trend Insight**
- **Takeaway title** = DIAGNOSTIC INSIGHT
- Visual: Screenshot of ONE line chart
- Two bullets: **Recommendation**, **Prediction**

**Slide 15: Operational Dashboard - Root Cause Breakdown Insight**
- **Takeaway title** = ROOT CAUSE INSIGHT
- Visual: Screenshot of ONE bar/column chart
- Two bullets: **Recommendation**, **Prediction**

### Key Slide Requirements:
- **Slide Title = The Insight**: State finding, not visual type
- **ONE visual per slide**: No full dashboard screenshots - select specific chart
- **Two bullets below visual**: (1) Recommendation, (2) Prediction
- **Excel contains NO interpretations**: Slides are THE ONLY place for insights

---

## Interview Format

**Duration:** 15 minutes + 5-minute debrief
**Location:** In person, Hilton 114

**Structure:**
1. "Tell me about yourself" (1 minute)
   - Education, extracurriculars, work history, personal tidbit
   - **SEAMLESS SEGUE into project** (critical!)

2. Foundation (3-4 minutes)
   - Job Description, Decision Area, Stakeholder, Problem Statement
   - Dataset Overview, Data Quality, Primary Metric
   - **Must draw whiteboard roadmap**

3. Descriptive Analytics (3-4 minutes)
   - Central Tendency + Variability with IRPM
   - Strategic Dashboard (choose ONE chart to discuss in depth)

4. Diagnostic Analytics (3-4 minutes)
   - PivotTable 1 + PivotTable 2 with IRPM
   - Operational Dashboard (choose ONE chart to discuss in depth)

5. Follow-up Questions (2-3 minutes)
   - "Why?" drilling
   - Challenges and decisions
   - Business implications

**Whiteboard Requirement:**
Students must draw the project roadmap:
```
[Job] → [Decision Area] → [Stakeholder] → [Problem]
                                              ↓
                                    [Solution Overview]
                                              ↓
                      [Dataset] → [Data Quality] → [Metric]
                                              ↓
            ┌────────────────────┴────────────────────┐
            ↓                                         ↓
   [DESCRIPTIVE ANALYTICS]              [DIAGNOSTIC ANALYTICS]
            ↓                                         ↓
  Central Tendency + Variability           PivotTable 1 + 2
            ↓                                         ↓
   Strategic Dashboard (1 chart)      Operational Dashboard (1 chart)
```

---

## Interview Assessment Rubric

**Total:** 100 points (= 15% of final course grade)

### 1. Depth of Understanding (40 points)
- Can explain WHY analytical choices were made
- Understands what numbers mean
- Can defend methodology
- **Grade A:** Clear mastery, ready to lead without hand-holding
- **Grade B:** Meets core requirements, minor gaps
- **Grade C:** Satisfies basics, uneven skills, needs mentoring
- **Grade D/F:** Significant shortcomings, substantial improvements needed

### 2. Business Acumen (30 points)
- Connects analysis to business problems
- Realistic and actionable recommendations
- Understands stakeholder's perspective

### 3. Communication Skills (20 points)
- Explains technical concepts clearly
- Structures responses logically
- Adapts to follow-up questions

### 4. Synthesis & Progression (10 points)
- Insights build on each other
- Can articulate analytics maturity journey (Foundation → Descriptive → Diagnostic)

**Interview Question:**
"Can I trust you to confidently lead stakeholders through a meeting on a project like the one you've just described?"

---

## Common Mistakes to Avoid

**❌ Content Mistakes:**
- Skipping Dataset Overview or Data Quality sections
- Discussing all 3 dashboard charts instead of choosing ONE
- Forgetting to connect analysis back to job description
- Presenting data without IRPM framework

**❌ Communication Mistakes:**
- Using technical jargon without explaining it
- Rambling without structure (use IRPM!)
- Not making eye contact or facing the whiteboard
- Forgetting the segue from "Tell me about yourself" to project

**❌ Timing Mistakes:**
- Spending 5 minutes on Foundation, leaving 2 minutes for all analysis
- Trying to discuss all 3 dashboard insights (choose ONE!)
- Not practicing with a timer beforehand

**❌ IRPM Mistakes:**
- Stating only Insight and Method, forgetting Recommendation and Prediction
- Vague Predictions ("things will improve" instead of "delivery time will decrease 20%")
- Generic Recommendations ("investigate the issue" instead of "hire 2 warehouse staff in East Region")
- Incomplete Method ("I used Excel" instead of "I used Excel's Descriptive Statistics tool on 1,247 orders to calculate mean, median, std dev...")

---

**Source References:**
- Study Guide: Complete midterm interview study guide document
- Project Requirements: Milestone 1 section (lines 565-937)
- IRPM Framework: Lines 85-101 in Study Guide
- Rubric: Lines 15-30 in Study Guide
