# Analytics Type Specifications

## Descriptive & Diagnostic Analytics (Milestone 1)

### Purpose
- **Descriptive**: What happened? (Summary statistics, trends, patterns)
- **Diagnostic**: Why did it happen? (Root cause analysis)

### Data Structure Requirements

**Essential Fields**:
- Date/timestamp field (for trend analysis)
- Primary metric (numeric) - the key performance indicator
- 2-3 categorical dimensions (for grouping and comparison)
- Additional supporting metrics (3-5 numeric fields)

**Time Characteristics**:
- Minimum 6 months of data (preferably 12+ months)
- Daily, weekly, or monthly granularity
- Sequential dates with realistic patterns (trends, seasonality if applicable)

**Categorical Dimensions** (include 2-3):
- Geographic (region, warehouse location, distribution center)
- Product-related (category, SKU group, product line)
- Time-based (day of week, shift, season)
- Process-related (machine, line, carrier, supplier)
- People-related (team, shift supervisor)

### Key Questions to Ask

1. **Operational Scenario**: "Which scenario best fits your problem? [Suggest 2-3 based on decision area] or describe your own?"
2. **Time Period**: "What time period should the data cover and at what granularity (daily/weekly/monthly)?"
3. **Key Metrics**: "What metrics do you need to analyze? [Suggest 8-12 based on decision area]"
4. **Dimensions for Root Cause**: "What dimensions do you need to drill down by? (e.g., region, product category, shift)"

**Then INFORM (don't ask)**: "Your dataset will include all standard data quality issues for comprehensive learning practice: 2-5% missing values, 1-3% duplicates, mixed date formats, 2-3% outliers, and inconsistent category variations."

### Data Generation Guidelines

- Include realistic trends (gradual increase/decrease)
- Add seasonal patterns if time period > 1 year
- Create variations across categorical dimensions (for root cause discovery)
- Ensure sufficient records per category (minimum 30 for statistical validity)

---

## Predictive Analytics - Time Series Forecasting (Milestone 2A)

### Purpose
Forecast future values of a metric based on historical time patterns.

### Data Structure Requirements

**Essential Fields**:
- Date field (sequential, NO GAPS)
- Target variable (what they're forecasting)
- Optional: 1-2 context fields (for reference, not forecasting)

**Time Characteristics**:
- **Minimum**: 18 months of historical data (recommended 24 months)
- **Frequency**: Monthly preferred (daily or weekly also acceptable)
- **Pattern**: MUST include both trend AND seasonal components
- **Data Quality**: CLEAN data only - no missing values, no duplicates, no format issues

### Key Questions to Ask

1. **Forecasting Target**: "What do you want to forecast? (e.g., monthly demand, weekly orders, monthly revenue)"
2. **Time Horizon**: "How far ahead do you need to forecast? (next month, next quarter)"
3. **Data Period**: "How many months of historical data do you need? (18-24 months recommended)"
4. **Business Context**: "What's the business scenario? (e.g., seasonal product demand, service call volume)"

**DO NOT ask about patterns** - Students must discover patterns through decomposition analysis.

### Data Generation Guidelines

**IMPORTANT**: Generate data with BOTH trend and seasonal patterns, but DO NOT tell the student what patterns exist. They must decompose and identify patterns themselves (Milestone 02 Slide 3 requirement).

**Required Pattern Components**:
- **Trend**: Clear linear increase or decrease over time (not too steep - realistic business growth/decline)
- **Seasonality**: Repeating patterns aligned with frequency (monthly = 12-month cycle, quarterly = 4-quarter cycle)
- **Noise**: Random variation (±5-10% of mean value)

**For Excel FORECAST.LINEAR and FORECAST.ETS Methods**:
- Generate sequential dates with NO GAPS
- Ensure trend is detectable but not overwhelming
- Make seasonal patterns realistic (e.g., retail holiday spikes, summer/winter variations)
- Add enough noise to make forecasting interesting but not impossible
- Target variable should have realistic scale for business context

**Pattern Obfuscation**:
- Generate data, but in README/data dictionary, describe only the metric (e.g., "Monthly sales in units")
- DO NOT mention: "trend", "seasonal", "increasing", "cyclical" in any documentation
- Let students discover patterns through their own analysis

**Delivery Format**:
- Excel workbook: `milestone-02-time-series-fname-lname.xlsx`
- Worksheets:
  - **Raw**: Time series dataset (clean data)
  - **Data_Dictionary**: Field definitions
  - **Time_Series_Forecasting**: Empty worksheet for student's analysis

---

## Predictive Analytics - Regression Analysis (Milestone 2B)

### Purpose
Predict a dependent variable based on relationships with independent variables using multiple linear regression.

### Data Structure Requirements

**Sample Size**: 500-1000 records (750 recommended)

**Required Fields**:
- Record ID
- Dependent variable (what they're predicting)
- **4-6 independent variables** (to support testing minimum 3 different models)

**Variable Mix**:
- **ALL 4-6 independent variables must be NUMERIC/CONTINUOUS** (distance, weight, time, cost, quantity, temperature, etc.)
- **NO categorical variables** (students have not learned dummy variable creation)
- Realistic correlations (not perfect, not random)
- **Data Quality**: CLEAN data only - no missing values, no duplicates, no format issues

### Key Questions to Ask

1. **Dependent Variable**: "What are you trying to predict? (e.g., delivery time, order cost, defect rate, satisfaction score)"
2. **Independent Variables**: "What numeric factors might influence this? I recommend 4-6 variables so you can test different model combinations. All variables must be numeric (like distance, weight, time, cost, quantity, temperature)."
3. **Business Context**: "What's the business scenario?"

### Data Generation Guidelines

**Multiple Regression Model Support**:
- Generate 4-6 independent variables total
- Each variable should have some predictive value (varying strengths)
- Students will test minimum 3 different models (each with 2+ variables)
- Ensure different variable combinations produce different R² values

**Correlation Structure**:
- Create realistic relationships between IVs and DV (r = 0.3 to 0.7)
- **NO multicollinearity between IVs** - independent variables should be independent of each other (r < 0.3 between IVs)
- Target adjusted R² of 0.65-0.80 for best model

**Variable Design**:
- **ALL variables must be NUMERIC/CONTINUOUS**: distance, weight, time, cost, quantity, temperature, experience, age, price, volume, speed, rating, hours, days, percentage, count
- **NO categorical variables allowed**: Do not include yes/no flags, binary (0/1), or category labels
- **Significant variables**: 3-4 should have p < 0.05 in best model
- **Weaker variables**: 1-2 can be less significant (but still numeric)

**Realistic Business Relationships**:
- Coefficients should make business sense
- Scale variables appropriately
- Add realistic noise to prevent perfect predictions

**Delivery Format**:
- Excel workbook: `milestone-02-regression-fname-lname.xlsx`
- Worksheets:
  - **Raw**: Regression dataset (clean data, 500-1000 records)
  - **Data_Dictionary**: Field definitions
  - **Regression_Analysis**: Empty worksheet for student's analysis

---

## Prescriptive Analytics - Linear Programming (Milestone 3A)

### Purpose
Find optimal solution (maximize profit, minimize cost) given constraints.

### Data Structure Requirements

**Decision Variables** (3-10 recommended):
- What the stakeholder is deciding (product quantities, resource allocations)
- Each with cost/profit coefficient

**Constraints** (4-8 recommended):
- Budget limits
- Capacity constraints
- Time restrictions
- Minimum/maximum requirements

### Key Questions to Ask

1. **Optimization Problem Type**: "What type of optimization? [Suggest 2-3 based on decision area] or describe yours?"
2. **Objective Function**: "What are you trying to maximize or minimize? (profit, cost, throughput, etc.)"
3. **Decision Variables**: "What are you deciding? (How many units to produce? How to allocate resources?)"
4. **Constraints**: "What are the limiting factors? (budget, capacity, time, minimum service levels)"

### Data Generation Guidelines

**Create Three Files**:

1. **Decision Variables Table**:
   - Variable ID, name, unit profit/cost, resource consumption per unit

2. **Constraints Table**:
   - Constraint name, type (<=, >=, =), limit value, unit

3. **Resource Usage Matrix**:
   - How much of each resource each decision variable consumes

**Ensure**:
- Feasible solution exists (constraints not impossible)
- Optimal solution is interesting (not trivial)
- Sensitivity analysis will be meaningful

---

## Prescriptive Analytics - Monte Carlo Simulation (Milestone 3B)

### Purpose
Model uncertainty and assess risk through probabilistic simulation.

### Data Structure Requirements

**Historical Variability Data**: 250-500 records showing past variation

**Required Elements**:
- Uncertain variable(s) with clear variability
- Probability distribution parameters (mean, std dev, min, max)
- Output metric that depends on uncertain inputs

### Key Questions to Ask

1. **Simulation Scenario**: "What uncertainty do you want to model? [Suggest 2-3 based on decision area]"
2. **Uncertain Variables**: "What variables are uncertain? (demand, lead time, defect rate, costs)"
3. **Probability Distribution**: "What distribution fits best?"
   - Normal: Mean and standard deviation?
   - Uniform: Minimum and maximum?
   - Triangular: Min, most likely, max?
4. **Simulation Size**: "How many scenarios to simulate? (typically 1,000-10,000)"

### Data Generation Guidelines

**Historical Data**:
- Show realistic variability in uncertain variable
- Data should clearly fit a distribution (normal, uniform, or triangular)
- Include enough records to estimate parameters

**Distribution Parameters**:
- Calculate and provide: mean, standard deviation, min, max
- Show data can be modeled with chosen distribution
- Ensure simulation will produce meaningful risk assessment

---

## General Data Quality Standards (All Types)

### Intentional Quality Issues - ALWAYS Include ALL 5 Types

**IMPORTANT**: Students do NOT choose which issues to include. ALL datasets MUST contain ALL 5 quality issue types below for comprehensive learning practice.

**1. Missing Values** (2-5% of cells - REQUIRED):
- Random distribution across fields
- More in optional fields, less in critical fields

**2. Duplicate Records** (1-3% - REQUIRED):
- Exact duplicates AND near-duplicates (slight variations)

**3. Date Format Inconsistencies** (REQUIRED):
- Mix 70% YYYY-MM-DD and 30% MM/DD/YYYY

**4. Outliers** (2-3% of numeric fields - REQUIRED):
- Realistic outliers (not impossible values)
- Should trigger student investigation

**5. Inconsistent Categories** (REQUIRED):
- Variations like "Northeast", "North East", "NE"
- Case inconsistencies: "Warehouse A" vs "warehouse a"

**Validation Before Delivery**: Confirm dataset includes ALL 5 quality issue types.

### Data Dictionary Requirements

**Required Columns**:
- Column Name
- Data Type (Text, Number, Date, Boolean)
- Notes/Description

**Notes Should Include**:
- Valid value ranges
- Format specifications
- Business rules
- Categories or codes
- Special handling notes

---

## Milestone-Specific Guidance

### Milestone 1: Descriptive/Diagnostic
- Must use SAME dataset for both
- Focus on historical analysis (what/why)
- Need rich categorical dimensions for drill-down
- Time period: 6-12 months minimum
- **Data Quality**: Include ALL 5 intentional quality issues (required for learning)

### Milestone 2: Predictive
- **GENERATE TWO SEPARATE DATASETS** (one for time series, one for regression)
- **Data Quality**: CLEAN data only - NO quality issues for Milestone 2
- **Time Series Dataset**:
  - Sequential dates, NO GAPS, 18-24 months
  - MUST have both trend AND seasonal patterns (don't tell student)
  - Clean data ready for forecasting
- **Regression Dataset**:
  - 500-1000 records with 4-6 independent variables
  - Clean data ready for multiple regression analysis
  - Support testing minimum 3 different models
- Focus on predictive modeling, not data cleaning

### Milestone 3: Prescriptive
- Can use same OR different dataset from previous milestones
- Optimization: Need parameters, constraints, objective
- Simulation: Need historical variability data
- Focus on decision-making under constraints/uncertainty
- **Data Quality**: Include intentional quality issues (unless requested otherwise)
