# Project Milestones 2 & 3 - Detailed Requirements
## (To be released after Milestone 1 completion)

---

## Milestone 2: Predictive Analytics
**Due: Tuesday, November 4, 2025 by 11:59 PM**
**Weight: 15 points**

### What You're Answering:
- **Predictive**: "What will happen?" - Forecasting and prediction

### Technical Requirements

**Time Series Forecasting (Excel):**
You must apply BOTH methods and compare results:

1. **Moving Average**
   - 3-month (or 3-week/3-day depending on granularity)
   - 6-month (or 6-week/6-day)
   - Calculate forecast accuracy (MAPE or RMSE)

2. **Exponential Smoothing**
   - Alpha = 0.2 (slow response to changes)
   - Alpha = 0.5 (moderate response)
   - Calculate forecast accuracy (MAPE or RMSE)

**Comparison Required:**
- Create a table comparing all methods' accuracy
- Select the BEST method and justify your choice
- Generate forecast for next period using your selected method

**Multiple Linear Regression (Excel):**
- Dependent variable: What you're predicting
- Independent variables: 3-8 factors that influence the dependent variable
- Use Excel Data Analysis Toolpak for regression
- **Interpret Key Outputs**:
  - Adjusted R² (how well the model fits)
  - Coefficients (relationship between each independent variable and dependent variable)
  - P-values (statistical significance)
  - Y-intercept (baseline prediction)
- Make predictions for new scenarios using your model
- Discuss business implications of the relationships you found

### Deliverables (DC ACT Framework)

**1. Define**
- What are you trying to predict and why?
- How does this prediction help your stakeholder make better decisions?
- Time horizon for forecast (next week? month? quarter?)

**2. Collect**
- If using new dataset: Include Data_Cleaning_Log worksheet (same format as Milestone 1)
- If using same dataset: Explain why it's suitable for forecasting/regression
- Data dictionary (if new dataset)

**3. Analyze**
- Excel workbook with:
  - Data_Cleaning_Log tab (if using new dataset)
  - Time Series Forecasting tab (both methods, comparison, selected forecast)
  - Regression Analysis tab (model output, interpretation, predictions)
  - Clear labels, formulas visible, professional formatting
- **Show your work**: Don't just paste regression output—annotate what it means

**4. Communicate**
- **Slide Deck** (3-5 NEW slides added to your existing deck):
  - **Slide 1**: Forecasting problem and approach
  - **Slide 2**: Time series results with **takeaway title** (which method works best? what's the forecast?)
  - **Slide 3**: Regression results with **takeaway title** (what relationships drive predictions?)
  - **Slide 4-5**: Business implications and how stakeholder should use these predictions
  - Each slide must have:
    - Takeaway title (the insight, not "Regression Analysis")
    - Supporting visual (chart showing forecast, regression coefficients, etc.)
    - Interpretation of what this means for the business

**5. Act**
- How should your stakeholder use these predictions?
- What decisions can be made with this forecast?
- What are the risks/limitations of the predictions?
- How to monitor actual vs. predicted (track prediction accuracy)

### Submission Files
Upload to Brightspace by **Tuesday, November 4, 2025, 11:59 PM**:

1. `[LastName]_[FirstName]_Milestone2_Slides.pptx` or `.pdf` (cumulative deck with Milestone 1 + 2 slides)
2. `[LastName]_[FirstName]_Milestone2_Analysis.xlsx` (must include Data_Cleaning_Log worksheet if using new dataset)
3. `[LastName]_[FirstName]_Milestone2_Data.csv` (if using new dataset)

---

## Milestone 3: Prescriptive Analytics
**Due: Thursday, December 4, 2025 by 11:59 PM**
**Weight: 15 points**

### What You're Answering:
- **Prescriptive**: "What should we do?" - Optimization and simulation for decision-making

### Technical Requirements

You must complete BOTH analyses (or justify why only one applies):

**1. Linear Programming with Excel Solver**

**Setup:**
- **Decision Variables**: 3-10 variables representing choices (how much to produce? how to allocate resources?)
- **Objective Function**: What are you maximizing or minimizing? (profit, cost, throughput, etc.)
- **Constraints**: 4-8 limitations (budget, capacity, time, minimum/maximum requirements)

**Analysis:**
- Build optimization model in Excel
- Use Solver to find optimal solution
- Run sensitivity analysis (what happens if constraints change?)
- Interpret results in business terms

**Example Problem Types:**
- Production planning: How many units of each product to produce?
- Resource allocation: How to allocate warehouse space to maximize profit?
- Transportation: Which routes/carriers to use to minimize cost?
- Inventory: What reorder quantities minimize total inventory costs?

---

**2. Monte Carlo Simulation (Excel)**

**Setup:**
- **Uncertain Variable(s)**: What has variability? (demand, lead time, defect rate, costs)
- **Probability Distribution**: Normal, uniform, or triangular distribution with parameters
- **Simulation**: Run 1,000-10,000 scenarios using Excel's random number functions

**Analysis:**
- Model the uncertain process in Excel
- Generate random values based on probability distribution
- Calculate outcome for each simulation run
- Analyze distribution of outcomes (mean, standard deviation, percentiles)
- Determine probabilities and confidence intervals

**Example Problem Types:**
- Inventory risk: What's the probability of stockout given variable demand and lead times?
- Capacity planning: How much capacity needed to meet demand 95% of the time?
- Quality: What's expected defect rate given variable process performance?
- Financial: What's the range of possible costs/revenues given variable inputs?

---

**Basic Complexity Guidance:**
This is your first exposure to these advanced techniques. We expect:
- **Linear Programming**: Basic problem with 3-6 decision variables, 4-6 constraints
- **Simulation**: Single uncertain variable with clear probability distribution
- **Focus**: Correct application of technique and business interpretation, not mathematical sophistication

---

### Deliverables (DC ACT Framework)

**1. Define**
- What decision is your stakeholder trying to make?
- What are they trying to optimize or understand uncertainty around?
- Why does this require prescriptive analytics (not just prediction)?

**2. Collect**
- Data for optimization parameters (costs, profits, capacities, limits)
- Historical data showing variability for simulation
- If using new dataset: Include Data_Cleaning_Log worksheet (same format as Milestone 1)
- Data dictionary (if new dataset)

**3. Analyze**
- Excel workbook with:
  - Data_Cleaning_Log tab (if using new dataset)
  - **Linear Programming tab**:
    - Decision variables clearly labeled
    - Objective function formula
    - Constraint formulas
    - Solver setup and solution
    - Sensitivity analysis results
  - **Monte Carlo Simulation tab**:
    - Random number generation formulas
    - Simulation model (1,000-10,000 runs)
    - Distribution of outcomes
    - Statistical summary (mean, std dev, percentiles)
    - Probability calculations
  - Clear documentation of assumptions, formulas, and results

**4. Communicate**
- **Slide Deck** (3-5 NEW slides added to your cumulative deck):
  - **Slide 1**: Prescriptive problem and approach
  - **Slide 2**: Optimization results with **takeaway title** (what's the optimal solution?)
  - **Slide 3**: Simulation results with **takeaway title** (what's the probability distribution? risk assessment?)
  - **Slide 4-5**: Decision recommendations and implementation roadmap
  - Each slide must have:
    - Takeaway title (the actionable insight)
    - Supporting visual (optimal solution table, probability distribution chart, etc.)
    - Interpretation of what stakeholder should do

**5. Act**
- **Specific Recommendations**: Based on optimization, what should stakeholder do?
- **Risk Assessment**: Based on simulation, what are the risks and how to mitigate?
- **Implementation Plan**: Steps to implement optimal solution
- **Monitoring Plan**: How to track if optimization is working, when to re-optimize

---

### Submission Files
Upload to Brightspace by **Thursday, December 4, 2025, 11:59 PM**:

1. `[LastName]_[FirstName]_Milestone3_Slides.pptx` or `.pdf` (COMPLETE cumulative deck with all milestones)
2. `[LastName]_[FirstName]_Milestone3_Analysis.xlsx` (must include Data_Cleaning_Log worksheet if using new dataset)
3. `[LastName]_[FirstName]_Milestone3_Data.csv` (if using new dataset)

---

## Grading Rubrics

### Milestone 2: Predictive Analytics Rubric (15 points)

#### Data Quality & Preparation (2 points)
- **If new dataset**: Same Data_Cleaning_Log rubric as Milestone 1 (worksheet must be present in Excel file)
- **If same dataset**: 2 points for explaining suitability for forecasting/regression

#### Technical Analysis Execution (4 points)
- **4.0 - Excellent**:
  - Time Series: Both methods applied correctly, accurate forecast, valid comparison, best method selected with justification
  - Regression: Correct model, all key outputs interpreted correctly (R², coefficients, p-values), valid predictions
  - Formulas and work shown clearly
- **3.0 - Good**:
  - Time Series: Both methods applied, forecast generated, comparison adequate, method selection reasonable
  - Regression: Correct model, most outputs interpreted, predictions made
  - Work mostly clear
- **2.0 - Adequate**:
  - Time Series: One or both methods applied with minor errors, forecast generated, limited comparison
  - Regression: Model built but interpretation incomplete, predictions attempted
  - Work somewhat unclear
- **1.0 - Poor**:
  - Time Series: Significant errors in methods, forecast questionable, no comparison
  - Regression: Model incorrect or interpretation missing, predictions invalid
  - Work unclear or missing
- **0 - Missing**: No technical analysis

#### Business Insights & Interpretation (2.5 points)
- **2.5 - Excellent**: Insights explain what predictions mean for business, clear implications, connects to decision-making
- **2.0 - Good**: Insights relate predictions to business, general implications, some connection to decisions
- **1.5 - Adequate**: Generic insights, limited business relevance, weak connection to decisions
- **1.0 - Poor**: No clear business insights, just technical results
- **0 - Missing**: No insights

#### Recommendations & Actions (2 points)
- **2.0 - Excellent**: Specific guidance on how to use predictions, decision framework, risk/limitation discussion, monitoring plan
- **1.5 - Good**: Clear guidance on using predictions, some decision support, mentions limitations, basic monitoring
- **1.0 - Adequate**: General recommendations, limited decision support, minimal limitation discussion
- **0.5 - Poor**: Vague recommendations, no decision support
- **0 - Missing**: No recommendations

#### Presentation Clarity (4.5 points)
Same rubric as Milestone 1

---

### Milestone 3: Prescriptive Analytics Rubric (15 points)

#### Data Quality & Preparation (2 points)
- **If new dataset**: Same Data_Cleaning_Log rubric as Milestone 1 (worksheet must be present in Excel file)
- **If same dataset**: 2 points for explaining suitability for optimization/simulation

#### Technical Analysis Execution (4 points)
- **4.0 - Excellent**:
  - Linear Programming: Correct model setup, valid constraints, Solver used correctly, optimal solution found, sensitivity analysis completed
  - Simulation: Correct probability distributions, 1000+ runs, distribution analyzed correctly, probabilities calculated
  - Both analyses completed (or one justified thoroughly)
- **3.0 - Good**:
  - Linear Programming: Model mostly correct, Solver used, solution found, limited sensitivity analysis
  - Simulation: Correct approach, adequate runs, basic distribution analysis
  - Both analyses attempted
- **2.0 - Adequate**:
  - Linear Programming: Model setup with errors, Solver used, solution questionable
  - Simulation: Basic approach, limited runs, incomplete analysis
  - One or both analyses incomplete
- **1.0 - Poor**:
  - Significant errors in setup or execution
  - Only one analysis attempted with major issues
- **0 - Missing**: No technical analysis

#### Business Insights & Interpretation (2.5 points)
- **2.5 - Excellent**: Insights explain optimal solution/risk profile in business terms, clear decision implications, connects to decision area
- **2.0 - Good**: Insights relate results to business, general implications, some decision guidance
- **1.5 - Adequate**: Generic insights, limited business relevance
- **1.0 - Poor**: No clear business insights, just technical results
- **0 - Missing**: No insights

#### Recommendations & Actions (2 points)
- **2.0 - Excellent**: Specific implementation plan for optimal solution, risk mitigation strategies, monitoring and re-optimization plan
- **1.5 - Good**: Clear implementation guidance, some risk discussion, basic monitoring plan
- **1.0 - Adequate**: General recommendations, limited implementation detail
- **0.5 - Poor**: Vague recommendations, no implementation plan
- **0 - Missing**: No recommendations

#### Presentation Clarity (4.5 points)
Same rubric as Milestone 1
