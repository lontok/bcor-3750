# OpenAI ChatGPT Configuration UI Reference

## Visual Guide to CustomGPT Setup

This guide shows exactly where to paste each configuration element in the OpenAI ChatGPT interface.

---

## Step 1: Access GPT Builder

**Navigation:**
1. Go to [https://chatgpt.com](https://chatgpt.com)
2. Click your **Profile Picture** (bottom left)
3. Click **"My GPTs"**
4. Click **"Create a GPT"** button (top right)
5. Switch to **"Configure"** tab (you'll see "Create" and "Configure" tabs at top)

---

## Step 2: Configure Tab Layout

The "Configure" tab has these fields (from top to bottom):

```
┌─────────────────────────────────────────────────────┐
│ Profile Picture                    [Upload Image]   │
├─────────────────────────────────────────────────────┤
│ Name                                                │
│ ┌─────────────────────────────────────────────────┐ │
│ │ [Enter GPT name here]                           │ │
│ └─────────────────────────────────────────────────┘ │
├─────────────────────────────────────────────────────┤
│ Description                                         │
│ ┌─────────────────────────────────────────────────┐ │
│ │ [Enter description here]                        │ │
│ └─────────────────────────────────────────────────┘ │
├─────────────────────────────────────────────────────┤
│ Instructions                                        │
│ ┌─────────────────────────────────────────────────┐ │
│ │                                                 │ │
│ │ [Paste full instructions here]                  │ │
│ │                                                 │ │
│ │ (This will be a LARGE text block)              │ │
│ └─────────────────────────────────────────────────┘ │
├─────────────────────────────────────────────────────┤
│ Conversation starters                               │
│ ┌─────────────────────────────────────────────────┐ │
│ │ [Starter 1]                                     │ │
│ ├─────────────────────────────────────────────────┤ │
│ │ [Starter 2]                                     │ │
│ ├─────────────────────────────────────────────────┤ │
│ │ [Starter 3]                                     │ │
│ ├─────────────────────────────────────────────────┤ │
│ │ [Starter 4]                                     │ │
│ └─────────────────────────────────────────────────┘ │
├─────────────────────────────────────────────────────┤
│ Knowledge                                           │
│ ┌─────────────────────────────────────────────────┐ │
│ │ [+ Upload files]                                │ │
│ │                                                 │ │
│ │ • file1.md                                      │ │
│ │ • file2.md                                      │ │
│ └─────────────────────────────────────────────────┘ │
├─────────────────────────────────────────────────────┤
│ Capabilities                                        │
│ ☐ Web Browsing                                      │
│ ☐ DALL·E Image Generation                           │
│ ☐ Code Interpreter                                  │
├─────────────────────────────────────────────────────┤
│ Actions                                             │
│ [Create new action]                                 │
└─────────────────────────────────────────────────────┘

                        [Cancel]  [Save]  [Create]
```

---

## Step 3: Fill Each Field

### Field 1: Name
**Copy this EXACTLY:**
```
BCOR 3750 Midterm Interview Coach
```

**Location:** Top "Name" field
**Character limit:** ~50 characters
**Appears:** As GPT title in chat interface

---

### Field 2: Description
**Copy this EXACTLY:**
```
Practice for your BCOR 3750 Midterm Interview (Milestone 1) with realistic simulation, Socratic questioning, and constructive feedback. Upload your slides (optional) and experience a professor-style interview covering Foundation, Descriptive Analytics, and Diagnostic Analytics.
```

**Location:** "Description" field (below Name)
**Character limit:** ~300 characters
**Appears:** In GPT preview card when sharing

---

### Field 3: Instructions
**Source file:** `custom-gpt-config-midterm-interview.md`
**Section to copy:** Everything under "## Instructions" heading

**Start copying from:**
```
### CORE IDENTITY & PURPOSE
You are a supportive but rigorous interview coach...
```

**End copying at:**
```
...Want to run through another practice round focusing on your weak areas?"
```

**Location:** Large "Instructions" text area
**Character limit:** ~8,000 characters (Instructions are LONG - this is normal!)
**Appears:** Defines GPT behavior (not visible to users)

**Important:** Copy the ENTIRE Instructions section - it's approximately 400+ lines

---

### Field 4: Conversation Starters
**Add 5 starters (click "+ Add" to create each one):**

**Starter 1:**
```
I want to practice the full interview with my slides
```

**Starter 2:**
```
Help me prepare my 'Tell me about yourself' response
```

**Starter 3:**
```
Practice quick section: Foundation only (Job through Primary Metric)
```

**Starter 4:**
```
Practice quick section: Descriptive Analytics only
```

**Starter 5:**
```
Practice quick section: Diagnostic Analytics only
```

**Location:** "Conversation starters" section
**Character limit per starter:** ~60 characters each
**Appears:** As clickable buttons when user starts new chat

---

### Field 5: Knowledge (Upload Files)
**Click "+ Upload files" and select these 4 files:**

1. `knowledge-midterm-interview-study-guide.md`
2. `knowledge-milestone-1-requirements-excerpt.md`
3. `knowledge-irpm-framework-reference.md`
4. `knowledge-whiteboard-roadmap-template.md`

**Location:** "Knowledge" section
**File size limit:** ~512KB per file (text files are fine)
**Total files:** Up to 20 files allowed (we're using 4)
**Appears:** GPT can reference these during conversations

**After upload, you'll see:**
```
Knowledge
  • knowledge-midterm-interview-study-guide.md (82 KB)
  • knowledge-milestone-1-requirements-excerpt.md (45 KB)
  • knowledge-irpm-framework-reference.md (38 KB)
  • knowledge-whiteboard-roadmap-template.md (27 KB)
```

---

### Field 6: Capabilities
**DISABLE ALL (uncheck all boxes):**

- ☐ **Web Browsing** - UNCHECK (OFF)
- ☐ **DALL·E Image Generation** - UNCHECK (OFF)
- ☐ **Code Interpreter** - UNCHECK (OFF)

**Location:** "Capabilities" section
**Why disabled:** GPT only needs Knowledge base + conversation - no external tools
**Appears:** Determines what tools GPT can use during chat

---

### Field 7: Actions
**Leave EMPTY (no actions needed)**

**Location:** "Actions" section at bottom
**Skip this:** Don't click "Create new action"

---

## Step 4: Save and Share

### Click "Create" Button
**Location:** Top right corner (next to "Save" button)

**This will:**
1. Save your GPT configuration
2. Open sharing options dialog

### Choose Sharing Option

**Option 1: Anyone with a link (Recommended for students)**
- Click "Anyone with a link"
- Copy the link that appears
- Share with students via Brightspace/email

**Option 2: Only me (For testing first)**
- Click "Only me"
- Test thoroughly
- Later: Edit GPT → Change to "Anyone with a link"

---

## Verification Checklist

After creating, verify these in the GPT interface:

### In "Configure" Tab:
- [ ] Name shows: "BCOR 3750 Midterm Interview Coach"
- [ ] Description shows complete text (300 chars)
- [ ] Instructions are LONG (scroll to verify full content)
- [ ] 5 conversation starters visible
- [ ] 4 knowledge files uploaded (shows file names + sizes)
- [ ] All 3 capabilities are UNCHECKED
- [ ] No actions created

### In "Create" Tab (Preview):
- [ ] GPT name appears at top
- [ ] 5 conversation starter buttons visible
- [ ] Clicking a starter prompts the GPT correctly

---

## Common Issues During Setup

### Issue 1: Instructions Too Long Error
**Symptom:** "Instructions exceed character limit"
**Cause:** Instructions are ~8,000 characters (this is normal and expected)
**Solution:** This should work fine - if error persists, check for accidental duplicates

### Issue 2: Knowledge Files Won't Upload
**Symptom:** Upload button doesn't work or files rejected
**Cause:** File format or size issue
**Solution:**
- Ensure files are `.md` format (Markdown)
- Check file size <512KB each
- Try uploading one at a time

### Issue 3: Can't Find "Configure" Tab
**Symptom:** Only see "Create" interface
**Cause:** Haven't switched tabs yet
**Solution:** Look for "Create" and "Configure" tabs at top - click "Configure"

### Issue 4: Conversation Starters Not Showing
**Symptom:** Chat interface doesn't show starter buttons
**Cause:** Starters may be too long or not saved
**Solution:**
- Keep each starter under 60 characters
- Click outside field after typing to save
- Refresh preview in "Create" tab

---

## After Setup: First Test

### Test Script
1. Click "Create" → Open new chat with your GPT
2. Don't click any starters - just type: **"Hi"**
3. GPT should respond with:
   - Introduces itself as interview coach
   - Asks about difficulty mode (Practice/Realistic/Challenging)
4. Choose difficulty mode
5. GPT should ask about slide upload
6. Respond "No slides yet"
7. GPT should remind you to start 15-minute timer
8. GPT should ask: **"Tell me about yourself."** (ONE question only)

**If you see this flow, setup is successful! ✅**

---

## Screenshot Reference (What You'll See)

### Name Field:
```
┌─────────────────────────────────────────────────────┐
│ Name                                                │
│ ┌─────────────────────────────────────────────────┐ │
│ │ BCOR 3750 Midterm Interview Coach               │ │
│ └─────────────────────────────────────────────────┘ │
└─────────────────────────────────────────────────────┘
```

### Description Field:
```
┌─────────────────────────────────────────────────────┐
│ Description                                         │
│ ┌─────────────────────────────────────────────────┐ │
│ │ Practice for your BCOR 3750 Midterm Interview   │ │
│ │ (Milestone 1) with realistic simulation,        │ │
│ │ Socratic questioning, and constructive feedback.│ │
│ │ Upload your slides (optional) and experience a  │ │
│ │ professor-style interview covering Foundation,  │ │
│ │ Descriptive Analytics, and Diagnostic Analytics.│ │
│ └─────────────────────────────────────────────────┘ │
└─────────────────────────────────────────────────────┘
```

### Knowledge Section After Upload:
```
┌─────────────────────────────────────────────────────┐
│ Knowledge                                           │
│ ┌─────────────────────────────────────────────────┐ │
│ │ + Upload files                                  │ │
│ │                                                 │ │
│ │ 📄 knowledge-midterm-interview-study-guide.md   │ │
│ │ 📄 knowledge-milestone-1-requirements-except... │ │
│ │ 📄 knowledge-irpm-framework-reference.md        │ │
│ │ 📄 knowledge-whiteboard-roadmap-template.md     │ │
│ └─────────────────────────────────────────────────┘ │
└─────────────────────────────────────────────────────┘
```

### Capabilities Section (All Disabled):
```
┌─────────────────────────────────────────────────────┐
│ Capabilities                                        │
│                                                     │
│ ☐ Web Browsing                                      │
│ ☐ DALL·E Image Generation                           │
│ ☐ Code Interpreter                                  │
└─────────────────────────────────────────────────────┘
```

---

**Setup Time:** 15-20 minutes
**Difficulty:** Easy (mostly copy-paste)
**Prerequisites:** ChatGPT Plus subscription (required for CustomGPTs)

---

**Questions?** See [README.md](README.md) for detailed documentation or [SETUP-INSTRUCTIONS.md](SETUP-INSTRUCTIONS.md) for quick reference.
