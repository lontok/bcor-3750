# Data Craft Custom GPT - Optimized Configuration

## 📋 Overview

This folder contains the optimized configuration for the **Data Craft** Custom GPT, redesigned using **Anthropic's Effective Context Engineering Principles** to reduce token usage by 95% while maintaining (and improving) effectiveness.

## 🎯 Optimization Results

| Metric | Before | After | Improvement |
|--------|--------|-------|-------------|
| **Instructions Length** | 771 lines | 150 lines | **80% reduction** |
| **Context Tokens** | ~50,000 chars | ~2,500 chars | **95% reduction** |
| **Knowledge Structure** | All embedded | 4 external files | Retrievable on-demand |
| **Maintainability** | Difficult | Easy | Update specific files |
| **User Experience** | Generic entry | Milestone-specific | Better guidance |

## 📁 Files in This Folder

### Core Configuration Files

1. **`instructions.md`**
   - Core GPT instructions for the Instructions field
   - ~150 lines, ~2,500 characters
   - Focuses on behavior, interaction flow, and references to knowledge base

2. **`ui-configuration.md`**
   - Complete setup guide for Custom GPT UI
   - Description, conversation starters, implementation steps
   - Testing checklist and troubleshooting

### Knowledge Base Files (Upload to GPT)

3. **`ops-decision-areas-reference.md`**
   - 10 Operations Management Decision Areas
   - Example problems, metrics, and scenarios by area
   - Retrieved when student selects decision area

4. **`analytics-type-specifications.md`**
   - Detailed specs for Descriptive, Diagnostic, Predictive, Prescriptive analytics
   - Data structure requirements and key questions
   - Retrieved based on milestone/analytics type

5. **`output-templates-and-formats.md`**
   - Data dictionary format
   - README structure template
   - Final confirmation checklist and delivery messaging

6. **`milestone-requirements-summary.md`**
   - Milestone 1, 2, 3 specific requirements
   - What students need for each milestone
   - Interview preparation guidance

## 🚀 Quick Start Implementation

### Step 1: Open Custom GPT Configuration
1. Go to https://chat.openai.com/
2. Navigate to your existing "Data Craft" GPT or create new
3. Click "Configure" tab

### Step 2: Update Instructions
1. Open `instructions.md`
2. Copy ENTIRE content
3. Paste into "Instructions" field
4. Verify no truncation

### Step 3: Update Description & Starters
1. Set Description: "I help you create realistic operational datasets for analytics projects based on your job description and business problem."
2. Add 4 conversation starters from `ui-configuration.md`

### Step 4: Upload Knowledge Files
Upload these 4 files to Knowledge section:
- `ops-decision-areas-reference.md`
- `analytics-type-specifications.md`
- `output-templates-and-formats.md`
- `milestone-requirements-summary.md`

### Step 5: Verify & Test
1. Ensure GPT-5 is selected as model
2. Save configuration
3. Test with conversation starters
4. Verify ONE question at a time behavior

## ✅ Key Improvements Based on Anthropic Principles

### 1. "Smallest Set of High-Signal Tokens"
- ✅ Reduced instructions from 771 to 150 lines
- ✅ Core behavior only in main prompt
- ✅ Detailed specs moved to retrievable knowledge files

### 2. "Right Altitude" Language
- ✅ Clear heuristics instead of exhaustive rules
- ✅ Adaptive guidance: "Suggest 2-3 based on context"
- ✅ Trust GPT-5 to infer and adapt

### 3. "Avoid Laundry List of Edge Cases"
- ✅ Removed exhaustive if-then scenarios
- ✅ Replaced with high-level guidance + external reference
- ✅ Let model handle variations intelligently

### 4. "Use Structured Sections"
- ✅ Clear delineation: `<core_identity>`, `<interaction_flow>`, `<technical_essentials>`
- ✅ Organized knowledge files by purpose
- ✅ Easy to navigate and understand

### 5. "Sub-Agent Architecture"
- ✅ Main instructions = core behavior
- ✅ Knowledge files = specialized reference content
- ✅ Retrieved on-demand, not loaded upfront

## 🎓 How It Works

### The "ONE Question at a Time" Principle

The optimized GPT follows a Socratic questioning approach:

1. **Phase 1: Context Discovery**
   - Ask about job/industry/company (one question at a time)
   - Retrieve relevant decision area details when selected

2. **Phase 2: Problem Definition**
   - Ask about stakeholder, problem, milestone (sequentially)
   - Adapt based on responses

3. **Phase 3: Data Requirements**
   - Based on milestone, ask targeted questions
   - Retrieve detailed specs from knowledge files

4. **Phase 4: Generation & Delivery**
   - Confirm specifications
   - Generate dataset with intentional quality issues
   - Provide formatted deliverables

### Knowledge Retrieval Strategy

The GPT references knowledge files when:
- Student selects a decision area → Retrieve `ops-decision-areas-reference.md`
- Student indicates milestone → Retrieve `analytics-type-specifications.md`
- Time to generate outputs → Retrieve `output-templates-and-formats.md`
- Need milestone context → Retrieve `milestone-requirements-summary.md`

## 🔧 Maintenance & Updates

### To Update Decision Areas
1. Edit `ops-decision-areas-reference.md`
2. Re-upload to GPT Knowledge section
3. No changes needed to main instructions

### To Update Analytics Specs
1. Edit `analytics-type-specifications.md`
2. Re-upload to GPT Knowledge section
3. No changes needed to main instructions

### To Update Templates
1. Edit `output-templates-and-formats.md`
2. Re-upload to GPT Knowledge section
3. No changes needed to main instructions

### To Update Core Behavior
1. Edit `instructions.md`
2. Copy/paste into GPT Instructions field
3. Knowledge files remain unchanged

## 📊 Student Experience Improvements

### Before
- Generic "Create a dataset" entry point
- All questions shown at once (overwhelming)
- Difficult to know where to start

### After
- 4 milestone-specific conversation starters
- ONE question at a time (progressive discovery)
- Clear guidance based on context

### Conversation Flow Example

**Student**: "I need data for Milestone 1"

**GPT**: "Let's start by understanding your professional context. Please upload:
1. Your resume (optional but helpful)
2. The job description for the operations/supply chain role you're targeting"

*(waits for response)*

**Student**: *uploads job description*

**GPT**: "What industry or sector is the company in? (e.g., e-commerce, manufacturing, retail, healthcare)"

*(continues ONE question at a time)*

## 🧪 Testing & Validation

### Test Scenarios

1. **Milestone 1 Entry**
   - Start: "I need data for Milestone 1"
   - Verify: Asks about descriptive/diagnostic context
   - Verify: ONE question at a time

2. **Milestone 2 Entry**
   - Start: "I need data for Milestone 2"
   - Verify: Asks about forecasting OR regression
   - Verify: References time series specs from knowledge

3. **Milestone 3 Entry**
   - Start: "I need data for Milestone 3"
   - Verify: Asks about optimization OR simulation
   - Verify: Provides appropriate parameter questions

4. **Decision Area Selection**
   - When student selects "Supply Chain Management"
   - Verify: Retrieves 2-3 relevant problems from knowledge file
   - Verify: Doesn't list all 10 areas upfront

## 📚 Additional Resources

- **Original Prompt**: `../custom-gpt-update-guide.md` (771 lines)
- **Anthropic Article**: https://www.anthropic.com/engineering/effective-context-engineering-for-ai-agents
- **Project Requirements**: `../project/project-requirements.md`
- **Milestone Details**: `../project/milestones-2-3-details.md`

## 🤝 Support

If you encounter issues:
1. Check `ui-configuration.md` troubleshooting section
2. Verify all knowledge files are uploaded
3. Test with specific conversation starters
4. Ensure GPT-5 model is selected

## 📝 Version History

- **v1.0** (Current): Optimized using Anthropic principles
  - 95% token reduction
  - Knowledge-based architecture
  - Milestone-specific entry points

- **v0.x** (Previous): Original monolithic prompt
  - 771 lines embedded in instructions
  - Generic conversation starters

---

**Created**: January 2025
**Optimized Using**: Anthropic's Effective Context Engineering for AI Agents
**For**: BCOR 3750 Analytics Project
