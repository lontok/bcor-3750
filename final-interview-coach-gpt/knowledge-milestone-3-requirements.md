# Milestone 3: Prescriptive Analytics Requirements

**Due: Sunday, December 7, 2025 by 11:59 PM**
**Weight: 15% of final grade (100 points)**

## What You're Answering
- **Prescriptive**: "What should we do?" - Optimization and decision-making under constraints

## Project Continuity
- Same job and stakeholder from Milestones 01 and 02
- Flexible decision area (can be same OR different from previous milestones)
- Two separate prescriptive problems required

## Two Prescriptive Analytics Problems Required

### Problem A: Linear Programming (Required)
Must use Excel Solver (Simplex LP) to solve ONE optimization problem.

**Model Requirements:**
- Objective function (maximize or minimize)
- Clearly labeled decision variables
- Objective coefficients
- Constraints with cell references
- Solver output showing optimal values
- Sensitivity Report interpretation

**Valid LP Types:**
- **Product Mix**: Maximize profit subject to resource constraints
- **Transportation**: Minimize shipping costs from suppliers to customers
- **Labor Scheduling**: Minimize labor costs while meeting service requirements
- **Blending**: Optimize ingredient mix to meet specifications at minimum cost

### Problem B: Choose ONE Additional Method
Select ONE prescriptive method (NOT Linear Programming):

**Option 1: Inventory Management (EOQ)**
- Economic Order Quantity calculation
- Reorder point
- Safety stock calculations
- Annual total cost (ordering + holding)

**Option 2: Aggregate Planning**
- Level, Chase, or Mixed strategy comparison
- Workforce planning over multiple periods
- Cost calculations: regular time, overtime, hiring, layoffs, inventory, backorders

**Option 3: Location Strategy (Factor Rating)**
- Weighted scoring method
- Normalization of quantitative factors
- Qualitative and quantitative factor evaluation
- Site selection recommendation

**Option 4: Capacity & Constraint Management**
- Capacity, utilization, efficiency calculations
- Bottleneck identification
- Throughput rate analysis
- Break-even analysis

## Parameter Value Justification (Critical!)

**You MUST justify every parameter value with real-world grounding:**
- Industry benchmarks or published standards
- Academic or professional sources
- Job description context
- Reasonable estimates with clear reasoning
- Real company data (with citation)

**Strong Justification Example:**
> Value: Holding cost = 22% per year
> Justification: "Typical warehouse carrying costs for retail inventory range 20-30% annually (Source: Supply Chain Management textbook, 14th ed., Ch. 12). Using 22% based on mid-range warehouse with moderate climate control."

**Weak Justification (Avoid):**
- "I used the GPT's numbers because they seemed reasonable"
- "I picked 25% because I needed a number"

## Slide Deck Requirements (10 slides)

**Slide 1: Cover Slide**
- Project title, your name, date, Milestone 3

**Slide 2: Problem Definition & Stakeholder Context**
- Takeaway title connecting both problems to business value
- Visual: Overview diagram
- Bullets: Stakeholder + Problem A description + Problem B description

**Slide 3: Problem A - LP Model Overview**
- Takeaway title explaining the model
- Visual: Model structure or Excel setup screenshot
- Bullets: Objective function + Decision variables + Objective coefficients + Constraints

**Slide 4: Problem A - Solver Output**
- Takeaway title revealing optimal solution
- Visual: Solver solution screenshot
- Bullets: Recommendation (optimal values) + Impact (objective achieved)

**Slide 5: Problem A - Sensitivity Analysis Insights**
- Takeaway title revealing key insight
- Visual: Sensitivity Report excerpt or shadow price table
- Bullets: Binding constraints + Where to focus improvement

**Slide 6: Problem B - Method Overview**
- Takeaway title explaining approach
- Visual: Problem setup or calculation diagram
- Bullets: Approach used + Key inputs

**Slide 7: Problem B - Analysis Results**
- Takeaway title with specific findings
- Visual: Results table or chart
- Bullets: Key calculation/score + Interpretation

**Slide 8: Problem B - Recommendation**
- Takeaway title with actionable recommendation
- Visual: Implementation approach or comparison
- Bullets: Specific action + Expected impact

**Slide 9: Implementation Plan**
- Takeaway title with action focus
- Visual: Timeline or process diagram
- State whether short-term or long-term approach
- Bullets: Timeframe & approach + Actions + Monitoring

**Slide 10: Business Impact Summary**
- Takeaway title summarizing total value
- Visual: Summary metrics or before/after comparison
- Bullets: Problem A results + Problem B results

## Excel Workbook Requirements

**File name:** `milestone-03-fname-lname.xlsx`

### Required Worksheets:

**1. Model_A_Linear_Programming**
- Decision variables clearly labeled
- Objective function calculation
- Constraints with cell references
- Parameters organized
- All formulas visible
- Solver parameters documented
- Optimal solution displayed
- Constraint satisfaction verified (binding vs. slack)

**2. Sensitivity_Analysis_A**
- Complete Sensitivity Report from Solver
- Shadow prices interpretation
- Allowable increases/decreases for objective coefficients
- Allowable increases/decreases for constraint RHS values
- Business implications of binding constraints

**3. Model_B_[MethodName]** (choose based on your method)
- `Model_B_EOQ`
- `Model_B_Aggregate_Planning`
- `Model_B_Factor_Rating`
- `Model_B_Capacity_Analysis`

All calculations organized, formulas visible, professional formatting.

## Key Technical Concepts

### Linear Programming
- **Decision Variables**: What you're deciding (e.g., units to produce)
- **Objective Function**: What you're optimizing (max profit or min cost)
- **Objective Coefficients**: Contribution of each variable to objective
- **Constraints**: Limitations (resources, demand, capacity)
- **Binding Constraint**: Fully utilized, limits the solution
- **Slack**: Unused capacity in non-binding constraints
- **Shadow Price**: Value of one additional unit of constrained resource
- **Allowable Range**: How much coefficient can change before solution changes

### EOQ / Inventory Management
- **EOQ Formula**: √(2DS/H) where D=demand, S=order cost, H=holding cost
- **Reorder Point**: Lead time demand + safety stock
- **Total Cost**: (D/Q)×S + (Q/2)×H

### Aggregate Planning
- **Level Strategy**: Constant workforce, use inventory to meet demand
- **Chase Strategy**: Vary workforce to match demand exactly
- **Mixed Strategy**: Combination approach
- **Costs to consider**: Regular time, overtime, hiring, layoffs, inventory, backorders

### Factor Rating
- **Weights**: Sum to 1.0, reflect importance
- **Scores**: Rate each location on each factor
- **Weighted Score**: Sum of (weight × score) for each location
- **Normalization**: Convert different scales to comparable scores

### Capacity Analysis
- **Design Capacity**: Maximum possible output
- **Effective Capacity**: Realistic sustainable output
- **Utilization**: Actual output / Design capacity
- **Efficiency**: Actual output / Effective capacity
- **Bottleneck**: Process step with lowest capacity

## Common Interview Questions

### Linear Programming
- "Walk through your optimization model."
- "What are you maximizing/minimizing?"
- "Which constraints are binding?"
- "What does shadow price of $X mean?"
- "What if you relaxed [constraint] by 10%?"
- "How do you know it's optimal?"

### EOQ
- "How did you calculate holding cost?"
- "What drives reorder point?"
- "What if demand doubles?"
- "Why this safety stock level?"

### Aggregate Planning
- "Why Level vs Chase?"
- "What are the trade-offs?"
- "How did you calculate overtime costs?"
- "What assumptions about workforce flexibility?"

### Factor Rating
- "How did you determine weights?"
- "Which factor mattered most?"
- "What if weights changed?"
- "How did you normalize?"

### Capacity
- "Where's the bottleneck?"
- "Utilization vs efficiency difference?"
- "How to increase throughput 20%?"
- "Walk through break-even."

### Sensitivity Analysis
- "What does the sensitivity report tell you?"
- "Which constraint should stakeholder focus on?"
- "How much can [coefficient] change before solution changes?"
- "What's the economic value of relaxing [constraint]?"
