# BCOR 3750 Final Interview Coach - Custom GPT Setup Guide

This guide walks you through creating the **BCOR 3750 Final Interview Coach** Custom GPT in ChatGPT.

## Prerequisites

- ChatGPT Plus, Team, or Enterprise subscription (Custom GPTs require a paid plan)
- Access to ChatGPT at https://chat.openai.com

## Files in This Directory

| File | Purpose |
|------|---------|
| `custom-gpt-instructions.md` | System instructions to paste into the GPT configuration |
| `knowledge-final-interview-study-guide.md` | Upload as knowledge file |
| `knowledge-milestone-2-requirements.md` | Upload as knowledge file |
| `knowledge-milestone-3-requirements.md` | Upload as knowledge file |
| `README.md` | This setup guide |

## Step-by-Step Setup Instructions

### Step 1: Navigate to GPT Creation

1. Go to https://chat.openai.com
2. Click on your profile icon in the bottom-left corner
3. Select **"My GPTs"** from the menu
4. Click **"+ Create"** or **"Create a GPT"** button

### Step 2: Configure Basic Settings

In the **Create** tab, you can chat with GPT Builder, but for precise control, click the **Configure** tab instead.

**Name:**
```
BCOR 3750 Final Interview Coach
```

**Description:**
```
Practice coach for BCOR 3750 Final Interview covering Predictive Analytics (Milestone 2) and Prescriptive Analytics (Milestone 3). Simulates realistic interview experience with personalized feedback based on your uploaded slides.
```

**Instructions:**
Copy and paste the ENTIRE contents of `custom-gpt-instructions.md` into the Instructions field.

### Step 3: Upload Knowledge Files

In the **Knowledge** section, click **"Upload files"** and add these three files:

1. `knowledge-final-interview-study-guide.md`
2. `knowledge-milestone-2-requirements.md`
3. `knowledge-milestone-3-requirements.md`

These files give the GPT context about interview requirements, rubric, timing, and expectations.

### Step 4: Configure Conversation Starters

Add these conversation starters (copy each one):

```
I want to practice the full 20-minute interview
```

```
Help me prepare my 'Tell me about yourself' with project segue
```

```
Practice Milestone 2 (Predictive) only
```

```
Practice Milestone 3 (Prescriptive) only
```

```
Quiz me on Time Series Forecasting
```

```
Quiz me on Linear Programming and Sensitivity Analysis
```

```
Ask me challenging 'Why?' questions
```

```
Give me feedback on my whiteboard approach
```

### Step 5: Configure Capabilities

Enable the following capabilities:
- [x] **Web Browsing** - OFF (not needed)
- [x] **DALL-E Image Generation** - OFF (not needed)
- [x] **Code Interpreter** - OFF (not needed)

Keep all capabilities OFF to ensure focused interview coaching experience.

### Step 6: Set Profile Picture (Optional)

You can generate or upload a profile picture. Suggested prompt for DALL-E:
```
A professional, friendly coaching icon for a business analytics interview preparation tool. Blue and gold color scheme (LMU colors). Clean, modern design with elements suggesting data analysis, charts, and professional development.
```

Or use a simple professional icon/image of your choice.

### Step 7: Save and Test

1. Click **"Save"** in the top-right corner
2. Choose visibility:
   - **"Only me"** - for testing
   - **"Anyone with a link"** - to share with students
3. Click **"Confirm"**

### Step 8: Test the GPT

After saving, test the GPT by:

1. Starting a new conversation with it
2. Trying each conversation starter
3. Uploading sample Milestone 2/3 slides to test personalization
4. Testing Voice Mode (click the sound wave icon)
5. Verifying it asks appropriate questions and gives structured feedback

## Sharing with Students

Once tested and ready:

1. Go to **My GPTs**
2. Click on **BCOR 3750 Final Interview Coach**
3. Click the **"..."** menu and select **"Share"**
4. Set to **"Anyone with the link"**
5. Copy the link
6. Share in course materials and study guide

**Expected URL format:**
```
https://chatgpt.com/g/g-[unique-id]-bcor-3750-final-interview-coach
```

## Updating the GPT

To update instructions or knowledge files:

1. Go to **My GPTs**
2. Click on **BCOR 3750 Final Interview Coach**
3. Click **"Edit"** (pencil icon)
4. Make changes in the Configure tab
5. Click **"Save"** → **"Confirm"**

## Troubleshooting

**GPT doesn't recognize uploaded slides:**
- Ensure students upload PDF or image files of their actual slides
- Remind students to upload BOTH M2 and M3 slides for full practice

**Responses are too generic:**
- Check that all three knowledge files are uploaded
- Verify the full instructions were pasted (not truncated)

**Voice Mode not working:**
- Voice Mode requires ChatGPT mobile app or desktop app
- Web browser has limited voice support
- Recommend students use the mobile app for voice practice

**GPT is too easy/hard:**
- Students can request difficulty level: "Switch to Challenging mode" or "Use Practice mode"
- The instructions include three difficulty levels

## Quick Reference

| Setting | Value |
|---------|-------|
| Name | BCOR 3750 Final Interview Coach |
| Knowledge Files | 3 (study guide + M2 requirements + M3 requirements) |
| Capabilities | All OFF |
| Visibility | Anyone with link (for students) |

## Support

For issues with the Custom GPT configuration, contact the course instructor.

For ChatGPT platform issues, see: https://help.openai.com/
