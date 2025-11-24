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

## Prescriptive Analytics - Problem A: Linear Programming (Milestone 3 - REQUIRED)

### Purpose
Find optimal solution (maximize profit, minimize cost) using Excel Solver with linear programming.

### Data Structure Requirements

**CRITICAL: Must be a LINEAR problem solvable with Simplex LP method**

**Decision Variables** (3-7 recommended):
- What the stakeholder is deciding (product quantities, resource allocations)
- Each with objective coefficient (contribution to objective function)

**Constraints** (4-8 recommended):
- Budget limits
- Capacity constraints
- Resource availability
- Minimum/maximum requirements
- Must include 2-3 binding constraints for sensitivity analysis

**Linearity Requirements**:
- Linear objective function (no exponents like x², no products like x₁×x₂)
- Linear constraints only (no nonlinear relationships)
- All coefficients must be constants, not variables

### Key Questions to Ask

1. **Business Context**: "What business problem are you solving? (production planning, resource allocation, product mix, etc.)"
2. **Objective Function**: "What are you trying to maximize or minimize? (profit, cost, revenue, throughput, etc.)"
3. **Decision Variables**: "What are you deciding? (How many units to produce? How to allocate resources?)"
4. **Constraints**: "What are the limiting factors? (budget, machine hours, labor hours, materials, minimum requirements)"

### Data Generation Guidelines

**Generate data in BOTH formats:**

**Option 1: Pre-Formatted Excel Tables** (Ready for Solver)
Create four organized tables:

1. **Decision Variables Table**:
   - Columns: Variable Name, Description, Unit
   - Example: Product A, Product B, Product C

2. **Objective Coefficients Table**:
   - Columns: Variable, Objective Coefficient, Unit
   - Example: Product A = $50 profit/unit

3. **Constraints Table**:
   - Columns: Constraint Name, Type (≤, ≥, =), Limit, Unit
   - Example: Machine Hours, ≤, 2000, hours/month

4. **Resource Usage Matrix**:
   - Rows: Constraints, Columns: Decision Variables
   - Cell values: Usage coefficients (how much of constraint each variable consumes)
   - Example: Product A uses 2 machine hours/unit

**Option 2: Raw Parameter Data** (Students organize themselves)
Provide the same information as text/lists:
- List of decision variable options with descriptions
- Objective coefficients for each variable
- List of constraints with limits
- Resource consumption rates for each variable-constraint combination
- Let students structure the LP model themselves

**Quality Assurance**:
- **Test feasibility**: Ensure a feasible solution exists
- **Verify linearity**: All relationships must be linear (no x², no x₁×x₂)
- **Create interesting problem**: Optimal solution should NOT be obvious
- **Include binding constraints**: 2-3 constraints should be binding at optimum (for sensitivity analysis)
- **Realistic business context**: Coefficients and constraints should make business sense
- **Manageable complexity**: 3-7 decision variables, 4-8 constraints

---

## Prescriptive Analytics - Problem B: Inventory Management (Milestone 3 - STUDENT CHOICE)

### Purpose
Optimize inventory decisions using Economic Order Quantity (EOQ) model and reorder point calculations.

### Data Structure Requirements

**EOQ Parameters**:
- Annual demand (units/year)
- Ordering cost per order ($)
- Holding cost per unit per year ($ or % of unit cost)
- Unit cost ($)
- Lead time (days)
- Optional: Quantity discount breakpoints

### Key Questions to Ask

1. **Inventory Item**: "What are you managing inventory for? (raw materials, finished goods, spare parts)"
2. **Demand Pattern**: "What's the annual demand volume?"
3. **Cost Structure**: "What are the ordering costs and holding costs?"
4. **Service Requirements**: "What's the lead time for replenishment?"

### Data Generation Guidelines

**Generate data in BOTH formats:**

**Option 1: Pre-Formatted Excel Tables**
- Inventory Parameters Table with all EOQ inputs organized and labeled
- Optional: Demand variability data for safety stock calculation

**Option 2: Raw Parameter Data**
- Annual demand: realistic value (e.g., 5,000-50,000 units/year)
- Ordering cost: $50-$500 per order
- Holding cost: 20-30% of unit cost per year OR $1-$10 per unit per year
- Unit cost: realistic for item type
- Lead time: 5-30 days
- Optional: Demand standard deviation for safety stock

**Quality Assurance**:
- EOQ should result in reasonable order frequency (not too many, not too few orders per year)
- Total annual inventory cost should be realistic for business context
- If including quantity discounts, ensure breakpoints create interesting analysis

---

## Prescriptive Analytics - Problem B: Aggregate Planning (Milestone 3 - STUDENT CHOICE)

### Purpose
Develop a production plan that matches supply with demand over a planning horizon while minimizing costs.

### Data Structure Requirements

**Planning Parameters** (6-12 periods):
- Demand forecast by period
- Regular time production capacity (units)
- Regular time production cost ($/unit)
- Overtime capacity (units)
- Overtime cost ($/unit)
- Subcontracting cost ($/unit)
- Inventory holding cost ($/unit/period)
- Backorder/stockout cost ($/unit)
- Hiring cost ($/worker)
- Firing/layoff cost ($/worker)
- Current workforce level
- Units per worker per period

### Key Questions to Ask

1. **Planning Horizon**: "How many periods (months) should the plan cover? (6-12 recommended)"
2. **Demand Pattern**: "What's the demand pattern? (seasonal, growing, stable)"
3. **Production Options**: "What production flexibility exists? (overtime, subcontracting, inventory)"
4. **Workforce Changes**: "Can workforce size change? (hiring/firing allowed?)"

### Data Generation Guidelines

**Generate data in BOTH formats:**

**Option 1: Pre-Formatted Excel Tables**
- Demand Forecast Table (by period)
- Capacity & Cost Parameters Table
- Workforce Parameters Table
- All organized and ready for aggregate planning calculations

**Option 2: Raw Parameter Data**
- Period-by-period demand values
- Production capacity and cost parameters
- Workforce change costs
- Inventory and backorder costs
- Let students structure their own aggregate plan

**Quality Assurance**:
- Demand should show realistic pattern (seasonal peaks, growth, or stability)
- Costs should create trade-offs (regular vs overtime vs subcontracting)
- Planning problem should have multiple viable strategies
- Ensure feasible solutions exist (total capacity ≥ total demand over horizon)

---

## Prescriptive Analytics - Problem B: Location Strategy (Milestone 3 - STUDENT CHOICE)

### Purpose
Select optimal facility location using Factor Rating Method with weighted scoring.

### Data Structure Requirements

**Location Alternatives**: 3-5 site options

**Location Factors**: 5-8 factors to evaluate
- Cost-related (labor costs, facility costs, transportation)
- Operational (proximity to markets, supplier access, infrastructure)
- Strategic (skilled labor availability, quality of life, business climate)

**Scoring System**:
- Factor weights (importance ratings, must sum to 1.0 or 100)
- Location scores for each factor (0-100 scale)

### Key Questions to Ask

1. **Location Purpose**: "What type of facility? (warehouse, manufacturing plant, distribution center, retail store)"
2. **Location Options**: "How many location alternatives to compare? (3-5 recommended)"
3. **Critical Factors**: "What factors matter most? (costs, proximity, labor, infrastructure)"
4. **Stakeholder Priorities**: "How important is each factor relative to others?"

### Data Generation Guidelines

**Generate data in BOTH formats:**

**Option 1: Pre-Formatted Excel Tables**
- Location Alternatives Table (site names/cities)
- Factors Table with weights
- Scoring Matrix (locations × factors with scores)
- Organized for weighted score calculations

**Option 2: Raw Parameter Data**
- List of location alternatives with brief descriptions
- List of factors with assigned weights
- Factor scores for each location
- Let students organize Factor Rating analysis

**Quality Assurance**:
- Factor weights should sum to 1.0 (or 100)
- Scores should be on consistent 0-100 scale
- Create realistic trade-offs (no location dominates all factors)
- Winning location should be clear but not overwhelming
- Factors should align with Operations Management Decision Area

---

## Prescriptive Analytics - Problem B: Capacity & Constraint Management (Milestone 3 - STUDENT CHOICE)

### Purpose
Identify bottlenecks, calculate system capacity, and analyze constraint impacts using throughput analysis.

### Data Structure Requirements

**Process Steps**: 4-6 sequential or parallel process steps

**Capacity Data**:
- Processing time per unit at each step (minutes/unit or units/hour)
- Available time per step (hours/day or hours/week)
- Step capacity (units/hour or units/day)
- Demand requirement (units needed)

**Optional**:
- Setup times between batches
- Worker requirements per step
- Cost data for constraint analysis
- Quality/defect rates by step

### Key Questions to Ask

1. **Process Type**: "What process are you analyzing? (manufacturing line, service delivery, order fulfillment)"
2. **Process Steps**: "How many steps in the process? (4-6 recommended)"
3. **Constraint Concerns**: "What's the suspected bottleneck or capacity issue?"
4. **Demand Pressure**: "What's the demand requirement vs current capacity?"

### Data Generation Guidelines

**Generate data in BOTH formats:**

**Option 1: Pre-Formatted Excel Tables**
- Process Steps Table with capacities and processing times
- Demand Requirements Table
- Resource Availability Table
- Organized for bottleneck and throughput calculations

**Option 2: Raw Parameter Data**
- List of process steps with processing times
- Available time for each step
- Demand requirements
- Let students organize capacity analysis

**Quality Assurance**:
- Create clear bottleneck (one step with lowest capacity)
- System capacity should be less than demand (creates constraint management problem)
- Make constraint analysis meaningful (bottleneck should significantly limit throughput)
- Include realistic business context (manufacturing, service, or operational process)
- Provide enough data for students to calculate:
  - Capacity at each step
  - System bottleneck
  - System throughput
  - Utilization rates
  - Impact of constraint improvements

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
- **GENERATE TWO SEPARATE PRESCRIPTIVE PROBLEMS** (Problem A + Problem B)
- **Problem A - Linear Programming (REQUIRED)**: Always generate LP parameters
  - Provide BOTH pre-formatted Excel tables AND raw parameter data
  - Must be LINEAR problem (Simplex LP compatible)
  - Test feasibility before delivery
  - Include 2-3 binding constraints for sensitivity analysis
- **Problem B - Student Choice (REQUIRED)**: Ask which method, then generate:
  - Inventory Management (EOQ)
  - Aggregate Planning
  - Location Strategy (Factor Rating)
  - Capacity & Constraint Management
  - Provide BOTH pre-formatted tables AND raw parameter lists
- Focus on decision-making with parameter data (not transactional data)
- **Data Quality**: CLEAN data recommended (parameter data focus)
