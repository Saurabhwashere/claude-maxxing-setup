# Skills pack

4 skills: `weekly-report`, `email-reply`, `invoice`, `morning`.

Each skill is a folder with a `SKILL.md` inside. Claude reads the name and description, and loads the skill when your request matches.

## Install

**Claude Code**
Copy each folder into `~/.claude/skills/` (all projects) or `.claude/skills/` inside one project.
Then type `/weekly-report`, `/email-reply`, `/invoice` or `/morning`.

**Claude app (claude.ai / Desktop)**
Zip one skill folder on its own (e.g. `weekly-report.zip`) and upload it in Settings > Capabilities > Skills.

## Make them yours
1. Open a `SKILL.md` and change the steps to match how you actually work.
2. Add a `references/` folder next to it with real examples (a past report, your client list, your payment details).
3. When the output is off, tell Claude what was wrong and ask it to update the SKILL.md. It gets better every week.

## Grab these from GitHub
Anthropic publishes free, ready-made skills at https://github.com/anthropics/skills

My 3 picks:
- **skill-creator**: builds new skills for you. Describe a task, get a SKILL.md.
- **doc-coauthoring**: writes proposals, specs and long docs with you, section by section.
- **internal-comms**: status updates, newsletters, FAQs and team announcements.

**Claude Code:** add the repo once, then install.
```
/plugin marketplace add anthropics/skills
/plugin install example-skills@anthropic-agent-skills
```
Then just ask: "Use the skill-creator skill to make a skill for my weekly invoices."

**Claude app (paid plans):** these example skills are already built in. Turn them on in your settings under Skills.

Only install skills from sources you trust. A skill can tell Claude to run code.

## Make your own
Ask Claude: "Turn what we just did into a skill." Then save the SKILL.md it gives you.
One skill per task you do more than twice a week.
