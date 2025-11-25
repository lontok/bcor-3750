# Milestone 3: Prescriptive Analytics

**Analytics Types**: TWO Prescriptive Problems Required

**CRITICAL**: Students must complete **TWO SEPARATE PRESCRIPTIVE ANALYSES**:
- **Problem A**: Linear Programming (REQUIRED for all students)
- **Problem B**: Student chooses ONE method from 4 options

## Data Type: Parameter Data (Not Transactional)

**Important Distinction**:
- Milestones 1-2 used transactional/operational data (rows of transactions)
- Milestone 3 uses **parameter data** (model inputs, coefficients, constraints)
- Focus is on decision-making and optimization, not data cleaning
- **CLEAN data recommended** (no quality issues)

## Problem A: Linear Programming (REQUIRED)

### Requirements

**Decision Variables**: 3-7 recommended
- What the stakeholder is deciding
- Examples: product quantities, resource allocations, service levels

**Objective Function**: Maximize or Minimize
- What to optimize: profit, cost, revenue, throughput, etc.
- Each decision variable has an objective coefficient

**Constraints**: 4-8 recommended
- Budget limits
- Capacity constraints
- Resource availability
- Minimum/maximum requirements
- **Must include 2-3 binding constraints** for sensitivity analysis

### CRITICAL: Linearity Requirements

**MUST be solvable with Simplex LP method**:
- ✅ Linear objective function: `5x₁ + 3x₂ + 7x₃`
- ✅ Linear constraints: `2x₁ + 4x₂ ≤ 100`
- ❌ NO exponents: `x₁²` or `x₁³`
- ❌ NO products of variables: `x₁ × x₂`
- ❌ NO division of variables: `x₁ / x₂`
- ✅ All coefficients must be constants, not variables

### Data Format Options

Generate data in **BOTH formats**:

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
   - Rows: Constraints
   - Columns: Decision Variables
   - Cell values: Usage coefficients
   - Example: Product A uses 2 machine hours/unit

**Option 2: Raw Parameter Data** (Students organize themselves)

Provide the same information as text/lists:
- List of decision variable options with descriptions
- Objective coefficients for each variable
- List of constraints with limits and types
- Resource consumption rates for each variable-constraint combination
- Students structure the LP model themselves

### Quality Assurance Checklist

Before providing LP data:
- [ ] Problem is LINEAR (no x², no x₁×x₂, constants only)
- [ ] Feasible solution exists (test in Solver)
- [ ] Optimal solution is NOT obvious (requires Solver to find)
- [ ] 2-3 constraints are binding at optimum (for sensitivity analysis)
- [ ] Realistic business context (production, resource allocation, etc.)
- [ ] Both format options provided (pre-formatted + raw)
- [ ] All parameters clearly labeled with units

### Key Questions to Ask Students

Ask sequentially (ONE at a time):
1. **Business Context**: "What business problem are you solving? (production planning, resource allocation, product mix, etc.)"
2. **Objective Function**: "What are you trying to maximize or minimize? (profit, cost, revenue, throughput, etc.)"
3. **Decision Variables**: "What are you deciding? (How many units to produce? How to allocate resources?)"
4. **Constraints**: "What are the limiting factors? (budget, machine hours, labor hours, materials, minimum requirements)"

### Analysis Requirements

Students must:
- Set up LP model in Excel with decision variables
- Define objective function with coefficients
- Add all constraints to Solver
- Use Simplex LP method to find optimal solution
- Interpret results:
  - Optimal values for each decision variable
  - Optimal objective function value
- Perform sensitivity analysis:
  - Shadow prices (value of additional resources)
  - Binding vs non-binding constraints
  - Allowable increases/decreases

## Problem B: Student Choice (ONE of Four Methods)

### Method 1: Inventory Management (EOQ)

**Purpose**: Optimize inventory decisions using Economic Order Quantity model

**Parameters Required**:
- Annual demand (units/year)
- Ordering cost per order ($)
- Holding cost per unit per year ($ or % of unit cost)
- Unit cost ($)
- Lead time (days)
- Optional: Quantity discount breakpoints

**Analysis Requirements**:
- Calculate Economic Order Quantity
- Determine reorder point
- Calculate total inventory costs (ordering + holding)
- Analyze trade-offs
- Optional: Evaluate quantity discounts

**Key Questions** (ONE at a time):
1. "What are you managing inventory for? (raw materials, finished goods, spare parts)"
2. "What's the annual demand volume?"
3. "What are the ordering costs and holding costs?"
4. "What's the lead time for replenishment?"

### Method 2: Aggregate Planning

**Purpose**: Develop production plan matching supply with demand over planning horizon

**Parameters Required** (6-12 periods):
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

**Analysis Requirements**:
- Develop production plan over planning horizon
- Balance capacity, costs, and demand
- Consider regular time, overtime, subcontracting, inventory
- Minimize total costs
- Evaluate trade-offs between strategies

**Key Questions** (ONE at a time):
1. "How many periods (months) should the plan cover? (6-12 recommended)"
2. "What's the demand pattern? (seasonal, growing, stable)"
3. "What production flexibility exists? (overtime, subcontracting, inventory)"
4. "Can workforce size change? (hiring/firing allowed?)"

### Method 3: Location Strategy (Factor Rating)

**Purpose**: Select optimal facility location using Factor Rating Method

**Parameters Required**:
- 3-5 location alternatives
- 5-8 factors to evaluate:
  - Cost-related (labor costs, facility costs, transportation)
  - Operational (proximity to markets, supplier access, infrastructure)
  - Strategic (skilled labor availability, quality of life, business climate)
- Factor weights (importance ratings, must sum to 1.0 or 100)
- Location scores for each factor (0-100 scale)

**Analysis Requirements**:
- Evaluate location alternatives using weighted factors
- Calculate weighted scores for each location
- Recommend optimal location
- Analyze sensitivity to factor weights

**Key Questions** (ONE at a time):
1. "What type of facility? (warehouse, manufacturing plant, distribution center, retail store)"
2. "How many location alternatives to compare? (3-5 recommended)"
3. "What factors matter most? (costs, proximity, labor, infrastructure)"
4. "How important is each factor relative to others?"

**Quality Assurance**:
- Factor weights must sum to 1.0 (or 100)
- Scores on consistent 0-100 scale
- Create realistic trade-offs (no location dominates all factors)
- Winning location should be clear but not overwhelming

### Method 4: Capacity & Constraint Management

**Purpose**: Identify bottlenecks, calculate system capacity, analyze constraint impacts

**Parameters Required**:
- 4-6 process steps (sequential or parallel)
- Processing time per unit at each step (minutes/unit or units/hour)
- Available time per step (hours/day or hours/week)
- Step capacity (units/hour or units/day)
- Demand requirement (units needed)
- Optional: Setup times, worker requirements, cost data, quality/defect rates

**Analysis Requirements**:
- Identify process bottleneck
- Calculate system capacity and throughput
- Analyze constraint impacts
- Recommend constraint management strategies
- Evaluate impact of constraint improvements

**Key Questions** (ONE at a time):
1. "What process are you analyzing? (manufacturing line, service delivery, order fulfillment)"
2. "How many steps in the process? (4-6 recommended)"
3. "What's the suspected bottleneck or capacity issue?"
4. "What's the demand requirement vs current capacity?"

**Quality Assurance**:
- Create clear bottleneck (one step with lowest capacity)
- System capacity should be less than demand (creates meaningful problem)
- Make constraint analysis impactful (bottleneck significantly limits throughput)
- Include realistic business context

## Data Format for All Problem B Methods

Generate data in **BOTH formats**:

**Option 1: Pre-Formatted Excel Tables**
- Method-specific tables organized and labeled
- Ready for calculations
- Clear structure for analysis

**Option 2: Raw Parameter Lists**
- Same information as text/lists
- Students organize and structure themselves
- Builds modeling skills

## Deliverables

Students submit:
1. **Problem A workbook** with LP analysis:
   - Pre-formatted parameter tables OR raw parameters (student's choice)
   - Solver setup and solution
   - Sensitivity analysis
2. **Problem B workbook** with chosen method analysis:
   - Pre-formatted tables OR raw parameters (student's choice)
   - Method-specific calculations
   - Recommendations
3. **Data dictionary** explaining all parameters
4. **README** with both problems explained, decision area connection, and analysis guidance

## Generation Guidelines

### General Approach
1. **Ask which Problem B method** student wants (Inventory/Aggregate/Location/Capacity)
2. **Generate Problem A (LP)** with BOTH format options
3. **Generate Problem B** specific to chosen method with BOTH format options
4. **Provide CLEAN data** (parameter data focus, not data cleaning)
5. **Create comprehensive documentation** (data dictionary + README)

### Quality Checks
- [ ] Problem A is LINEAR (Simplex LP compatible)
- [ ] Problem A feasible solution exists (tested)
- [ ] Problem A has 2-3 binding constraints
- [ ] Problem B method matches student's choice
- [ ] Both problems have BOTH format options (pre-formatted + raw)
- [ ] All parameters clearly labeled with units
- [ ] README explains both problems and decision area connection
- [ ] Data dictionary defines all parameters

### Documentation Requirements
- README must explain BOTH problems
- Connect both problems to Operations Management Decision Area
- Provide analysis guidance for both LP and chosen Problem B method
- Explain DC ACT Framework application
- Include interview preparation guidance
