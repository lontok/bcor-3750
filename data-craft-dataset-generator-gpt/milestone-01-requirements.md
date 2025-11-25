# Milestone 1: Descriptive & Diagnostic Analytics

**Analytics Types**: Descriptive (What happened?) + Diagnostic (Why did it happen?)

## Technical Requirements

### Dataset Structure
- **500-1,000 rows** with realistic operational data
- **5+ variables** including:
  - Date/time field (REQUIRED) - daily, weekly, or monthly granularity
  - Categorical dimensions for grouping/comparison (regions, products, categories)
  - Numeric metrics for analysis (sales, costs, quantities, rates)
  - Text fields where appropriate (IDs, names, descriptions)

### Data Quality Issues (ALWAYS INCLUDE ALL 5)

**CRITICAL**: Students do NOT choose which issues to include. ALL datasets MUST contain ALL 5 quality issue types for comprehensive learning practice.

1. **Missing Values** (2-3% of records):
   - Randomly distributed across 2 fields
   - Excel: leave cells empty (blank)
   - CSV: leave cells empty or use blank string

2. **Duplicate Records** (1-3% of records):
   - Exact duplicates of random existing records
   - Creates data integrity issues students must identify

3. **Date Format Inconsistencies** (REQUIRED):
   - Mix YYYY-MM-DD and MM/DD/YYYY formats
   - ~50% of dates in each format
   - Creates parsing/sorting challenges

4. **Outliers** (1-2% of records in 1 numeric field):
   - Realistic but anomalous values
   - Not errors, but unusual observations
   - Example: sales spike, unusually high/low values

5. **Inconsistent Categories** (REQUIRED):
   - Variations in categorical field values
   - Example: "Northeast" vs "North East" vs "NE"
   - Creates grouping/aggregation challenges

**Important**: These issues are intentional for learning purposes. Students will use the Data Quality Framework to identify, assess, analyze, decide, and fix each issue.

## Deliverables

Students must submit:

1. **CSV Dataset** - Raw data with all 5 quality issues
2. **Data Dictionary** - Column definitions, data types, notes
3. **README** - Business context, problem statement, decision area connection, analysis guidance

## Analysis Requirements

Students will perform:

### Descriptive Analytics (What happened?)
- Summary statistics (mean, median, mode, standard deviation)
- Trend analysis over time using date/time field
- Distribution analysis by categorical dimensions
- Visualizations: trend charts, distributions, comparisons
- **Strategic Dashboard** (Slide 11): Trend charts require date/time field

### Diagnostic Analytics (Why did it happen?)
- Root cause investigation using pivot tables
- Slicers for filtering and drilling down
- Cross-dimensional comparisons
- Pattern identification
- **Operational Dashboard** (Slide 14): Trend charts require date/time field

### Data Quality Framework Application
Students must document how they:
1. **Identify** - Find each of the 5 quality issues
2. **Assess** - Determine business impact of each issue
3. **Analyze** - Investigate root cause
4. **Decide** - Choose approach (Remove/Update/Do Nothing)
5. **Fix** - Implement solution and document in cleaning log

## Key Questions to Ask Students

During discovery phase, ask sequentially (ONE at a time):

1. **Operational Scenario**: "What operational process or business activity should this dataset represent?"
2. **Time Period**: "What time period should the data cover? (e.g., 6 months, 1 year, 2 years)"
3. **Granularity**: "What level of detail? (daily transactions, weekly summaries, monthly aggregates)"
4. **Key Metrics**: "What numeric metrics matter for analysis? (sales, costs, quantities, rates, percentages)"
5. **Dimensions**: "What categorical dimensions for comparison? (regions, products, customers, channels)"

Then INFORM (don't ask): "Your dataset will include all standard data quality issues for comprehensive learning practice: missing values, duplicates, date format inconsistencies, outliers, and inconsistent categories."

## Generation Guidelines

### Data Realism
- Use realistic business values appropriate to industry/context
- Ensure date/time field covers sufficient period for trend analysis
- Create meaningful patterns in the data (trends, seasonal effects, regional differences)
- Make quality issues realistic but discoverable

### Quality Issue Distribution
- Spread issues across different records (don't cluster)
- Make issues discoverable but not immediately obvious
- Ensure issues create meaningful learning opportunities
- Test that each issue type is present and identifiable

### Documentation
- Data dictionary must explain all fields clearly
- README must connect to Operations Management Decision Area
- README must explain DC ACT Framework application
- README must provide analysis guidance specific to the scenario
