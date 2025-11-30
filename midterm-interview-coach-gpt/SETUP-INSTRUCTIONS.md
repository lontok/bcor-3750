# Quick Setup: BCOR 3750 Midterm Interview Coach

## 1. Create New GPT

Go to [ChatGPT](https://chatgpt.com) → Profile → "My GPTs" → "Create a GPT" → Switch to "Configure" tab

---

## 2. Copy-Paste Configuration

### Name
```
BCOR 3750 Midterm Interview Coach
```

### Description
```
Practice for your BCOR 3750 Midterm Interview (Milestone 1) with realistic simulation, Socratic questioning, and constructive feedback. Upload your slides (optional) and experience a realistic interview covering Data Foundations, Descriptive Analytics, and Diagnostic Analytics.
```

### Instructions
**📋 Copy the ENTIRE condensed instructions from:**
`custom-gpt-instructions-condensed.md`

**⚠️ IMPORTANT:** The full `custom-gpt-config-midterm-interview.md` instructions are TOO LONG (12K chars, limit is 8K). Use the condensed version instead.

(Copy everything from "You are a supportive but rigorous..." to the end of that file - approximately 5,000 characters)

### Conversation Starters
Add these 5 starters:

1. `I want to practice the full interview with my slides`
2. `Help me prepare my 'Tell me about yourself' response`
3. `Practice only Job through Primary Metric`
4. `Practice Descriptive Analytics only`
5. `Practice Diagnostic Analytics only`

---

## 3. Upload Knowledge Files

Click "+ Upload files" in the Knowledge section and upload these 4 files:

1. ✅ `knowledge-midterm-interview-study-guide.md`
2. ✅ `knowledge-milestone-1-requirements-excerpt.md`
3. ✅ `knowledge-irpm-framework-reference.md`
4. ✅ `knowledge-whiteboard-roadmap-template.md`

---

## 4. Configure Capabilities

**Disable all capabilities:**
- ❌ Web Browsing: OFF
- ❌ DALL·E Image Generation: OFF
- ❌ Code Interpreter: OFF

---

## 5. Save and Share

1. Click "Create" (top right)
2. Choose sharing option:
   - **"Anyone with a link"** (recommended for students)
   - OR "Only me" if testing first
3. Copy the share link

---

## 6. Test Critical Behaviors

### Test 1: ONE Question at a Time ✅
- Start a session
- GPT should ask ONE question, wait for response, then ask next question
- ❌ Should NOT ask multiple questions in one message

### Test 2: Socratic Questioning ✅
- When asked a question, respond "I don't know"
- GPT should ask guiding questions (NOT give direct answer)
- Should see 4 levels: Clarification → Connecting → Probing → Leading

### Test 3: IRPM Validation ✅
- Describe a central tendency finding (just state the number)
- GPT should prompt for all 4 IRPM elements:
  - I - Insight (what it means)
  - R - Recommendation (what to do)
  - P - Prediction (expected outcome)
  - M - Method (how you calculated)

### Test 4: Feedback Quality ✅
- Complete a practice session
- Check debrief includes:
  - ✅ 4 rubric dimensions (Depth 40%, Business 30%, Communication 20%, Synthesis 10%)
  - ✅ 2-3 specific weaknesses with examples
  - ✅ Study guide references (line numbers)
  - ✅ Rubric quote for performance level

### Test 5: Whiteboard Simulation ✅
- Start Foundation section
- GPT should prompt to draw roadmap on paper/tablet
- GPT should request photo upload
- GPT should validate against template

---

## 7. Share with Students

**Share Link Format:**
```
https://chatgpt.com/g/g-XXXXXX-bcor-3750-midterm-interview-coach
```

**Recommended Student Instructions:**
> "Practice your Midterm Interview with the AI coach. Upload your Milestone 1 slides for personalized feedback, or practice without slides for generic questions. The coach will ask ONE question at a time, guide you with Socratic questioning if you struggle, and provide honest feedback based on the interview rubric."

---

## Troubleshooting

### Issue: GPT asks multiple questions
**Fix:** In Instructions, emphasize "Never ask multiple questions in a single message"

### Issue: GPT gives direct answers
**Fix:** Test Socratic questioning section - should have 4-level strategy

### Issue: GPT doesn't validate IRPM
**Fix:** Check Knowledge files uploaded correctly - especially `knowledge-irpm-framework-reference.md`

### Issue: Feedback is generic
**Fix:** Review "FEEDBACK STRUCTURE" section in Instructions - should reference specific examples from session

### Issue: Study guide not referenced
**Fix:** Verify all 4 Knowledge files uploaded and accessible

---

## Quick Reference Card

**What this GPT does:**
✅ Simulates realistic Midterm Interview (Milestone 1 only)
✅ Asks ONE question at a time (builds conversation)
✅ Uses Socratic questioning (guides to answers, never gives them)
✅ Validates IRPM framework for 5 required components
✅ Provides ruthlessly honest yet supportive feedback
✅ Validates whiteboard roadmap drawings
✅ References study guide sections in feedback

**What this GPT does NOT do:**
❌ Cover Milestones 2-3 (Predictive/Prescriptive)
❌ Give direct answers or write IRPM for students
❌ Grade actual submissions (practice only)
❌ Track improvement across sessions

---

## Files Created

**Configuration:**
- [custom-gpt-config-midterm-interview.md](custom-gpt-config-midterm-interview.md) - Main config file

**Knowledge Base:**
- [knowledge-midterm-interview-study-guide.md](knowledge-midterm-interview-study-guide.md) - Complete study guide
- [knowledge-milestone-1-requirements-excerpt.md](knowledge-milestone-1-requirements-excerpt.md) - Milestone 1 requirements
- [knowledge-irpm-framework-reference.md](knowledge-irpm-framework-reference.md) - IRPM framework details
- [knowledge-whiteboard-roadmap-template.md](knowledge-whiteboard-roadmap-template.md) - Whiteboard template

**Documentation:**
- [README.md](README.md) - Complete setup guide
- [SETUP-INSTRUCTIONS.md](SETUP-INSTRUCTIONS.md) - This quick reference
- [custom-gpt-update-guide.md](custom-gpt-update-guide.md) - Update instructions

---

**Setup Time:** ~15 minutes
**Last Updated:** January 2025
**Version:** 1.0
