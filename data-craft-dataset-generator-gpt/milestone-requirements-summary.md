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
  - **Workbook 1**: `milestone-02-time-series-fname-lname.xlsx` with worksheets:
    - Raw (time series dataset)
    - Data_Dictionary (field definitions)
    - Time_Series_Forecasting (empty - for student's analysis work)
  - **Workbook 2**: `milestone-02-regression-fname-lname.xlsx` with worksheets:
    - Raw (regression dataset)
    - Data_Dictionary (field definitions)
    - Regression_Analysis (empty - for student's analysis work)
- NO Data_Cleaning_Log (data is clean)
- Slide deck (11 slides - SEPARATE deck, not attached to Milestone 01)

### Data Generation Guidance

**For Time Series Dataset**:
- Sequential dates with NO GAPS, 18-24 months recommended
- **Internally generate data with trend AND seasonal patterns** (NEVER mention "trend", "seasonal", "increasing", "cyclical" to students - let them discover through decomposition)
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
- **NO multicollinearity between IVs** - independent variables should be independent (r < 0.3 between IVs)
- Target adjusted R² of 0.65-0.80 for best model
- Clean data ready for regression (no missing values, no duplicates)

---

## Milestone 3: Prescriptive Analytics

**Due**: Thursday, December 4, 2025
**Analytics Types**: TWO Prescriptive Problems Required

### What Students Need

**Dataset Requirements**:
- Students must complete **TWO separate prescriptive analytics problems**
- **Problem A**: Linear Programming (Required) - Excel Solver
- **Problem B**: Choose ONE method from:
  - Inventory Management (Economic Order Quantity)
  - Aggregate Planning
  - Location Strategy (Factor Rating Method)
  - Capacity & Constraint Management

**Technical Analysis Required**:

1. **Problem A - Linear Programming** (Required):
   - Decision variables (clearly labeled)
   - Objective function (maximize or minimize)
   - Objective coefficients (contribution of each decision variable)
   - Constraints (limitations on the problem)
   - Excel Solver solution (Simplex LP method)
   - Sensitivity analysis interpretation:
     - Shadow prices
     - Binding vs. non-binding constraints
     - Allowable increases/decreases

2. **Problem B - Choose ONE Method**:
   - **Inventory Management**: EOQ calculation, reorder points, total cost analysis
   - **Aggregate Planning**: Capacity planning, workforce/production adjustments, cost optimization
   - **Location Strategy**: Factor rating method, weighted scores, site comparison
   - **Capacity & Constraint Management**: Bottleneck identification, throughput analysis, constraint optimization

**Deliverables**:
- Excel workbook with both Problem A and Problem B analyses
- Data cleaning log (if using new dataset - NOT required if data is clean)
- COMPLETE slide deck (all 3 milestones - exactly 10 slides for Milestone 3)

### Data Generation Guidance

**IMPORTANT**: Milestone 3 requires **parameter data**, not transactional data like previous milestones.

**For Problem A - Linear Programming**:

Generate data in **BOTH formats** to give students flexibility:

**Option 1: Pre-Formatted Excel Tables** (Ready for Solver)
- Decision variables table with clear labels
- Objective coefficients for each decision variable
- Constraints table with:
  - Resource usage coefficients (how much each decision variable consumes)
  - Constraint limits (budget, capacity, minimum/maximum requirements)
  - Constraint types (≤, ≥, or =)
- All sections clearly labeled and organized
- Ready to reference in Excel Solver setup

**Option 2: Raw Parameter Data** (Students organize themselves)
- List of decision variable options with relevant parameters
- Cost/profit/contribution data for objective function
- Resource consumption rates
- Constraint limit values
- Students structure the model themselves

**Key LP Data Characteristics**:
- 3-7 decision variables (manageable complexity)
- 4-8 constraints (realistic problem scope)
- **MUST be a LINEAR problem** solvable with Simplex LP method:
  - Linear objective function (no exponents, no products of decision variables)
  - Linear constraints only (no nonlinear relationships)
  - All coefficients must be constants, not variables
- Ensure feasible solution exists (test before providing)
- Create interesting optimal solution (not obvious, requires Solver)
- Include at least 2-3 binding constraints for sensitivity analysis
- Provide realistic business context (production, resource allocation, etc.)

**For Problem B - Student-Selected Method**:

**Approach**: Generate data for the **specific method the student requests** after asking which Problem B method they want to analyze.

**Inventory Management Data**:
- Annual demand (units/year)
- Ordering cost per order ($)
- Holding cost per unit per year ($)
- Lead time (days)
- Unit cost
- Optional: Quantity discount breakpoints

**Aggregate Planning Data**:
- Demand forecast by period (6-12 periods)
- Regular time capacity and cost
- Overtime capacity and cost
- Subcontracting cost
- Inventory holding cost
- Backorder/stockout cost
- Hiring/firing costs
- Current workforce level

**Location Strategy Data**:
- 3-5 location alternatives
- 5-8 factors (cost, labor availability, proximity to markets, infrastructure, etc.)
- Factor weights (importance ratings)
- Location scores for each factor (0-100 scale)
- Optional: Qualitative descriptions of each location

**Capacity & Constraint Management Data**:
- Process step capacities (units/hour or units/day)
- Processing times for each step
- Demand requirement
- Resource availability
- Setup times (if applicable)
- Optional: Cost data for constraint analysis

**Data Format Options**:
- Provide both **pre-formatted tables** AND **raw parameter lists**
- Pre-formatted: Ready to use in Excel calculations
- Raw: Students organize and structure themselves
- Include clear labels and units for all parameters

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
- For time series: Emphasize NO GAPS, 18-24 months; internally ensure patterns exist but NEVER mention "trend", "seasonal", "increasing", or "cyclical" to students
- For regression: 4-6 independent variables, support testing 3+ models
- Data must be CLEAN (no quality issues) - focus is on predictive modeling
- Separate problems: Problem A (time series forecast) and Problem B (regression prediction)

**For Milestone 3**:
- Students need TWO prescriptive problems: Problem A (LP) + Problem B (student choice)
- **Problem A - Linear Programming**: Always required, provide BOTH pre-formatted and raw parameter options
  - Ask about: Decision variables, objective (max/min), constraints, business context
  - Ensure feasible solution exists with interesting optimal solution
  - Include 2-3 binding constraints for sensitivity analysis
- **Problem B - Student Choice**: Ask which method they want (Inventory/Aggregate/Location/Capacity)
  - Generate data specific to their chosen method
  - Provide both pre-formatted tables and raw parameter lists
  - Include all parameters needed for complete analysis
- Parameter data focus (not transactional data like Milestones 1-2)

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
- [ ] Time series: 18-24 months, NO GAPS, patterns generated internally (NEVER mention pattern types to students)
- [ ] Regression: 4-6 independent variables, supports testing 3+ models

**Milestone 3 Specific**:
- [ ] TWO problems being generated: Problem A (LP required) + Problem B (student choice)
- [ ] Problem A: Both pre-formatted AND raw parameter options provided
- [ ] Problem A: LP model is feasible with interesting optimal solution
- [ ] Problem A: 2-3 binding constraints included for sensitivity analysis
- [ ] Problem B: Student has specified which method (Inventory/Aggregate/Location/Capacity)
- [ ] Problem B: Complete parameters for chosen method with both format options
- [ ] All parameters clearly labeled with units and business context
