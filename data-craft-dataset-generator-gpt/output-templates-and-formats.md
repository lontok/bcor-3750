# Output Templates and Formats

## Data Dictionary Format

### Required Structure

Create a table with these columns:

| Column Name | Data Type | Notes |
|-------------|-----------|-------|
| [field_name] | [type] | [description and context] |

### Data Types
- Text
- Number
- Date
- Boolean
- Categorical

### Notes Should Include
- Valid value ranges (e.g., "Values between 0-100")
- Format specifications (e.g., "MM/DD/YYYY")
- Business rules (e.g., "Cannot be negative")
- Categories or codes (e.g., "N, S, E, W for regions")
- Special handling notes

### Example Entry

| Column Name | Data Type | Notes |
|-------------|-----------|-------|
| order_id | Text | Unique identifier for each order |
| order_date | Date | Date when order was placed (Format: YYYY-MM-DD, some may be MM/DD/YYYY for data quality exercise) |
| customer_id | Text | Unique identifier for customer |
| region | Categorical | Geographic region (Valid values: Northeast, Southeast, Midwest, West - used for regional performance analysis) |
| order_value | Number | Total order value in USD (Range: $10 - $10,000 - impacts shipping method selection and profitability) |

---

## README Structure

### Template Outline

```markdown
# [Scenario Name] Dataset for Analytics Project

## Operations Management Context
**Decision Area**: [Number and Name]
- [Brief description of how this dataset connects to the decision area]
- [Key decision questions this data helps answer]

## Business Context
- **Industry**: [industry]
- **Company Profile**: [company description]
- **Stakeholder**: [stakeholder role and responsibilities]
- **Business Problem**: [problem statement in required format]

## Dataset Overview
- **Records**: [number] rows
- **Variables**: [number] columns
- **Time Period**: [date range]
- **Granularity**: [daily/weekly/monthly]

## Files Included
1. `[filename]_data.csv` - Primary dataset
2. `data_dictionary.csv` - Field definitions

## Data Quality Issues (Milestone-Specific)

**For Milestone 1 (Descriptive/Diagnostic):**

This dataset includes realistic data quality issues you'll need to address using the **Data Quality Framework**:

**Framework Steps:**
1. **Identify** the data quality issue
2. **Assess** the business ramification
3. **Analyze** the root cause
4. **Decide** on the best option (Remove / Update / Do Nothing)
5. **Fix** the issue, if applicable

**Issues Included:**
- **Missing Values**: ~[X]% of records have missing data in [fields]
- **Duplicates**: ~[X]% duplicate records
- **Date Formats**: Mixed YYYY-MM-DD and MM/DD/YYYY formats
- **Outliers**: Some records have anomalous values in [fields]
- **Inconsistent Categories**: Variations in [categorical fields]

**For Milestone 2 (Predictive Analytics):**

This dataset contains **CLEAN data ready for predictive modeling**. No data quality issues are present - focus on forecasting and regression analysis.

**For Milestone 3 (Prescriptive Analytics):**

Same as Milestone 1 - includes intentional data quality issues for comprehensive learning.

## Suggested Analysis Approach

### DC ACT Framework
1. **Define** the business problem
2. **Collect** and prepare the data
3. **Analyze** the data and generate insights
4. **Communicate** the insights, recommendations, and predictions
5. **Act** and track the change

### For Milestone 1: Descriptive & Diagnostic Analytics

**Descriptive (What happened?)**
- Calculate summary statistics (mean, median, mode, standard deviation)
- Analyze trends over time
- Identify patterns by [dimensions]
- Create visualizations showing distributions and trends
- **Connection to [Decision Area]**: [Specific insights this provides]

**Diagnostic (Why did it happen?)**
- Use pivot tables to drill down into [key metric] by [dimensions]
- Apply slicers to filter data and identify root causes
- Compare performance across [segments]
- Investigate why [metric] varies by [dimension]
- **Connection to [Decision Area]**: [Specific root causes to investigate]

### For Milestone 2: Predictive Analytics

**IMPORTANT**: Milestone 2 requires TWO separate predictive analyses with TWO different datasets:

**Time Series Forecasting (Problem A):**
- Decompose time series to identify: trend, seasonal, cyclic, random patterns
- Test minimum 3 forecasting models:
  - N-Period Moving Average
  - N-Period Weighted Moving Average
  - Excel's FORECAST.LINEAR
  - Excel's FORECAST.ETS
- Compare forecast accuracy (MAD, MSE, MAPE)
- Select BEST method and justify
- Generate forecast for next period
- **Connection to [Decision Area]**: [What predictions help decide]

**Multiple Linear Regression (Problem B):**
- Conduct correlation analysis to identify relationships
- Test minimum 3 multiple regression models (each with 2+ independent variables)
- Dependent variable: [variable]
- Independent variables (4-6 total): [variables]
- Interpret: Adjusted R², coefficients, p-values, significance
- Select BEST model and justify
- Make predictions for 2-3 scenarios
- **Connection to [Decision Area]**: [What relationships help decide]

### For Milestone 3: Prescriptive Analytics

**Linear Programming:**
- Decision variables: [variables]
- Objective: Maximize/Minimize [metric]
- Constraints: [list constraints]
- Use Excel Solver to find optimal solution
- **Connection to [Decision Area]**: [What this optimizes]

**OR Monte Carlo Simulation:**
- Uncertain variable: [variable]
- Distribution: [distribution type with parameters]
- Run 1,000-10,000 simulations
- Analyze probability distributions of outcomes
- Determine risk and confidence intervals
- **Connection to [Decision Area]**: [What uncertainty this models]

## Business Questions to Answer

1. **Descriptive**: [Question related to descriptive analytics and decision area]
2. **Diagnostic**: [Question related to diagnostic analytics and decision area]
3. **Predictive**: [Question related to predictive analytics and decision area]
4. **Prescriptive**: [Question related to prescriptive analytics and decision area]

## Interview Preparation

Be ready to discuss using the DC ACT Framework:

**Define:**
- Why did you choose this problem and how does it relate to [Decision Area]?
- Who is your stakeholder and why do they care?

**Collect:**
- How did you collect the data?
- What data quality issues did you find and how did you address them?

**Analyze:**
- What insights did you discover across the analytics maturity scale?
- How did you progress from descriptive → diagnostic → predictive → prescriptive?

**Communicate:**
- What are your key takeaways (use takeaway slide titles)?
- How do visualizations support your insights?

**Act:**
- What specific actions should your stakeholder take?
- How will these actions improve decisions in [Decision Area]?
- How would you track the impact of these changes?

---
Generated by Data Craft GPT for BCOR 3750 Analytics Project
Connected to Operations Management Decision Area: [Decision Area]
```

---

## Final Confirmation Checklist

Before generating, confirm with user:

### Context Summary
- **Industry**: [industry]
- **Company**: [company type]
- **Operations Management Decision Area**: [decision area]
- **Stakeholder**: [stakeholder role]
- **Problem**: [problem statement]

### Dataset Specifications
- **Analytics Type**: [Descriptive/Diagnostic/Predictive/Prescriptive]
- **Scenario**: [operational scenario]
- **Time Period**: [time range]
- **Granularity**: [daily/weekly/monthly]
- **Key Metrics**: [list metrics]
- **Sample Size**: [number of records]
- **Data Quality Issues**: [types of issues included]

### File Deliverables

**For Milestone 1:**
1. Primary dataset (CSV)
2. Data dictionary (explains all fields)
3. README with problem context, decision area connection, and analysis guidance

**For Milestone 2 (TWO SEPARATE DATASETS):**
1. **Time Series Dataset**: CSV + data dictionary + README (Problem A)
2. **Regression Dataset**: CSV + data dictionary + README (Problem B)

**For Milestone 3:**
1. Primary dataset (CSV)
2. Data dictionary
3. [If applicable]: Optimization parameters OR simulation variability data
4. README with problem context and analysis guidance

**Ask**: "Does this match your needs, or should I adjust anything?"

---

## Post-Generation Next Steps Message

```markdown
Your dataset is ready! Here's what I've included:

📊 **Dataset Summary:**
- [Number] records across [number] variables
- Time period: [period covered]
- Intentional data quality issues: [list issues]
- Connected to Operations Management Decision Area: **[Decision Area]**

📁 **Files Included:**

**For Milestone 1:**
1. `[filename]_data.csv` - Primary dataset
2. `data_dictionary.csv` - Field definitions and descriptions
3. `README.md` - Context, problem statement, decision area connection, and analysis guidance

**For Milestone 2 (TWO SEPARATE DELIVERIES):**

**Dataset 1 - Time Series Forecasting (Problem A):**
1. `[filename]_timeseries_data.csv` - Time series dataset
2. `timeseries_data_dictionary.csv` - Field definitions
3. `timeseries_README.md` - Problem A context and forecasting guidance

**Dataset 2 - Multiple Regression (Problem B):**
1. `[filename]_regression_data.csv` - Regression dataset
2. `regression_data_dictionary.csv` - Field definitions
3. `regression_README.md` - Problem B context and regression guidance

**For Milestone 3:**
1. `[filename]_data.csv` - Primary dataset
2. `data_dictionary.csv` - Field definitions
3. `README.md` - Context and guidance
4. [If applicable]: `[filename]_optimization_params.csv` or `[filename]_simulation_data.csv`

💡 **Next Steps for Your Analysis:**

**DC ACT Framework (5-Step Analytics Framework):**
1. **Define** the business problem - You've identified the problem for [Decision Area]
2. **Collect** and prepare the data - Use the Data Quality Framework to clean your data
3. **Analyze** the data and generate insights - Apply your analytics techniques
4. **Communicate** the insights, recommendations, and predictions - Prepare your slides
5. **Act** and track the change - Recommend specific actions for your stakeholder

**Analytics Progression:**
1. **Data Quality Phase**: Use the Data Quality Framework (Identify → Assess → Analyze → Decide → Fix)
2. **Descriptive Analytics**: Explore distributions, trends, and summary statistics (What happened?)
3. **Diagnostic Analytics**: Investigate root causes using pivot tables and slicers (Why did it happen?)
4. **Predictive Analytics**: Build forecasting models - moving average, exponential smoothing, regression (What will happen?)
5. **Prescriptive Analytics**: Develop optimization models (Solver) and/or simulation (Monte Carlo) (What should we do?)

🎯 **Remember for Your Interview:**
You'll need to explain:
- Why you chose this problem and how it relates to [Decision Area]
- How you collected and prepared the data (including data quality issues you addressed)
- What insights you discovered across the analytics maturity scale
- What actions you recommend to your stakeholder
- How your recommendations help make better decisions in [Decision Area]

The AI helped you structure the data, but YOU need to understand and interpret it. Good luck!
```
