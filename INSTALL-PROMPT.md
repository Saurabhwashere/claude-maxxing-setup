# One-prompt install

Open **Claude Code** (terminal, desktop app or IDE), paste everything in the box below, and press Enter. Claude installs the skills and builds your personal CLAUDE.md with you. It takes about 5 minutes.

```text
Set up the "Claude maxxing" pack for me from https://github.com/Saurabhwashere/claude-maxxing-setup

Work through these steps in order. Ask me before you overwrite or delete anything.

1. DOWNLOAD
   Clone the repo into a temporary folder.

2. INSTALL THE SKILLS
   Copy these 4 folders from the repo's skills/ folder into ~/.claude/skills/ (create it if needed):
   weekly-report, email-reply, invoice, morning
   If a skill with the same name already exists, show me the difference and ask before replacing it.

3. BUILD MY CLAUDE.md
   Read CLAUDE.md-template.md from the repo.
   Then interview me to fill it in. Ask ONE question at a time and wait for my answer:
   - What do you do, and who do you do it for?
   - What are you working on right now? (1 to 3 things)
   - How do you like answers: short or detailed?
   - Describe your writing voice in 3 words.
   - Paste 3 to 5 sentences you wrote that sound like you.
   - Any words or phrases you never want to see?
   - Which tools do you use every day?
   - Which currency and units should I use?
   Keep the file under 60 lines and remove every hint and placeholder.
   Save it to ~/.claude/CLAUDE.md. If that file already exists, back it up to ~/.claude/CLAUDE.md.backup first, then merge: keep my existing rules and add the new sections.

4. SAVE THE GUIDES
   Copy agent-workflows.md, connector-stack.md and taste-checklist.pdf to ~/claude-maxxing/ so I can read them later.

5. CLEAN UP
   Delete the temporary clone.

6. REPORT
   Tell me in under 10 lines:
   - Which skills were installed and how to use each one (/weekly-report, /email-reply, /invoice, /morning).
   - Where my CLAUDE.md is, and show it to me.
   - Where the guides are.
   - One optional extra: to add Anthropic's free skills, I can type these two commands myself:
     /plugin marketplace add anthropics/skills
     /plugin install example-skills@anthropic-agent-skills

Finally, test it: answer "What do you know about me and how should you write for me?" using my new CLAUDE.md.
```

## After it's done
- Restart Claude Code so it picks up the new skills.
- Type `/morning` to try your first skill.
- Using the Claude app instead of Claude Code? Copy your new CLAUDE.md into Settings > Profile, and upload each skill folder as a zip under Skills.
