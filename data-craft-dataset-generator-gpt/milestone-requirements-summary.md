# Milestone Requirements Summary

## Milestone 1: Descriptive & Diagnostic Analytics

**Due**: Monday, October 20, 2025
**Analytics Types**: Descriptive (What happened?) + Diagnostic (Why did it happen?)

### What Students Need

**Dataset Requirements**:
- **MUST use the SAME dataset** for both Descriptive and Diagnostic
- Minimum 500 rows, 5+ variables
- Time-stamped data (6-12 months recommended)
- Numeric metrics for summary statistics
- Categorical dimensions (2-3) for drill-down analysis
- Intentional data quality issues for learning

**Technical Analysis Required**:
1. **Descriptive Statistics**:
   - Central tendency (mean, median, mode)
   - Variability (standard deviation, range, coefficient of variation)
   - Distributions and trends

2. **Diagnostic Analysis**:
   - Minimum 2 pivot tables
   - Root cause analysis using categorical dimensions
   - Slicers for interactive filtering
   - Conditional formatting

3. **Dashboards** (2 required):
   - Strategic Dashboard (Executive view)
   - Operational Dashboard (Detailed view)
   - Can use Excel OR external tools (Tableau, Power BI, Looker Studio)

**Deliverables**:
- Excel workbook with analysis
- Data dictionary
- Data cleaning log (Data Quality Framework applied)
- Slide deck (13+ slides with takeaway titles)
- Dashboard links (if using external tools)

### Data Generation Guidance

**Focus on**:
- Rich categorical dimensions for pivot table analysis
- Clear patterns across categories (for root cause discovery)
- Realistic trends over time
- Sufficient records per category (30+ for validity)

**Quality Issues to Include**:
- 2-5% missing values
- 1-3% duplicates
- Date format inconsistencies
- Outliers in 2-3% of records
- Inconsistent category names

---

## Milestone 2: Predictive Analytics

**Due**: Tuesday, November 11, 2025
**Analytics Types**: Time Series Forecasting + Multiple Linear Regression

### What Students Need

**Dataset Requirements**:
- **GENERATE TWO SEPARATE DATASETS** (not one unified dataset)
- **Dataset 1**: Time Series Forecasting data
- **Dataset 2**: Regression Analysis data
- **Data Quality**: CLEAN data only - NO data quality issues, NO Data_Cleaning_Log required
- Different from Milestone 1 (new problem, new data focused on predictive analytics)

**Technical Analysis Required**:

1. **Time Series Forecasting** (minimum 3 models tested):
   - N-Period Moving Average
   - N-Period Weighted Moving Average
   - Excel's FORECAST.LINEAR
   - Excel's FORECAST.ETS
   - Compare forecast accuracy (MAD, MSE, and/or MAPE)
   - Select BEST method and justify
   - Generate forecast for next period

2. **Multiple Linear Regression** (minimum 3 models tested):
   - Each model must have at least 2 independent variables
   - Test different variable combinations
   - Dependent variable (what they're predicting)
   - Independent variables (4-6 total for flexibility)
   - Excel Data Analysis Toolpak
   - Interpret: Adjusted R², coefficients, p-values, significance
   - Make predictions for 2-3 scenarios

**Deliverables**:
- TWO separate Excel workbooks:
  - `milestone-02-time-series-fname-lname.xlsx`
  - `milestone-02-regression-fname-lname.xlsx`
- Data dictionary for each dataset
- NO Data_Cleaning_Log (data is clean)
- Slide deck (11 slides - SEPARATE deck, not attached to Milestone 01)

### Data Generation Guidance

**For Time Series Dataset**:
- Sequential dates with NO GAPS, 18-24 months recommended
- **MUST include both trend AND seasonal patterns** (don't reveal patterns to student)
- Monthly frequency preferred
- Target variable to forecast (realistic scale)
- Optional: 1-2 context fields for reference
- Clean data ready for forecasting (no missing values, no duplicates)

**For Regression Dataset**:
- 500-1000 records (750 recommended)
- **4-6 independent variables** (allows testing multiple model combinations)
- **ALL variables must be NUMERIC/CONTINUOUS** - NO categorical variables (students have not learned dummy variables)
- Examples: distance, weight, time, cost, quantity, temperature, price, volume, speed, rating
- Realistic correlations (r = 0.3 to 0.7 between IVs and DV)
- Some multicollinearity between IVs (r = 0.3-0.6, realistic)
- Target adjusted R² of 0.65-0.80 for best model
- Clean data ready for regression (no missing values, no duplicates)

---

## Milestone 3: Prescriptive Analytics

**Due**: Thursday, December 4, 2025
**Analytics Types**: Linear Programming (Optimization) + Monte Carlo Simulation

### What Students Need

**Dataset Requirements**:
- Can use SAME dataset as previous milestones OR a different dataset
- Must complete BOTH analyses (or justify why only one applies):
  - **Optimization**: Parameters for Excel Solver
  - **Simulation**: Historical variability data

**Technical Analysis Required**:

1. **Linear Programming with Excel Solver**:
   - Decision variables (3-10)
   - Objective function (maximize/minimize what?)
   - Constraints (4-8 limitations)
   - Solver solution
   - Sensitivity analysis

2. **Monte Carlo Simulation**:
   - Uncertain variable(s)
   - Probability distribution (normal, uniform, or triangular)
   - 1,000-10,000 simulation runs
   - Distribution of outcomes
   - Risk assessment and confidence intervals

**Deliverables**:
- Excel workbook with optimization and simulation models
- Data cleaning log (if using new dataset)
- COMPLETE slide deck (all 3 milestones)

### Data Generation Guidance

**For Optimization**:
- Decision variables table (product/resource options with costs/profits)
- Constraints table (budget, capacity, minimum/maximum limits)
- Resource usage matrix
- Ensure feasible solution exists
- Make optimal solution interesting (not trivial)

**For Simulation**:
- Historical data showing variability (250-500 records)
- Clear probability distribution pattern
- Distribution parameters (mean, std dev, min, max)
- Uncertain variables that impact decisions
- Realistic uncertainty ranges

---

## Cross-Milestone Considerations

### Dataset Flexibility

**Option 1: Same Dataset Throughout** (Recommended if possible)
- Simplifies project coherence
- Shows analytics maturity progression on same problem
- Reduces data collection effort

**Option 2: Different Datasets by Milestone**
- Acceptable if original dataset doesn't support all analytics types
- Each new dataset requires Data Cleaning Log
- Must maintain connection to same stakeholder/problem/decision area

### Common Requirements Across All Milestones

**Connection to**:
- Specific job description and company
- Identified stakeholder (role, LinkedIn profile)
- Problem statement (consistent format)
- Operations Management Decision Area (same throughout)

**Data Quality**:
- All datasets must include intentional quality issues
- Data Quality Framework must be applied
- Data Cleaning Log required for each new dataset

**Communication**:
- Cumulative slide deck (grows with each milestone)
- Takeaway titles (insight, not description)
- ONE visual per slide with Recommendation/Prediction bullets
- Professional formatting and design

**Frameworks**:
- DC ACT Framework (Define → Collect → Analyze → Communicate → Act)
- Data Quality Framework (Identify → Assess → Analyze → Decide → Fix)
- Connection to Operations Management Decision Area

---

## Student Interview Preparation

### Midterm Interview (Milestone 1)
**When**: Week of October 20-22, 2025
**Coverage**: Data quality, descriptive analytics, diagnostic analytics

**Be Ready to Explain**:
- Why you chose your problem and decision area
- Data quality issues found and how you addressed them
- Key descriptive findings (trends, patterns)
- Root causes identified through diagnostic analysis
- Connection to stakeholder's problem

### Final Interview (Milestones 2-3)
**When**: Finals week, December 2025
**Coverage**: Predictive analytics, prescriptive analytics, synthesis

**Be Ready to Explain**:
- Why your forecasting method worked best
- What regression relationships revealed
- Your optimization model and constraints
- Simulation results and risk assessment
- How all analytics types connect to inform decisions
- If stakeholder could only implement ONE recommendation, which and why?

---

## Tips for Data Craft GPT Usage

### When Students Ask for Help

**For Milestone 1**:
- Guide them to descriptive/diagnostic scenario
- Ask about time period (6-12 months)
- Focus on categorical dimensions for drill-down
- Ensure rich enough data for pivot table analysis

**For Milestone 2**:
- Students need BOTH time series and regression - generate TWO SEPARATE datasets
- For time series: Emphasize NO GAPS, 18-24 months, MUST have trend + seasonal (don't reveal)
- For regression: 4-6 independent variables, support testing 3+ models
- Data must be CLEAN (no quality issues) - focus is on predictive modeling
- Separate problems: Problem A (time series forecast) and Problem B (regression prediction)

**For Milestone 3**:
- Ask: Optimization, simulation, or both?
- For optimization: Decision variables, constraints, objective
- For simulation: Uncertain variables, distribution type, parameters
- Can be different dataset if needed

### Quality Checks Before Generation

**All Milestones**:
- [ ] Problem connects clearly to Operations Management Decision Area
- [ ] Stakeholder is specific (role, company, ideally LinkedIn profile)
- [ ] Dataset structure matches analytics type requirements
- [ ] README will connect to DC ACT Framework and Decision Area
- [ ] Student understands what milestone they're working on

**Milestone 1 Specific**:
- [ ] Intentional quality issues planned (ALL 5 types: missing values, duplicates, date inconsistencies, outliers, inconsistent categories)
- [ ] Rich categorical dimensions for pivot table drill-down

**Milestone 2 Specific**:
- [ ] TWO separate datasets being generated (time series + regression)
- [ ] NO quality issues (clean data only)
- [ ] Time series: 18-24 months, NO GAPS, has trend + seasonal patterns (don't reveal)
- [ ] Regression: 4-6 independent variables, supports testing 3+ models

**Milestone 3 Specific**:
- [ ] Optimization OR simulation requirements clear
- [ ] Parameters/constraints/distributions appropriate
