# Agent workflows

How to make Claude do the work, not just talk about it. These are for Claude Code, unless marked otherwise.

---

## 14. Plan mode first
Press **Shift+Tab** until you see "plan mode on". Claude reads and thinks, but can't change anything.

Use it for anything bigger than a one-line fix:
1. Describe the goal.
2. Read the plan. Push back on anything wrong.
3. Approve it. Then Claude builds.

Fixing a bad plan takes 1 minute. Fixing bad work takes 1 hour.

## 15. Claude Code, not chat
Chat gives you text to copy. Claude Code edits files, runs commands and checks its own work.

Good first projects that aren't "coding":
- A folder of notes: "Turn these meeting notes into a task list."
- Your content folder: "Rename these 40 images by what's in them."
- A spreadsheet: "Clean this CSV and tell me the top 5 customers."

## 16. Scheduled tasks
Have Claude run a prompt on a timer. Ideas:
- 7:00 daily: `/morning` brief.
- Friday 16:00: `/weekly-report` from this week's notes.
- Monday 9:00: "Check my inbox for unpaid invoices and draft reminders."

In Claude Code, type `/schedule` and describe what you want in plain English.

## 17. Subagents
Subagents are helpers with their own job and their own context. The main Claude hands them work and gets back a summary.

Easiest way: just ask. "Use subagents to research these 5 competitors in parallel."

Make a reusable one: save a file at `.claude/agents/researcher.md`:
```markdown
---
name: researcher
description: Researches a company or topic and returns a short summary with sources.
---
Find the facts. Cite every source. Return max 10 bullet points.
```

## 18. Hooks for auto-checks
Hooks are commands that run automatically at set moments, like after Claude edits a file. Use them for checks you'd forget.

Examples:
- After every edit: run your formatter or spell-checker.
- Before finishing: run the tests.

Easiest setup: ask Claude Code "Add a hook that runs <your check> after every file edit." It writes the config for you.

## 19. Run 4 sessions at once
Each session works on its own task in parallel:
- Session 1: sorting your inbox.
- Session 2: building a landing page.
- Session 3: researching competitors.
- Session 4: drafting invoices.

Give each one a clear goal and a "done looks like" line. Check back when they finish, not while they work.

---

**Rule of thumb:** if you explain the same thing twice, make it a skill. If you check the same thing twice, make it a hook. If you do it on a schedule, make it a scheduled task.
