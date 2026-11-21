# Connector stack

Claude is 10x more useful when it can see your real stuff. Here's what to connect and what to ask once it's connected.

---

## 20. Gmail, Notion, Drive, Calendar
Claude app > Settings > Connectors. Turn on the ones you use.

| Connector | Ask it |
|---|---|
| Gmail | "Which emails from this week still need a reply from me?" |
| Google Calendar | "Find 3 free 30-minute slots next week for a client call." |
| Google Drive | "Summarize the last 3 proposals I sent and what they had in common." |
| Notion | "Turn this meeting into tasks in my Projects database." |

Start read-only. Let it draft, you send.

## 21. Claude in Chrome
A browser extension that lets Claude click, type and read pages for you.

Good jobs for it:
- "Compare these 6 flights and fill in the booking form up to payment."
- "Go through these 10 competitor pricing pages and make a table."

You stay in control of logins and payments. Watch the first few runs.

## 22. Claude Desktop app
Install the desktop app instead of using a browser tab. You get a keyboard shortcut to open Claude from anywhere, plus local files and tools.

## 23. MCP connectors
MCP (Model Context Protocol) is the plug that connects Claude to other apps. Most connectors are MCP under the hood.

- Check the connector directory in Settings > Connectors first.
- Your favorite app not there? Search "<app name> MCP server". Most big tools have one.
- In Claude Code: `claude mcp add` connects one from the terminal.

Only install connectors from companies or developers you trust. A connector can read what you give it access to.

## 24. Computer use
Claude can control a desktop app by looking at the screen and clicking. Slower than a connector, but works with apps that have no connector.

Use it for: old desktop software, apps with no API, one-off repetitive clicking.

---

**A good starting stack:** Gmail + Calendar + Notion + Drive connectors, Claude in Chrome for the web, Claude Code for files and automations.
