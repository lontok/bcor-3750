## **Final Interview Study Guide**

**Overall Grade %:** 25 
**Total Points:** 100 (Make every effort to attempt all questions for partial credit) 
**Total Time:** 20 minutes + 5-minute debrief (for feedback) 
**Location:** In person, Hilton 114 
**Scheduling:** [https://calendly.com/greg-lontok/3750-final-interview](https://calendly.com/greg-lontok/3750-final-interview) 
Schedule a 25-minute interview between Monday, December 8, and Thursday, December 11, 2025. 

The final interview assesses your understanding of **Predictive Analytics (Milestone 2)** and **Prescriptive Analytics (Milestone 3)**. Your project serves as the primary case study. If you've completed Milestones 2 and 3, you already have everything you need.

This guide helps you organize your work into a confident, 20-minute interview conversation.

**Key Success Factors:**
- **Information dense**: Every sentence should carry weight
- **Succinct delivery**: No rambling—use IRPM structure
- **Practice, practice, practice**: The more you rehearse, the more confident you'll be

---

### **Rubric**

What is the interviewer trying to assess?

1. Can you explain WHY you made analytical choices and defend your methodology?
2. Do you understand what your numbers mean and can you explain them in business terms?
3. How well do you connect analysis to business problems with realistic, actionable recommendations?
4. **Can I trust you to confidently present predictive insights and optimization recommendations to stakeholders?**

| Grade | Criteria |
| :---: | ----- |
| A | Exceptional - Clear mastery of predictive and prescriptive analytics, strong business insight, technical depth, and confident communication. Ready to lead data-driven decision-making. "I'm impressed. Let's hire this candidate." |
| B | Strong - Meets all core requirements and shows solid understanding. Minor gaps in explanation or connection to business context. "Good candidate, would bring back for another interview." |
| C | Adequate - Satisfies basic criteria but displays uneven understanding. Can perform analysis but struggles to explain or connect to business value. "Has potential but needs more development." |
| D, F | Underperforming - Fell significantly short of expectations. Cannot explain own analysis or connect to stakeholder needs. "Not ready for this role." |

---

### **Point Distribution**

| Category | Points | Description |
|----------|--------|-------------|
| Whiteboard & Analytical Flow | 15 | Effective visual storytelling demonstrating analytical progression |
| "Tell Me About Yourself" + Segue | 10 | Professional intro with seamless project connection |
| Predictive Analytics (M2) | 30 | Time Series (15) + Regression (15) with IRPM |
| Prescriptive Analytics (M3) | 30 | Linear Programming (15) + Problem B (15) with IRPM |
| Communication & Follow-up Questions | 15 | Clarity, confidence, handling probing questions |
| **Total** | **100** | |

---

### **Structure and Timing**

**Total Time: 20 minutes**

| Section | Time | Content |
|---------|------|---------|
| "Tell me about yourself" | 2 min | Professional intro + project segue |
| Context/Whiteboard Setup | 1 min | Job, stakeholder, draw roadmap |
| **Milestone 2: Predictive** | **8 min** | |
| → Time Series Forecasting | 4 min | Decomposition → Model Comparison → Forecast (IRPM) |
| → Regression Analysis | 4 min | Correlation → Model Comparison → Scenarios (IRPM) |
| **Milestone 3: Prescriptive** | **8 min** | |
| → Linear Programming | 4 min | Model Setup → Solver Output → Sensitivity (IRPM) |
| → Problem B | 4 min | Method → Analysis → Recommendation (IRPM) |
| Follow-up Questions | 1 min | Discussion and clarification |

---

### **Interview Questions**

1. **"Tell me about yourself."** (2 minutes | 10 points)

   **IMPORTANT:** Assume the interviewer does NOT know you. This mirrors real-world interviews where you always start fresh—even if you've met the interviewer before.

   Structure your response around:
   1. Education
   2. Extracurricular activities or a side project that shows initiative
   3. Relevant work or internship history
   4. Personal tidbit (human connection)
   5. **Seamless segue into your project (critical—don't skip this!)**

2. **"Tell me more about your project."** (17 minutes | 75 points)

   Use the whiteboard to guide your presentation. Draw as you speak.

---

### **Whiteboard Roadmap (Required - 15 points)**

You MUST use the whiteboard to visually guide your presentation. Draw the roadmap as you present—this demonstrates mastery of your material and helps the interviewer follow your analytical story.

**Choose vertical OR horizontal orientation based on your preference.**

#### **Vertical Flow Option:**
```
[Job Title] → [Stakeholder] → [Problem]
                    ↓
         ══════════════════════
            PREDICTIVE (M2)
          "What will happen?"
         ══════════════════════
                    ↓
         Forecast        Drivers
        (Time Series)  (Regression)
                    ↓
         ══════════════════════
           PRESCRIPTIVE (M3)
         "What should we do?"
         ══════════════════════
                    ↓
          Optimize      [Method B]
            (LP)       (EOQ/Agg/Loc/Cap)
                    ↓
         ══════════════════════
              IMPACT
           [Quantified Result]
         ══════════════════════
```

#### **Horizontal Flow Option:**
```
[Job/Stakeholder/Problem] → PREDICTIVE (M2) → PRESCRIPTIVE (M3) → IMPACT
                            "What will happen?"  "What should we do?"
                                   ↓                    ↓
                           Time Series  Regression   LP    [Method B]
```

**Key Points:**
- Draw as you speak (builds engagement, shows mastery)
- Add 2-3 specific figures to each box as you discuss it
- Use the whiteboard as your navigation tool throughout
- Point to sections as you transition between topics

---

### **IRPM Framework (Required for All 4 Analysis Components)**

Use IRPM for EVERY analysis component. This structure ensures you're information dense yet succinct.

**Note:** Cover Method at a high level, but be prepared to answer detailed questions when asked.

```
┌─────────────────────────────────────────────────────────────┐
│ I - INSIGHT: What did you discover?                         │
│     → The data-driven finding or pattern (with numbers)     │
│                                                              │
│ R - RECOMMENDATION: What should stakeholder do?             │
│     → Specific, actionable advice based on the insight      │
│                                                              │
│ P - PREDICTION: What outcome do you expect?                 │
│     → Quantifiable result if recommendation is followed     │
│                                                              │
│ M - METHOD: How did you analyze the data?                   │
│     → Key steps, Excel functions/tools, reasoning           │
└─────────────────────────────────────────────────────────────┘
```

**Total IRPM Cycles: 4**
1. Time Series Forecasting
2. Multiple Linear Regression
3. Linear Programming
4. Problem B (EOQ / Aggregate Planning / Factor Rating / Capacity)

---

### **Content Coverage by Section**

#### **MILESTONE 2: PREDICTIVE ANALYTICS (8 minutes)**

**Time Series Forecasting (4 minutes) - IRPM Required**

Cover these key components with 2-3 specific figures:

| Component | What to Mention | Example Figures |
|-----------|-----------------|-----------------|
| **Decomposition** | Patterns identified (trend, seasonal, cyclic, random) | "Strong upward trend of 5% monthly growth, seasonal peaks in Q4" |
| **Model Comparison** | Models tested and accuracy measures | "Tested 3-month MA, 6-month MA, FORECAST.ETS; ETS had lowest MAPE at 8.2%" |
| **Best Model & Forecast** | Selected model and ONE period forecast | "ETS forecasts 1,250 units for January, 18% above current capacity" |

**IRPM Example - Time Series:**
> **Insight**: "FORECAST.ETS achieved the lowest error rate at 8.2% MAPE, outperforming moving average methods because it captures both the upward trend and Q4 seasonality in our order data."
>
> **Recommendation**: "I recommend the stakeholder use FORECAST.ETS for monthly demand planning and increase warehouse capacity by 20% before Q4."
>
> **Prediction**: "If we expand capacity as recommended, we can meet the forecasted 1,250 unit demand in January without stockouts, potentially increasing revenue by $45,000."
>
> **Method**: "I tested three forecasting models using 24 months of historical data, calculated MAD, MSE, and MAPE for each, and selected the model with the lowest error rate."

---

**Multiple Linear Regression (4 minutes) - IRPM Required**

Cover these key components with 2-3 specific figures:

| Component | What to Mention | Example Figures |
|-----------|-----------------|-----------------|
| **Correlation Analysis** | Key relationships identified | "Distance (r=0.82) and Weight (r=0.71) showed strongest correlation with delivery time" |
| **Model Comparison** | Models tested and fit statistics | "2-variable model: Adj R²=0.74; 3-variable model: Adj R²=0.81" |
| **Coefficients & Scenarios** | What drives the outcome, predictions | "Each additional mile adds 0.12 days; Peak scenario predicts 6.2-day delivery" |

**IRPM Example - Regression:**
> **Insight**: "The 3-variable model explains 81% of delivery time variation. Distance is the strongest driver—each additional mile adds 0.12 days to delivery time, while package weight adds 0.05 days per pound."
>
> **Recommendation**: "I recommend the stakeholder prioritize shipments from the closest distribution center and consolidate heavy packages into fewer, larger shipments."
>
> **Prediction**: "Implementing proximity-based routing could reduce average delivery time from 5.2 days to 4.1 days, meeting our 4-day target."
>
> **Method**: "I built a correlation matrix, created scatter plots for the top 3 variables, tested two regression models with different variable combinations, and validated statistical significance using p-values."

---

#### **MILESTONE 3: PRESCRIPTIVE ANALYTICS (8 minutes)**

**Linear Programming (4 minutes) - IRPM Required**

Cover these key components with 2-3 specific figures:

| Component | What to Mention | Example Figures |
|-----------|-----------------|-----------------|
| **Model Setup** | Objective, decision variables, constraints | "Maximize profit; 3 products (A, B, C); 4 constraints (machine hrs, labor, materials, demand)" |
| **Solver Output** | Optimal solution values | "Produce 150A, 200B, 100C for maximum profit of $45,000" |
| **Sensitivity Analysis** | Binding constraints, shadow prices | "Machine hours binding—shadow price $45/hr; adding 10 hours increases profit by $450" |

**IRPM Example - Linear Programming:**
> **Insight**: "The optimal product mix is 150 units of A, 200 units of B, and 100 units of C, generating $45,000 in profit. Machine hours are the binding constraint with a shadow price of $45 per hour."
>
> **Recommendation**: "I recommend the stakeholder invest in additional machine capacity. Each additional machine hour is worth $45 in profit, up to 50 additional hours."
>
> **Prediction**: "Adding 50 machine hours would increase monthly profit by $2,250, a 5% improvement with minimal capital investment."
>
> **Method**: "I formulated the LP model in Excel with decision variables, objective function, and constraints, then used Solver with Simplex LP to find the optimal solution and generated the Sensitivity Report."

---

**Problem B - Choose ONE Method (4 minutes) - IRPM Required**

Cover the key components for YOUR chosen method:

**If EOQ (Inventory Management):**
| Component | What to Mention | Example Figures |
|-----------|-----------------|-----------------|
| **EOQ Calculation** | Optimal order quantity | "EOQ = 800 units per order" |
| **Reorder Point & Safety Stock** | When to order | "Reorder at 200 units; safety stock of 50 units" |
| **Total Cost** | Annual ordering + holding costs | "Total annual cost: $12,400 (vs. current $18,000)" |

**If Aggregate Planning:**
| Component | What to Mention | Example Figures |
|-----------|-----------------|-----------------|
| **Strategy Comparison** | Level vs. Chase vs. Mixed | "Level strategy: $425K; Chase strategy: $380K" |
| **Workforce/Production Plan** | Key decisions by period | "Hire 5 workers in March, produce 1,200 units/month" |
| **Total Cost** | All cost components | "Chase saves $45K annually but requires flexible workforce" |

**If Factor Rating (Location Strategy):**
| Component | What to Mention | Example Figures |
|-----------|-----------------|-----------------|
| **Factors & Weights** | Critical factors identified | "Labor (0.35), Transportation (0.25), Cost (0.20), Quality of Life (0.20)" |
| **Location Scores** | Weighted scores by location | "Location A: 82; Location B: 76; Location C: 71" |
| **Recommendation** | Best location and why | "Location A wins due to superior labor availability score (95/100)" |

**If Capacity & Constraint Management:**
| Component | What to Mention | Example Figures |
|-----------|-----------------|-----------------|
| **Capacity Metrics** | Utilization, efficiency | "Current utilization: 78%; Efficiency: 85%" |
| **Bottleneck Analysis** | Constraint identification | "Assembly station is bottleneck at 95% utilization" |
| **Break-even/Throughput** | Key calculations | "Break-even at 850 units; current throughput: 920 units" |

---

### **Sample Interview Question Bank**

Practice answering these questions about YOUR specific project:

#### **Opening & Context Questions**
- "Tell me about yourself." (Practice the segue!)
- "Why did you choose this job/company/stakeholder?"
- "How do Milestones 2 and 3 connect to your Milestone 1 findings?"
- "What business problem are you ultimately trying to solve?"

#### **Time Series Forecasting Questions**
- "What patterns did you identify in your time series data?"
- "Why did you choose [X] periods for your moving average?"
- "Explain why [forecasting method] worked better than the others."
- "How confident are you in your forecast? What could go wrong?"
- "What would happen to your forecast if the seasonal pattern changed?"
- "How would you know if your forecast is accurate after implementation?"
- "What's the difference between MAD, MSE, and MAPE? Why did you focus on [one]?"

#### **Regression Analysis Questions**
- "Walk me through your correlation analysis. What did you find?"
- "What does a coefficient of [X] mean in plain English?"
- "Why didn't you include [variable] in your final model?"
- "What does an Adjusted R² of [X] mean? Is that good?"
- "How do you know your variables are statistically significant?"
- "If [independent variable] increased by 10%, what happens to [dependent variable]?"
- "What are the limitations of your regression model?"
- "Why did you choose the 3-variable model over the 2-variable model?" (or vice versa)

#### **Linear Programming Questions**
- "Walk me through your optimization model setup."
- "What are you maximizing/minimizing and why?"
- "Explain your constraints. Why do they matter?"
- "What does the sensitivity analysis tell you?"
- "Which constraint is binding? What does that mean for the business?"
- "What's a shadow price and why should the stakeholder care?"
- "What would happen if you relaxed [constraint] by 10%?"
- "How did you validate that your solution is optimal?"

#### **Problem B Questions (Method-Specific)**

*EOQ/Inventory:*
- "Walk me through your EOQ calculation."
- "How did you determine the holding cost percentage?"
- "What happens if demand variability increases?"
- "Why is this reorder point appropriate?"

*Aggregate Planning:*
- "Why did you choose [Level/Chase/Mixed] strategy?"
- "What are the trade-offs between strategies?"
- "How did you calculate overtime/hiring/layoff costs?"
- "What assumptions did you make about workforce flexibility?"

*Factor Rating:*
- "How did you determine the factor weights?"
- "Which factor had the biggest impact on your recommendation?"
- "What if the stakeholder valued [factor] more heavily?"
- "How did you normalize the quantitative factors?"

*Capacity:*
- "How did you identify the bottleneck?"
- "What's the difference between utilization and efficiency?"
- "What would it take to increase throughput by 20%?"
- "Walk me through your break-even analysis."

#### **Synthesis & Business Impact Questions**
- "How did your descriptive findings inform your predictive model?"
- "How do your M2 predictions connect to your M3 optimization?"
- "Looking across all analytics types, what's the complete story?"
- "If your stakeholder could only implement ONE recommendation, which would you prioritize?"
- "What's the total business impact of your recommendations?"
- "What are the risks if the stakeholder doesn't act on your analysis?"

#### **Challenge Questions (Expect These!)**
- "What would you do differently if you started over?"
- "What are the limitations of your analysis?"
- "How would you validate your recommendations before full implementation?"
- "What data would you want that you didn't have?"
- "Why should the stakeholder trust your predictions?"
- "What's the biggest assumption in your analysis?"

#### **Depth Questions**
- "Why?" (about any decision you made)
- "Can you elaborate on that?"
- "What would happen if [different scenario]?"
- "How did you arrive at that conclusion?"
- "Can you show me that on the whiteboard?"

---

### **Common Mistakes to Avoid**

#### **Content Mistakes**
- Skipping the project segue in "Tell me about yourself"
- Not using the whiteboard (15-point deduction!)
- Confusing R² with Adjusted R² (Adjusted R² accounts for number of variables)
- Not understanding what regression coefficients mean in business terms
- Jumping to LP solution without explaining model setup (objective, variables, constraints)
- Not knowing what shadow prices mean or why they matter
- Forgetting to mention binding vs. non-binding constraints
- Unable to explain why you chose your Problem B method
- Not connecting analysis back to stakeholder's problem

#### **Technical Mistakes**
- Can't explain the difference between forecasting methods
- Confusing correlation with causation in regression
- Not knowing which constraints are binding in your LP
- Unable to interpret sensitivity report allowable ranges
- Mixing up decision variables and parameters in LP
- Not remembering your own numbers (practice with your slides!)

#### **Communication Mistakes**
- Rambling without structure (use IRPM!)
- Using technical jargon without explaining it
- Not making eye contact (facing the whiteboard the whole time)
- Speaking too fast or too slow
- Not listening to follow-up questions before answering
- Giving vague answers instead of specific numbers

#### **Timing Mistakes**
- Spending 5+ minutes on "Tell me about yourself"
- Rushing through one milestone to spend more time on the other
- Not practicing with a timer beforehand
- Trying to cover everything instead of hitting key points with IRPM
- Running out of time before discussing business impact

#### **Quick Fixes**
- Practice the 20-minute structure with a timer multiple times
- Know your key numbers cold (memorize 2-3 figures per section)
- Prepare to answer "Why?" for every analytical decision
- Use IRPM framework consistently—it keeps you structured and succinct
- Practice drawing the whiteboard roadmap until it's automatic

---

### **Study Materials**

**High Priority:**
- **Your Milestone 2 Slides** - Know every chart, every number, every insight
- **Your Milestone 3 Slides** - Know every chart, every number, every insight
- **Your Excel Workbooks** - Be able to explain any formula or calculation

**Standard Resources:**
- Lesson Exercises
- Lesson Slides
- Zoom Recordings
- Zoom AI Companion Meeting Summaries
- Supplement with YouTube, [O'Reilly resources](https://go.oreilly.com/loyola-marymount), online tutorials

---

### **Study Tips**

#### **Practice with a Classmate** (Most Effective)
- **Setup** (5 min): Exchange Milestone 2-3 slides, review each other's projects
- **Interview** (25 min): One person presents (20 min) + feedback (5 min)
- **Switch** (25 min): Other person presents (20 min) + feedback (5 min)
- **Debrief** (10 min): Discuss what worked, what needs improvement

**During Partner's Interview:**
- Use timing breakdown to give time checks ("4 minutes left for M2")
- Ask "Why?" follow-up questions when they finish each IRPM cycle
- Note where they hesitated or couldn't explain their numbers
- Check if they used IRPM framework for all 4 components
- Verify they used the whiteboard effectively

**Giving Feedback** (Use the Rubric):
- What worked well: Specific strengths you observed
- What needs work: 2-3 specific improvement areas
- One thing to practice: Most critical item before interview
- Rubric estimate: Where would they fall (A/B/C/D)?

#### **Practice with AI** - BCOR 3750 Final Interview Coach
- **Use Voice Mode** (sound wave icon) for most realistic practice
- Upload your Milestone 2 AND Milestone 3 slides for personalized questions
- Choose difficulty: Practice (gentler), Realistic (standard), or Challenging (deep drilling)
- Get honest feedback on all rubric dimensions
- IRPM framework validation—coach flags missing elements
- Whiteboard guidance—coach prompts you to describe your visual roadmap

**Conversation Starters:**
- "I want to practice the full 20-minute interview"
- "Help me prepare my 'Tell me about yourself' with project segue"
- "Practice Milestone 2 (Predictive) only"
- "Practice Milestone 3 (Prescriptive) only"
- "Quiz me on Time Series Forecasting"
- "Quiz me on Regression Analysis"
- "Quiz me on Linear Programming"
- "Quiz me on [EOQ/Aggregate Planning/Factor Rating/Capacity]"
- "Ask me challenging 'Why?' questions"

#### **Practice with Yourself**
- Record yourself presenting (video preferred, audio minimum)
- Time each section to hit the timing breakdown
- Draw the whiteboard roadmap from memory without notes
- Watch/listen back and identify where you hesitated
- Re-record until you can present smoothly within 20 minutes

#### **Whiteboard Practice**
- Draw the roadmap template from memory on paper/whiteboard
- Time yourself—can you draw it in under 30 seconds?
- Practice adding 2-3 figures to each box as you discuss it
- Practice pointing to sections as you talk
- Ensure you can draw while maintaining some eye contact

#### **Number Memorization**
For each of your 4 IRPM sections, memorize:
- 2-3 key figures (e.g., "MAPE of 8.2%", "Adj R² of 0.81", "Shadow price of $45")
- The "so what" business implication of each figure
- Practice saying them out loud until automatic

---

### **Quick Reference Card**

Print or write this on a notecard for last-minute review:

```
┌─────────────────────────────────────────────────────┐
│ FINAL INTERVIEW CHECKLIST                           │
├─────────────────────────────────────────────────────┤
│ ☐ Tell me about yourself (2 min) + PROJECT SEGUE   │
│ ☐ WHITEBOARD: Draw roadmap as you present          │
│ ☐ Context: Job → Stakeholder → Problem             │
│                                                     │
│ MILESTONE 2 - PREDICTIVE (8 min)                   │
│ ☐ Time Series: Decomposition → Models → Forecast   │
│ ☐ Regression: Correlation → Models → Scenarios     │
│                                                     │
│ MILESTONE 3 - PRESCRIPTIVE (8 min)                 │
│ ☐ LP: Model Setup → Solver → Sensitivity           │
│ ☐ Problem B: Method → Analysis → Recommendation    │
│                                                     │
│ IRPM EVERY TIME (4 cycles total):                  │
│ I - Insight (what I found + specific numbers)      │
│ R - Recommendation (what stakeholder should do)    │
│ P - Prediction (expected outcome with numbers)     │
│ M - Method (how I analyzed—tools & approach)       │
│                                                     │
│ KEY NUMBERS TO MEMORIZE:                           │
│ • Time Series: _______ (e.g., MAPE, forecast)     │
│ • Regression: _______ (e.g., Adj R², coefficient) │
│ • LP: _______ (e.g., optimal value, shadow price) │
│ • Problem B: _______ (e.g., EOQ, total cost)      │
│                                                     │
│ DON'T FORGET:                                       │
│ ✓ Assume interviewer doesn't know you              │
│ ✓ Use whiteboard (15 points!)                      │
│ ✓ 2-3 specific figures per section                 │
│ ✓ Connect everything to stakeholder's problem      │
│ ✓ Be ready to answer "Why?" for every decision    │
└─────────────────────────────────────────────────────┘
```

---

### **Last Tips**

- Get a good night's sleep.
- Take a deep breath if you get nervous.
- Don't be afraid to ask for clarification.
- If you don't know something, describe how you would find the answer.
- It's okay to pause and think before responding.

You already did the hard work—the forecasting, the regression, the optimization. This interview is your chance to own your work, explain it like a professional, and show how much you've learned.

**You've progressed through the entire analytics maturity scale:**
- Descriptive: What happened?
- Diagnostic: Why did it happen?
- Predictive: What will happen?
- Prescriptive: What should we do?

Now tell that complete story with confidence. You've got this.
