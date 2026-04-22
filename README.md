# Obsidian Starter Vault

> **ELI5:** This is a ready-to-use folder you open with Obsidian. Everything is set up — folder structure, templates, live dashboards, AI prompt files. Replace the `[bracket]` placeholders with your own info and you're running in under 15 minutes.

---

## What you're getting

- **Context Primer** — one file you paste into any AI (Claude, ChatGPT, Gemini) for instant full context every session. No more re-explaining yourself.
- **Live dashboards** — Dataview queries that show your open tasks, recent decisions, and active sessions automatically.
- **Templates** — Templater templates for daily notes, weekly reviews, monthly reviews, session debriefs, and decisions.
- **Skill notes** — reusable AI workflow files that Claude Code can load directly.
- **Memory file** — where lessons from every AI session compound over time.

---

## Get running in 15 minutes

### Step 1 — Download Obsidian (free)
→ https://obsidian.md/download
Mac · Windows · Linux · iOS · Android. Free for personal use.

### Step 2 — Open this folder as a vault
1. Open Obsidian
2. Click **"Open folder as vault"**
3. Select the `obsidian-starter` folder
4. Click Open

### Step 3 — Install the plugins
Settings (gear icon) → Community plugins → Turn off Safe mode → Browse

| Plugin | Why |
|--------|-----|
| **Templater** | Powers all the templates in 09-templates/ |
| **Dataview** | Powers the live queries in HOME.md |
| **Periodic Notes** | Auto-creates daily/weekly/monthly notes |
| **Calendar** | Sidebar calendar navigation |
| **Obsidian Git** | Auto-backup to GitHub |
| **Tasks** | Cross-vault task tracking |

### Step 4 — Configure Templater
Settings → Templater → Template folder location → `09-templates`
Turn on: "Trigger Templater on new file creation"

### Step 5 — Fill in your Context Primer
Open `CONTEXT_PRIMER.md`. Replace every `[bracket]` with your real info. This is the most important file in the vault.

### Step 6 — Pin HOME.md
Open `00-index/HOME.md`. Right-click the tab → Pin. Open this every morning.

---

## Folder structure

```
obsidian-starter/
├── 00-index/          ← Daily entry point. Open this every morning.
├── 01-rules/          ← Rules for AI sessions, workflow, and tools
├── 02-projects/       ← One sub-folder per project
│   └── my-project/
│       └── decisions/ ← One note per major decision
├── 03-skills/         ← Reusable AI workflow notes
├── 04-brand/          ← Voice, tone, content rules
├── 05-resources/      ← Tools, links, reference material
├── 07-memory/         ← Patterns and learnings that persist forever
├── 08-journal/        ← Daily, weekly, monthly reviews
│   ├── daily/
│   ├── weekly/
│   └── monthly/
├── 09-templates/      ← Templater templates (don't rename these)
├── CONTEXT_PRIMER.md  ← Paste into any AI session ← START HERE
└── README.md          ← This file
```

> **Why numbered folders?** Numbers keep a fixed order in the sidebar. 00 is always first. Easier to navigate when the vault grows.

---

## For developers using Claude Code

Add Filesystem MCP to `~/.claude/settings.json`:

```json
{
  "mcpServers": {
    "filesystem": {
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-filesystem", "/path/to/obsidian-starter"]
    }
  }
}
```

Then in your project's `CLAUDE.md`:
```
Context: ~/obsidian-starter/CONTEXT_PRIMER.md
Rules: ~/obsidian-starter/01-rules/WORKFLOW_RULES.md
Memory: ~/obsidian-starter/07-memory/CROSS_SESSION_MEMORY.md
```

Claude reads these automatically at session start. You never explain your project from scratch again.

---

## Contributing back

If you improve a template, prompt, or structure — submit a pull request. Everyone using this setup benefits.

1. Fork the repo
2. Make your improvement
3. Submit a PR with a clear description of what got better
4. Gets reviewed, merged, live for everyone
5. `git pull` to get the update in your vault

---

## Links
- Obsidian: https://obsidian.md/download
- Docs: https://help.obsidian.md
- Plugins: https://obsidian.md/plugins
- Forum: https://forum.obsidian.md
