---
name: morning
description: Gives me a short daily brief to start the day. Use when I say "morning", "daily brief", or "what's on today".
---

# Morning brief

## Steps
1. If calendar is connected, list today's meetings with times. Flag any clashes.
2. If email is connected, find emails that need a reply from me today. Max 5. One line each.
3. Read `references/priorities.md` if it exists, and pick my top 3 tasks for today.
4. Put it all in this layout:

```
Today, <day date>

Meetings
- <time> <meeting>

Reply today
- <sender>: <what they need>

Top 3
1. <task>
2. <task>
3. <task>

One thing to watch: <risk, deadline or clash, or "nothing">
```

## Rules
- Whole brief fits on one phone screen.
- If a connector isn't set up, skip that section and say so in one line.
- No motivational quotes.

## Run it every day
Set up a scheduled task that runs "/morning" every day at 7:00. In Claude Code you can type `/schedule` and describe it in plain English.
