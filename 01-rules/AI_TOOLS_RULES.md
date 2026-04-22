# AI Tools Rules
*Tool-specific rules. Keep separate from general workflow rules so each has a clean home.*

[[00-index/HOME|← Home]] | [[WORKFLOW_RULES|Workflow Rules]]

---

## Claude Code

### Non-obvious config
- MCP config must go in `~/.claude/settings.json` — `claude mcp add` writes to `~/.claude.json` which Claude Code ignores silently
- If an MCP server fails after 2 attempts: restart the session, don't keep debugging in-session

### Session memory
- Phrase memory saves as natural language — some tools intercept `/dream`
- Use an `/observe`-style skill at session end to capture learnings back to vault

### Useful slash commands
| Command | What it does | Type |
|---------|-------------|------|
| `/ultraplan` | Cloud planning for complex multi-file features | ✅ Official |
| `/debug` | Investigate errors and trace root cause | Bundled |
| `/simplify` | Refactor complex code | Bundled |

### Installed tools — fill this in
> List your Claude Code skills and plugins here. Check before installing anything new.

- [Tool name] — [what it does]

---

## Claude.ai (chat)

- Always paste `CONTEXT_PRIMER.md` at the start of any new project session
- Use **Projects** for persistent context on long-running work
- Single copiable code blocks only — no nested formatting

---

## Patterns learned from real failures

> Add entries here when a tool wastes significant time.

- [e.g. "Tool X doesn't work for task Y — caused 2 wasted sessions"]

---

## See also
- [[00-index/HOME|← Home]]
- [[WORKFLOW_RULES|Workflow Rules]]
- [[../07-memory/CROSS_SESSION_MEMORY|What I've Learned]]
