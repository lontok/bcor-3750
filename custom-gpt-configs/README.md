# BCOR 3750 Midterm Interview Coach - CustomGPT Setup Guide

## Overview

This CustomGPT simulates the BCOR 3750 Midterm Interview (Milestone 1) with realistic professor-style questioning, Socratic guidance, and constructive feedback.

## Files in This Directory

### Configuration Files
- **[custom-gpt-config-midterm-interview.md](custom-gpt-config-midterm-interview.md)**: Complete reference configuration (full documentation)
  - **NOTE:** Instructions section is too long for OpenAI (12K chars, limit is 8K) - use for reference only
- **[custom-gpt-instructions-condensed.md](custom-gpt-instructions-condensed.md)**: **⭐ USE THIS for OpenAI setup**
  - Condensed instructions (~5K characters) that fit within 8K limit
  - All essential behaviors preserved
  - GPT Name, Description, Conversation Starters included

### Knowledge Base Files (Upload to GPT)
These files provide the GPT with essential reference material:

1. **[knowledge-midterm-interview-study-guide.md](knowledge-midterm-interview-study-guide.md)**
   - Complete Midterm Interview Study Guide
   - Rubric, structure, timing breakdown, sample questions
   - Lines 1-369 from original study guide

2. **[knowledge-milestone-1-requirements-excerpt.md](knowledge-milestone-1-requirements-excerpt.md)**
   - Milestone 1 Descriptive & Diagnostic Analytics requirements
   - Project foundation, data requirements, analysis specifications
   - Slide deck structure and IRPM framework overview
   - Interview format and assessment rubric

3. **[knowledge-irpm-framework-reference.md](knowledge-irpm-framework-reference.md)**
   - IRPM Framework structure and usage
   - 5 complete examples (Central Tendency, Variability, PivotTable, Dashboards)
   - Validation checklist and interview questioning strategies
   - Common mistakes and strong examples

4. **[knowledge-whiteboard-roadmap-template.md](knowledge-whiteboard-roadmap-template.md)**
   - Visual roadmap template students must draw
   - Drawing instructions and component details
   - Validation checklist for uploaded whiteboard photos
   - Feedback examples (strong, needs improvement, insufficient)

### Update Guide
- **[custom-gpt-update-guide.md](custom-gpt-update-guide.md)**: Step-by-step instructions for updating existing CustomGPTs

---

## Setup Instructions

### Step 1: Create New CustomGPT

1. Go to [ChatGPT](https://chatgpt.com)
2. Click your profile → "My GPTs" → "Create a GPT"
3. Switch to "Configure" tab

### Step 2: Basic Information

Copy from **[custom-gpt-config-midterm-interview.md](custom-gpt-config-midterm-interview.md)**:

**Name:**
```
BCOR 3750 Midterm Interview Coach
```

**Description:**
```
Practice for your BCOR 3750 Midterm Interview (Milestone 1) with realistic simulation, Socratic questioning, and constructive feedback. Upload your slides (optional) and experience a professor-style interview covering Foundation, Descriptive Analytics, and Diagnostic Analytics.
```

### Step 3: Instructions

Copy the ENTIRE **Instructions** section from **[custom-gpt-config-midterm-interview.md](custom-gpt-config-midterm-interview.md)** into the "Instructions" field.

This includes:
- Core Identity & Purpose
- Interview Scope
- Difficulty Modes
- Interaction Protocol (ONE question at a time, slide upload, timing, whiteboard)
- Framework Validation (IRPM)
- Socratic Questioning Strategy
- Weak Area Challenge & Support
- Behavioral Guardrails
- Tone
- Feedback Structure
- Success Criteria
- Knowledge Base References
- Session Flow
- Example Interaction Flow

### Step 4: Conversation Starters

Add these 5 conversation starters:

1. **"I want to practice the full interview with my slides"**
2. **"Help me prepare my 'Tell me about yourself' response"**
3. **"Practice quick section: Foundation only (Job through Primary Metric)"**
4. **"Practice quick section: Descriptive Analytics only"**
5. **"Practice quick section: Diagnostic Analytics only"**

### Step 5: Knowledge Base Upload

Upload these 4 files to the "Knowledge" section:

1. **knowledge-midterm-interview-study-guide.md**
2. **knowledge-milestone-1-requirements-excerpt.md**
3. **knowledge-irpm-framework-reference.md**
4. **knowledge-whiteboard-roadmap-template.md**

### Step 6: Capabilities

Configure capabilities:
- **Web Browsing**: ❌ OFF
- **DALL·E Image Generation**: ❌ OFF
- **Code Interpreter**: ❌ OFF

### Step 7: Save and Test

1. Click "Create" (top right)
2. Test with sample scenarios:
   - Start a practice session without slides
   - Upload sample slides and verify GPT analyzes them
   - Test Socratic questioning (say "I don't know" to a question)
   - Verify ONE question at a time behavior
   - Check IRPM validation triggers
   - Test whiteboard upload and feedback

---

## Testing Checklist

After setup, verify these critical behaviors:

### Core Behaviors
- [ ] GPT asks about difficulty mode at session start (Practice/Realistic/Challenging)
- [ ] GPT asks about slide upload
- [ ] GPT reminds student to start 15-minute timer
- [ ] GPT asks **ONE question at a time** (never batches questions)
- [ ] GPT contextualizes next question based on previous response

### Socratic Questioning
- [ ] When student says "I don't know," GPT uses guiding questions (not direct answers)
- [ ] GPT provides 4 levels of Socratic questions (Clarification → Connecting → Deeper Probing → Leading)
- [ ] GPT only provides example answers after extended Socratic dialogue

### IRPM Framework Validation
- [ ] GPT validates all 4 IRPM components (Insight, Recommendation, Prediction, Method)
- [ ] GPT flags missing IRPM elements
- [ ] GPT tracks 5 required IRPM cycles (2 stats + 1 strategic + 2 pivots)

### Feedback Quality
- [ ] GPT provides ruthlessly honest yet supportive feedback
- [ ] GPT assesses all 4 rubric dimensions (Depth 40%, Business 30%, Communication 20%, Synthesis 10%)
- [ ] GPT identifies 2-3 specific weaknesses with examples
- [ ] GPT references study guide sections and line numbers
- [ ] GPT quotes rubric when explaining performance level

### Whiteboard Simulation
- [ ] GPT prompts student to draw roadmap
- [ ] GPT requests photo upload of whiteboard
- [ ] GPT validates structure and content against template
- [ ] GPT provides specific feedback on missing/unclear elements

---

## Common Issues and Solutions

### Issue: GPT asks multiple questions in one message
**Solution:** Emphasize in testing: "Ask me ONE question, wait for my response, then ask the next question based on what I said."

### Issue: GPT gives direct answers when student struggles
**Solution:** Test by saying "I don't know" - GPT should ask guiding questions, not provide answers directly.

### Issue: GPT doesn't validate IRPM framework
**Solution:** Test by providing incomplete IRPM (e.g., only Insight and Method) - GPT should flag missing Recommendation and Prediction.

### Issue: Feedback is too generic
**Solution:** Review feedback - should include specific examples from the practice session, not generic advice.

### Issue: GPT doesn't reference study guide
**Solution:** Check Knowledge base upload - all 4 files should be present and accessible.

---

## Updating the GPT

See **[custom-gpt-update-guide.md](custom-gpt-update-guide.md)** for detailed update instructions.

Quick update process:
1. Edit relevant configuration or knowledge file in this directory
2. Go to ChatGPT → My GPTs → Edit "BCOR 3750 Midterm Interview Coach"
3. Update Instructions or re-upload Knowledge file
4. Save and test changes

---

## Usage Guidelines for Students

### Full Interview Practice (Recommended)
1. Complete Milestone 1 slides first
2. Start conversation: "I want to practice the full interview with my slides"
3. Upload slides when prompted
4. Practice for full 15 minutes
5. Review detailed feedback

### Section-Specific Practice
- **Foundation only**: "Practice quick section: Foundation only"
- **Descriptive only**: "Practice quick section: Descriptive Analytics only"
- **Diagnostic only**: "Practice quick section: Diagnostic Analytics only"

### "Tell Me About Yourself" Practice
- Start with: "Help me prepare my 'Tell me about yourself' response"
- Practice the 1-minute opening with project segue

### Multiple Sessions
- Each session is independent (no tracking across sessions)
- Students can practice multiple times focusing on different weak areas
- Feedback is specific to each session

---

## Key Design Principles

### 1. ONE Question at a Time
**Why:** Simulates real interview flow, prevents overwhelming students, allows context-aware follow-ups

**Implementation:** Explicit instructions to never batch questions, contextualize based on previous response

### 2. Socratic Questioning (Never Give Answers)
**Why:** Develops student reasoning, mirrors professor interview style, builds confidence through discovery

**Implementation:** 4-level questioning strategy (Clarification → Connecting → Probing → Leading), explicit "DO NOT" rules

### 3. IRPM Framework Validation
**Why:** Core requirement for Milestone 1, ensures students apply framework to all 5 components

**Implementation:** Validation checklist, flagging missing elements, example provision only after extended struggle

### 4. Ruthlessly Honest Yet Supportive Feedback
**Why:** Students requested honest assessment while maintaining encouragement

**Implementation:** Rubric-based assessment, specific weaknesses with examples, study guide references, actionable next steps

### 5. Whiteboard Simulation
**Why:** Required interview component, visual diagram validation needed

**Implementation:** Photo upload prompt, template validation, specific structural and content feedback

---

## Future Enhancements (Potential)

### Version 2.0 Ideas:
- **Final Interview GPT**: Cover Milestones 2-3 (Predictive + Prescriptive Analytics)
- **Adaptive Difficulty**: GPT automatically adjusts based on student performance
- **Common Weakness Library**: Track frequent student struggles and provide targeted resources
- **Timed Mode**: GPT enforces strict 15-minute limit with auto-debrief

---

## Support and Questions

**For Students:**
- Use conversation starters to guide your practice session
- Upload slides for personalized feedback
- Practice multiple times - each session is independent
- Review study guide references in feedback

**For Instructors:**
- Configuration file contains all behavioral rules
- Knowledge base files are modular (update individually)
- Test changes with sample scenarios before student use
- See update guide for maintenance workflow

---

**Last Updated:** January 2025
**Version:** 1.0
**Contact:** Greg Lontok (greg@lontok.com)
