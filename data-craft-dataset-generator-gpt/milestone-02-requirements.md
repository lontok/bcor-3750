# Milestone 2: Predictive Analytics

**Analytics Types**: Time Series Forecasting + Multiple Linear Regression

**CRITICAL**: Students must complete **TWO SEPARATE PREDICTIVE ANALYSES** with **TWO DIFFERENT DATASETS**

## Dataset Requirements

### General Requirements
- **CLEAN DATA ONLY** - NO quality issues (no missing values, duplicates, outliers, or format issues)
- Focus is on predictive modeling, not data cleaning
- Each dataset addresses a different predictive problem
- Both datasets must support required analysis techniques

### Dataset 1: Time Series Forecasting

**Structure Requirements**:
- **18-24 months of data** (NO GAPS - continuous time series)
- **ONE time-stamped record per period** (daily, weekly, or monthly)
- **Target variable** to forecast (numeric)
- **Date/time field** in consistent format (YYYY-MM-DD)
- 3-5 additional context variables (optional but helpful)

**Pattern Requirements** (INTERNAL - NEVER MENTION TO STUDENTS):
- Data MUST internally contain:
  - **Trend component** (increasing, decreasing, or stable)
  - **Seasonal component** (recurring patterns)
  - Realistic variation (not perfectly smooth)
- **NEVER mention** pattern types to students in README or data dictionary
- **NEVER use words**: "trend", "seasonal", "increasing", "decreasing", "cyclical", "pattern"
- Students must discover patterns through decomposition analysis

**Analysis Requirements**:
Students must:
- Decompose time series (identify trend, seasonal, cyclic, random components)
- Test minimum 3 forecasting methods:
  - N-Period Moving Average
  - N-Period Weighted Moving Average
  - Excel's FORECAST.LINEAR
  - Excel's FORECAST.ETS (optional)
- Compare forecast accuracy using MAD, MSE, MAPE
- Select BEST method and justify selection
- Generate forecast for ONE future period (not 12 periods)

**Deliverable Format**:
- Excel workbook: `milestone-02-time-series-fname-lname.xlsx`
- Three worksheets:
  1. **Raw**: Time series dataset (clean data, 18-24 months, NO GAPS)
  2. **Data_Dictionary**: Field definitions
  3. **Time_Series_Forecasting**: Empty worksheet for student's analysis

### Dataset 2: Multiple Linear Regression

**Structure Requirements**:
- **500-1,000 records** (cross-sectional data)
- **ONE dependent variable** (numeric, continuous)
- **4-6 independent variables** (ALL NUMERIC - NO categorical variables)
- Dates NOT required (cross-sectional analysis)
- Moderate correlations between IVs and DV (0.3-0.8 range)

**CRITICAL - NO Categorical Variables**:
- Students have NOT learned dummy variable creation
- ALL independent variables must be NUMERIC only
- No region codes, no product types, no categories
- Use only: counts, amounts, percentages, ratios, rates, scores

**Variable Relationships**:
- Create realistic correlations between IVs and DV
- Avoid perfect multicollinearity between IVs
- Ensure adjusted R² of 0.65-0.80 is achievable with best model
- Support testing minimum 3 different model combinations

**Analysis Requirements**:
Students must:
- Conduct correlation analysis
- Test minimum 3 multiple regression models (each with 2+ independent variables)
- Interpret: Adjusted R², coefficients, p-values, significance (α = 0.05)
- Select BEST model and justify selection
- Make predictions for 2-3 scenarios using best model

**Deliverable Format**:
- Excel workbook: `milestone-02-regression-fname-lname.xlsx`
- Three worksheets:
  1. **Raw**: Regression dataset (clean data, 500-1000 records, 4-6 numeric IVs)
  2. **Data_Dictionary**: Field definitions
  3. **Regression_Analysis**: Empty worksheet for student's analysis

## Key Questions to Ask Students

### For Time Series Forecasting (Ask sequentially, ONE at a time):
1. **Target Variable**: "What do you want to forecast? (sales, demand, production, costs, etc.)"
2. **Time Horizon**: "How far into the future? (1 week, 1 month, 1 quarter ahead)"
3. **Data Period**: "How much historical data? (18-24 months recommended for pattern detection)"
4. **Business Context**: "What business decisions depend on this forecast?"

### For Multiple Linear Regression (Ask sequentially, ONE at a time):
1. **Dependent Variable**: "What outcome are you trying to predict? (must be numeric)"
2. **Independent Variables**: "What 4-6 NUMERIC factors might influence this outcome? (only numbers - counts, amounts, percentages, rates)"
3. **Business Context**: "What business decisions depend on understanding these relationships?"
4. **Data Scope**: "What records should be included? (time period, geographic scope, business units)"

## Generation Guidelines

### Time Series Dataset
- Ensure 18-24 continuous months with NO GAPS
- Internally generate trend + seasonal components (NEVER mention to students)
- Use realistic values appropriate to business context
- Create patterns strong enough to detect but not perfectly obvious
- Test that forecasting methods will yield different accuracy results

### Regression Dataset
- Generate 500-1000 records with realistic distributions
- Create moderate correlations (avoid too weak or too strong)
- ALL independent variables must be NUMERIC (no categories)
- Ensure multicollinearity is avoided between IVs
- Test that multiple models can be compared meaningfully
- Target adjusted R² of 0.65-0.80 for best model

### Documentation
- Data dictionary explains all variables (units, ranges, business meaning)
- README connects both problems to Operations Management Decision Area
- README provides analysis guidance for both time series and regression
- README explains DC ACT Framework application
- **NEVER mention pattern types** (trend, seasonal) in any student-facing documentation

## Common Mistakes to Avoid

### Time Series
- ❌ Gaps in the time series (missing months)
- ❌ Less than 18 months of data
- ❌ Mentioning "trend" or "seasonal" in README or data dictionary
- ❌ Patterns too obvious or too hidden
- ❌ Forecast requirement of 12 periods (should be ONE period)

### Regression
- ❌ Including categorical variables (region, product type, etc.)
- ❌ Less than 4 or more than 6 independent variables
- ❌ Perfect multicollinearity between IVs
- ❌ Too weak relationships (adjusted R² < 0.50)
- ❌ Including dates as variables (not needed for cross-sectional)
