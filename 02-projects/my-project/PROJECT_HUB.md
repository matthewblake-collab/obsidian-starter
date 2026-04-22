# [Project Name] — Hub
> **Open this at the start of every work session.** Everything about this project links from here.

[[00-index/HOME|← Brain Home]]

---

## What this is

**One-liner:** [What does this project do? One sentence.]
**Status:** [In development / Live / Paused]
**Started:** [Date]
**Links:** [Website / App / GitHub / etc]

---

## Live status

### Open tasks
```dataview
TASK
FROM "02-projects/my-project"
WHERE !completed
LIMIT 15
```

### Recent decisions
```dataview
LIST file.ctime
FROM "02-projects/my-project/decisions"
SORT file.ctime DESC
LIMIT 5
```

---

## Current priorities

1. [Top priority]
2. [Second priority]
3. [Third priority]

---

## Open questions

- [ ] [Question 1]
- [ ] [Question 2]

---

## Tech stack

| Layer | Technology |
|-------|-----------|
| [Frontend] | [e.g. SwiftUI / React] |
| [Backend] | [e.g. Supabase / Firebase] |
| [Hosting] | [e.g. Netlify / App Store] |

---

## Related notes

- [[../../01-rules/WORKFLOW_RULES|Workflow Rules]]
- [[../../03-skills/SKILLS_INDEX|Skills Index]]
- [[../../04-brand/BRAND_HUB|Brand Hub]]
- [[../../07-memory/CROSS_SESSION_MEMORY|What I've Learned]]
- [[../../CONTEXT_PRIMER|Context Primer]]
