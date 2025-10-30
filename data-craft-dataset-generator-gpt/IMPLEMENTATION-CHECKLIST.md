# Data Craft GPT - Implementation Checklist

## 🚀 Quick Start (5 Minutes)

### Pre-Implementation
- [ ] Backup current GPT instructions (copy/paste to a text file)
- [ ] Have all files from `custom-gpt` folder ready
- [ ] Open Custom GPT configuration page: https://chat.openai.com/ → Your GPTs → Data Craft

---

## Step 1: Update Instructions (2 min)

- [ ] Open `instructions.md` from this folder
- [ ] Copy ENTIRE content (Ctrl+A, Ctrl+C)
- [ ] In GPT Configure tab, clear existing Instructions field
- [ ] Paste new instructions (Ctrl+V)
- [ ] Verify no truncation occurred (scroll to bottom, should see "Adaptive Questioning Guidelines" section)

**Verification**: Instructions field should be ~150 lines, ending with "Include Data Quality Framework application guidance in README"

---

## Step 2: Update Description (30 sec)

- [ ] In Description field, replace with:
```
I help you create realistic operational datasets for analytics projects based on your job description and business problem.
```

**Verification**: Description mentions "operational datasets" and "job description"

---

## Step 3: Update Conversation Starters (1 min)

- [ ] Delete existing conversation starters
- [ ] Add Starter 1:
```
Help me create a dataset for my operations analytics project
```

- [ ] Add Starter 2:
```
I need data for Milestone 1 (Descriptive/Diagnostic Analytics)
```

- [ ] Add Starter 3:
```
I need data for Milestone 2 (Predictive Analytics)
```

- [ ] Add Starter 4:
```
I need data for Milestone 3 (Prescriptive Analytics)
```

**Verification**: You should see 4 conversation starters, each mentioning milestones or operations

---

## Step 4: Upload Knowledge Files (2 min)

- [ ] Click "Upload files" in Knowledge section
- [ ] Upload `ops-decision-areas-reference.md`
- [ ] Upload `analytics-type-specifications.md`
- [ ] Upload `output-templates-and-formats.md`
- [ ] Upload `milestone-requirements-summary.md`

**Verification**: Knowledge section should show 4 files uploaded

---

## Step 5: Verify Model Selection (10 sec)

- [ ] Scroll to "Recommended Model"
- [ ] Ensure "GPT-5" is selected (or latest available)

**Verification**: Model dropdown shows GPT-5

---

## Step 6: Save Configuration (10 sec)

- [ ] Click "Save" or "Update" button (top right)
- [ ] Wait for confirmation message
- [ ] Navigate back to ChatGPT interface

**Verification**: Changes saved successfully, GPT available for testing

---

## 🧪 Testing (5 Minutes)

### Test 1: Milestone 1 Entry
- [ ] Start new conversation
- [ ] Click "I need data for Milestone 1" starter
- [ ] **Expected**: GPT asks about resume/job description (ONE question)
- [ ] **Expected**: Does NOT list all questions at once
- [ ] Provide a sample job description
- [ ] **Expected**: GPT asks next question (industry/sector) only after receiving response

**✅ Pass if**: ONE question at a time, relevant to Milestone 1

---

### Test 2: Decision Area Retrieval
- [ ] Continue previous conversation or start new
- [ ] Get to decision area selection
- [ ] **Expected**: GPT suggests 2-3 options OR retrieves examples from knowledge file
- [ ] **Expected**: Does NOT list all 10 decision areas with full descriptions upfront

**✅ Pass if**: Concise options, retrieves knowledge when needed

---

### Test 3: Analytics Type Adaptation
- [ ] Start conversation with "I need data for Milestone 2"
- [ ] **Expected**: GPT asks about time series forecasting OR regression
- [ ] **Expected**: Questions are specific to predictive analytics
- [ ] Choose "time series forecasting"
- [ ] **Expected**: Asks about target variable, time horizon, etc.

**✅ Pass if**: Questions adapt based on analytics type selected

---

### Test 4: Complete Flow
- [ ] Complete a full conversation from start to dataset generation
- [ ] **Expected**: Progressive questioning through all 4 phases
- [ ] **Expected**: GPT INFORMS about data quality issues (doesn't ask which ones to include)
- [ ] **Expected**: Generates appropriate dataset with ALL 5 quality issue types
- [ ] **Expected**: Includes data dictionary
- [ ] **Expected**: README connects to Operations Management Decision Area

**✅ Pass if**: Complete deliverables match student requirements and ALL quality issues are present

---

## 🔍 Troubleshooting

### Issue: Instructions appear truncated
**Check**:
- [ ] Did you copy the ENTIRE `instructions.md` file?
- [ ] Is there a character limit warning in the UI?

**Fix**:
- Instructions should be ~2,500 characters (well under 8,000 limit)
- If truncated, verify no extra characters were copied
- Try copying in plain text editor first, then paste

---

### Issue: GPT not asking ONE question at a time
**Check**:
- [ ] Is "ONE Question at a Time" principle in Core Principles section?
- [ ] Are you testing with conversation starters or custom prompts?

**Fix**:
- Verify instructions were pasted correctly
- Test with provided conversation starters
- If persistent, add more emphasis: "CRITICAL: Always ask ONE question at a time. Never ask multiple questions in a single message."

---

### Issue: Knowledge files not being retrieved
**Check**:
- [ ] Are all 4 files uploaded to Knowledge section?
- [ ] Do file names match exactly what's in instructions? (check for typos)

**Fix**:
- Re-upload any missing files
- Verify file names:
  - `ops-decision-areas-reference.md`
  - `analytics-type-specifications.md`
  - `output-templates-and-formats.md`
  - `milestone-requirements-summary.md`

---

### Issue: Generic responses (not customized to context)
**Check**:
- [ ] Did GPT ask about job description, industry, decision area?
- [ ] Is it using information from previous answers?

**Fix**:
- Verify knowledge files are uploaded
- May need to explicitly remind: "Use the context I provided about [industry/decision area] to tailor your suggestions"

---

### Issue: Students reporting unexpected behavior
**Check**:
- [ ] What conversation starter did they use?
- [ ] What responses did they provide?
- [ ] Does it happen consistently?

**Fix**:
- Review specific conversation logs
- May need to adjust knowledge files for edge cases
- Update specific knowledge file (easy fix, no instructions change needed)

---

## 📊 Success Criteria

Your implementation is successful when:

✅ **Functionality**:
- [ ] GPT asks ONE question at a time consistently
- [ ] Milestone-specific conversation starters work correctly
- [ ] Knowledge files are retrieved appropriately
- [ ] Complete dataset generation produces all required deliverables

✅ **Quality**:
- [ ] Datasets match student milestone requirements
- [ ] Data quality issues are included intentionally
- [ ] README connects to Operations Management Decision Area
- [ ] Data dictionary is comprehensive

✅ **User Experience**:
- [ ] Students find it easier to start with conversation starters
- [ ] Progressive questioning feels natural
- [ ] Responses are customized to their context
- [ ] No overwhelming lists of options upfront

✅ **Maintenance**:
- [ ] You can update decision areas by editing one file
- [ ] You can update analytics specs by editing one file
- [ ] Core instructions remain stable
- [ ] Changes take <5 minutes to implement

---

## 📈 Monitoring & Iteration

### Week 1: Monitor Usage
- [ ] Check student feedback
- [ ] Look for common questions/confusion
- [ ] Identify any gaps in knowledge files

### Week 2: Refine Knowledge Files
- [ ] Update `ops-decision-areas-reference.md` if new examples needed
- [ ] Enhance `analytics-type-specifications.md` if students need more guidance
- [ ] Adjust templates if output format needs refinement

### Week 3: Optimize Flow
- [ ] Review conversation logs for common patterns
- [ ] Identify opportunities to improve question sequencing
- [ ] Update specific knowledge files (no instructions changes needed)

### Ongoing: Easy Updates
- New decision area examples? → Edit `ops-decision-areas-reference.md`
- New analytics type? → Edit `analytics-type-specifications.md`
- Template changes? → Edit `output-templates-and-formats.md`
- Milestone updates? → Edit `milestone-requirements-summary.md`

**No changes to core instructions needed!**

---

## 🎉 You're Done!

Congratulations! You've successfully optimized the Data Craft GPT using Anthropic's Effective Context Engineering Principles.

### What You've Achieved:
✅ 95% reduction in context tokens
✅ Better user experience with milestone-specific entry
✅ Easier maintenance (update specific files vs entire prompt)
✅ Scalable architecture for future enhancements
✅ Cost savings (~95% reduction in instruction tokens)

### Next Steps:
1. Monitor student usage for first few days
2. Gather feedback on user experience
3. Iterate on knowledge files as needed (quick updates)
4. Enjoy the improved maintainability!

---

**Questions or Issues?**
- Review `ui-configuration.md` for detailed troubleshooting
- Check `before-after-comparison.md` to understand optimizations
- See `README.md` for complete documentation

**Happy Dataset Generating! 🎯📊**
