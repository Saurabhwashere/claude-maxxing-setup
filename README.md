# Claude maxxing setup

30 setups that make Claude feel like a completely different tool. Everything from my Instagram carousel, ready to use.

By [@saurabhs.builds](https://www.instagram.com/saurabhs.builds/)

## What's inside

| # | File | What it does |
|---|---|---|
| 01–07 | [CLAUDE.md-template.md](CLAUDE.md-template.md) | Tell Claude who you are, once |
| 08–13 | [skills/](skills/) | 4 ready skills: weekly report, email reply, invoice, morning brief |
| 14–19 | [agent-workflows.md](agent-workflows.md) | Plan mode, subagents, hooks, scheduled tasks |
| 20–24 | [connector-stack.md](connector-stack.md) | What to connect and what to ask it |
| 25–30 | [taste-checklist.pdf](taste-checklist.pdf) | Run every draft through this |

## Install everything with one prompt
Using Claude Code? Paste [this one prompt](INSTALL-PROMPT.md) and Claude installs the skills and builds your CLAUDE.md with you.

## Or do it by hand (10 minutes)
1. Open [CLAUDE.md-template.md](CLAUDE.md-template.md).
2. Fill in the blanks.
3. Paste it into Claude.
4. Ask: "What do you know about me and how should you write for me?"

Then add one skill a week.

## Install the skills (Claude Code)
```bash
git clone https://github.com/Saurabhwashere/claude-maxxing-setup.git
mkdir -p ~/.claude/skills
cd claude-maxxing-setup/skills
cp -R weekly-report email-reply invoice morning ~/.claude/skills/
```
Then type `/weekly-report`, `/email-reply`, `/invoice` or `/morning`.

More install options, plus free skills from Anthropic: [skills/README.md](skills/README.md)

## License
MIT. Use it, change it, share it.
