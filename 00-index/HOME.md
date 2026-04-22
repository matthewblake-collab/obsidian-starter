# [Your Name] — Brain
> **Start here every morning.** This note gives you a live snapshot of everything across your vault — open tasks, recent decisions, active sessions — without you updating anything manually.

*Vault started: [Date]*

---

## Live dashboard

### Open tasks
```dataview
TASK
FROM "02-projects"
WHERE !completed
LIMIT 10
```

### Recent decisions (last 7 days)
```dataview
LIST file.ctime
FROM #type/decision
WHERE file.ctime >= date(today) - dur(7 days)
SORT file.ctime DESC
```

### Recent sessions
```dataview
LIST file.ctime
FROM #type/session
SORT file.ctime DESC
LIMIT 5
```

---

## Active projects

| Project | Status | Hub |
|---------|--------|-----|
| [Your project] | [In progress] | [[02-projects/my-project/PROJECT_HUB\|Project Hub]] |

---

## Vault map

| Section | What's in here |
|---------|---------------|
| [[01-rules/WORKFLOW_RULES\|Workflow Rules]] | Rules for every AI and coding session |
| [[01-rules/AI_TOOLS_RULES\|AI Tools Rules]] | Claude Code, MCP config, installed tools |
| [[02-projects/my-project/PROJECT_HUB\|Project Hub]] | Everything about your main project |
| [[03-skills/SKILLS_INDEX\|Skills Index]] | Reusable AI workflow notes |
| [[04-brand/BRAND_HUB\|Brand Hub]] | Voice, tone, content rules |
| [[07-memory/CROSS_SESSION_MEMORY\|What I've Learned]] | Compounding patterns from all sessions |
| [[CONTEXT_PRIMER\|Context Primer]] | Paste into any AI chat |

---

## How to use this vault

| What you want to do | How |
|---------------------|-----|
| Start an AI chat | Paste [[CONTEXT_PRIMER\|Context Primer]] |
| Log a session | New note in `07-memory/` → tpl-session |
| Record a decision | New note in `02-projects/my-project/decisions/` → tpl-decision |
| Weekly review | New note in `08-journal/weekly/` → tpl-weekly |
| Daily note | New note in `08-journal/daily/` → tpl-daily |
| Find anything | `Cmd/Ctrl + O` |
| Run any command | `Cmd/Ctrl + P` |
