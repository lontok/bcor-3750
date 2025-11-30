# Milestone 2: Predictive Analytics Requirements

**Due: Tuesday, November 11, 2025 by 11:59 PM**
**Weight: 15% of final grade (100 points)**

## What You're Answering
- **Predictive**: "What will happen?" - Forecasting and prediction

## Project Continuity
- Same job and stakeholder from Milestone 01
- Flexible decision area (can be same OR different from Milestone 01)
- New problem focused on predictive analytics
- New dataset structured for time series forecasting and multiple linear regression
- Clean data - no data quality issues to fix

## Two Separate Predictive Analyses Required

### 1. Time Series Forecasting Analysis (Problem A)
- Test minimum 3 different forecasting models
- Select 1 best model based on accuracy measures
- Generate forecast for ONE next period only

**Models to test (minimum 3):**
- N-Period Moving Average (e.g., 3-month, 6-month)
- N-Period Weighted Moving Average
- Excel's FORECAST.LINEAR (for trend projection)
- Excel's FORECAST.ETS (for trend + seasonality)

**Accuracy measures:**
- MAD (Mean Absolute Deviation)
- MSE (Mean Squared Error)
- MAPE (Mean Absolute Percentage Error)

### 2. Multiple Linear Regression Analysis (Problem B)
- Conduct correlation analysis to identify promising predictor variables
- Create scatter plots for top 3 independent variables
- Test minimum 2 multiple regression models (each with 2+ independent variables)
- Select 1 best model based on fit and significance
- Make predictions for 2-3 scenarios

**Key regression outputs to interpret:**
- Adjusted R² (model fit)
- Coefficients (relationships between variables)
- P-values (statistical significance)
- Y-intercept (baseline prediction)
- Standard Error
- Significance F

## Slide Deck Requirements (11 slides)

### Slide 1: Milestone 02 Overview
- Job and stakeholder (reference from Milestone 01)
- Two predictive problems (Time Series + Regression)
- Connection to Milestone 01

### SECTION A: TIME SERIES FORECASTING (Slides 2-5)

**Slide 2: Time Series Problem Statement**
- Takeaway title stating what's being forecasted
- Visual: Line chart of historical data
- Bullets: Problem + Impact

**Slide 3: Time Series Decomposition and Pattern Identification**
- Takeaway title identifying patterns found
- Visual: Decomposition chart or annotated line chart
- Identify: Trend, Seasonal, Cyclic, Random components
- Bullets: Data characteristics + Recommended methods

**Slide 4: Time Series Model Comparison**
- Takeaway title announcing winner
- Visual: Comparison table with 3+ models and accuracy measures
- Bullets: Recommendation + Justification

**Slide 5: Forecast Results**
- Takeaway title with forecast insight
- Visual: Line chart with historical + ONE forecast period
- Bullets: Recommendation + Prediction

### SECTION B: REGRESSION ANALYSIS (Slides 6-11)

**Slide 6: Regression Problem Statement**
- Takeaway title stating what you're predicting
- Visual: Conceptual diagram
- Bullets: Problem + Impact

**Slide 7: Regression Dataset Overview**
- Takeaway title about data characteristics
- Visual: Dataset characteristics table
- Bullets: Data description + Variables

**Slide 8: Correlation Analysis**
- Takeaway title revealing correlation insight
- Visual: Correlation matrix with conditional formatting
- Bullets: Variables being tested + Promising predictors

**Slide 9: Regression Model Comparison**
- Takeaway title announcing winning model
- Visual: Model comparison table (2+ models)
- Bullets: Recommendation + Justification

**Slide 10: Key Drivers and Relationships**
- Takeaway title revealing driver insight
- Visual: Coefficient chart or regression equation
- Bullets: Which factors to manage + Coefficient interpretation

**Slide 11: Prediction Scenarios**
- Takeaway title with scenario insight
- Visual: Table with 2-3 scenarios and predictions
- Bullets: How to use predictions + Expected outcomes

## Excel Workbook Requirements

### Workbook 1: Time Series Forecasting
**File name:** `milestone-02-time-series-fname-lname.xlsx`

Required worksheets:
1. **Raw** - Original dataset (unmodified)
2. **Data_Dictionary** - Field definitions
3. **Time_Series_Forecasting** - All analysis:
   - Historical data with date/time column
   - Line chart of target variable over time
   - Pattern decomposition (trend, seasonal, cyclic, random)
   - Minimum 3 forecasting models tested
   - Error measures (MAD, MSE, MAPE) for each model
   - Model comparison table
   - Best model highlighted with justification
   - Forecast for ONE next period

### Workbook 2: Multiple Linear Regression
**File name:** `milestone-02-regression-fname-lname.xlsx`

Required worksheets:
1. **Raw** - Original dataset (unmodified)
2. **Data_Dictionary** - Field definitions
3. **Regression_Analysis** - All analysis:
   - Correlation matrix with conditional formatting
   - Scatter plots for top 3 independent variables with trendlines
   - Minimum 2 regression models (2+ variables each)
   - Regression outputs clearly labeled
   - Model comparison table
   - Best model with coefficient interpretation
   - Scenario predictions table (2-3 scenarios)

## Key Technical Concepts

### Time Series Components
- **Trend**: Long-term increase or decrease
- **Seasonal**: Regular fluctuations within a year
- **Cyclic**: Multi-year patterns
- **Random**: Irregular variations

### Regression Interpretation
- **Adjusted R²**: Proportion of variance explained (adjusted for number of variables)
- **Coefficient**: Change in Y for 1-unit change in X
- **P-value**: Probability result is due to chance (< 0.05 = significant)
- **Standard Error**: Average prediction error

### Model Selection Criteria
**Time Series:**
- Lower MAPE = better accuracy
- Model should capture identified patterns (trend, seasonality)

**Regression:**
- Higher Adjusted R² = better fit
- All variables should be significant (p < 0.05)
- Lower Standard Error = more precise predictions
- Consider parsimony (simpler model if fit is similar)

## Common Interview Questions

### Time Series
- "What patterns did you identify?"
- "Why did [method] outperform others?"
- "What does MAPE of X% mean?"
- "How confident are you in your forecast?"
- "What would change your forecast?"

### Regression
- "Walk through your correlation analysis."
- "What does coefficient of X mean?"
- "Why exclude certain variables?"
- "What does Adjusted R² of X tell you?"
- "Interpret a 10% increase in [variable]."
