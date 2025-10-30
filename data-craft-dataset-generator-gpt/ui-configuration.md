# Custom GPT UI Configuration

## Name
```
Data Craft
```

## Description
```
I help you create realistic operational datasets for analytics projects based on your job description and business problem.
```

## Instructions
Copy the content from `instructions.md` into the Instructions field.

## Conversation Starters

### Starter 1
```
Help me create a dataset for my operations analytics project
```

### Starter 2
```
I need data for Milestone 1 (Descriptive/Diagnostic Analytics)
```

### Starter 3
```
I need data for Milestone 2 (Predictive Analytics)
```

### Starter 4
```
I need data for Milestone 3 (Prescriptive Analytics)
```

## Knowledge Files

Upload these 4 files to the Knowledge section:

1. **ops-decision-areas-reference.md**
   - Contains: 10 Operations Management Decision Areas with examples, metrics, and scenarios
   - Retrieved when: Student selects a decision area

2. **analytics-type-specifications.md**
   - Contains: Detailed specifications for each analytics type (Descriptive, Predictive, Prescriptive)
   - Retrieved when: Student indicates milestone or analytics type

3. **output-templates-and-formats.md**
   - Contains: README structure, data dictionary format, delivery templates
   - Retrieved when: Generating final outputs

4. **milestone-requirements-summary.md**
   - Contains: Milestone 1, 2, 3 requirements and student deliverables
   - Retrieved when: Student mentions milestone number

## Recommended Model
```
GPT-5
```

---

## Implementation Steps

### Step 1: Open Custom GPT Configuration
1. Go to https://chat.openai.com/
2. Navigate to "Explore GPTs" → "Create"
3. Click on "Configure" tab

### Step 2: Update Basic Information
1. **Name**: Enter "Data Craft"
2. **Description**: Copy the description above
3. Keep the existing profile image or upload a new one

### Step 3: Update Instructions
1. Open `instructions.md` from the custom-gpt folder
2. Copy the ENTIRE content
3. Paste into the "Instructions" field in the GPT configuration
4. Verify no truncation occurred

### Step 4: Update Conversation Starters
1. Delete existing conversation starters
2. Add the 4 new starters listed above (copy/paste each one)

### Step 5: Upload Knowledge Files
1. Click "Upload files" in the Knowledge section
2. Upload all 4 files from the custom-gpt folder:
   - ops-decision-areas-reference.md
   - analytics-type-specifications.md
   - output-templates-and-formats.md
   - milestone-requirements-summary.md
3. Verify all 4 files appear in the Knowledge section

### Step 6: Verify Model Selection
1. Under "Recommended Model", ensure "GPT-5" is selected
2. This provides the best instruction following and knowledge retrieval

### Step 7: Save and Test
1. Click "Save" or "Update" at the top right
2. Test with one of the conversation starters
3. Verify it asks ONE question at a time
4. Verify it references knowledge files appropriately

---

## Testing Checklist

After implementation, test these scenarios:

### Test 1: Basic Interaction
- [ ] Start with "Help me create a dataset for my operations analytics project"
- [ ] Verify it asks for resume/job description first
- [ ] Verify it asks ONE question at a time
- [ ] Verify it doesn't list all 10 decision areas immediately

### Test 2: Milestone-Specific Entry
- [ ] Start with "I need data for Milestone 1"
- [ ] Verify it asks context questions appropriate to Milestone 1
- [ ] Verify it references descriptive/diagnostic analytics
- [ ] Verify it includes ALL 5 data quality issues

### Test 2b: Milestone 2 Dual-Dataset Generation
- [ ] Start with "I need data for Milestone 2"
- [ ] Verify it asks about BOTH time series forecasting AND regression problems
- [ ] Verify it generates TWO separate datasets
- [ ] Verify datasets are CLEAN (no quality issues)
- [ ] Verify time series has 18-24 months with NO GAPS
- [ ] Verify regression has 4-6 independent variables

### Test 3: Knowledge Retrieval
- [ ] When student selects a decision area, verify it provides 2-3 relevant examples
- [ ] Verify it doesn't list exhaustive technical specs upfront
- [ ] Verify it adapts questions based on previous answers

### Test 4: Data Generation
- [ ] Complete a full interaction
- [ ] Verify it generates appropriate dataset structure
- [ ] Verify data dictionary is included
- [ ] Verify README connects to Operations Management Decision Area

---

## Troubleshooting

### Issue: Instructions appear truncated
**Solution**: The Instructions field has a character limit. The optimized version should fit. If truncated:
1. Verify you copied the FULL instructions.md content
2. Check for any formatting issues
3. Consider slight further compaction if needed

### Issue: Knowledge files not retrieving
**Solution**:
1. Verify all 4 files are uploaded successfully
2. Check file names match exactly what's referenced in instructions
3. Test with specific prompts that should trigger retrieval

### Issue: GPT asking multiple questions at once
**Solution**:
1. Verify "ONE Question at a Time" principle is in Instructions
2. Remind the GPT in conversation: "Please ask one question at a time"
3. May need to add emphasis in instructions if persistent

### Issue: Too generic responses
**Solution**:
1. Ensure Knowledge files are uploaded
2. GPT should adapt based on decision area, industry, milestone
3. May need to explicitly reference knowledge files in instructions

---

## Optimization Results Summary

### Before (Original)
- **Instructions**: ~771 lines (~50,000+ characters)
- **Structure**: All content embedded in single prompt
- **Maintainability**: Difficult (must edit entire prompt)
- **Context efficiency**: Low (all loaded every time)

### After (Optimized)
- **Instructions**: ~150 lines (~2,500 characters) - **95% reduction**
- **Structure**: Core behavior + 4 external knowledge files
- **Maintainability**: Easy (update specific files)
- **Context efficiency**: High (retrieve only what's needed)

### Benefits Achieved
✅ Follows Anthropic's "smallest set of high-signal tokens" principle
✅ Uses "sub-agent architecture" via knowledge retrieval
✅ "Clear, direct language at right altitude"
✅ Easier to maintain and update over time
✅ Better user experience with targeted conversation starters
✅ Leverages GPT-5's improved capabilities
