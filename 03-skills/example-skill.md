# Skill: Session Debrief Capture

> **This is an annotated example showing how skill notes are structured.** Copy it, rename it, replace the content. Delete this example once you've written 2-3 real ones.

[[SKILLS_INDEX|← Skills Index]]

---

## When to use this skill

At the end of any AI working session — before closing the chat. Use it every time without exception.

---

## What you need before starting

- The AI chat still open
- 3 minutes
- Your `07-memory/` folder accessible

---

## Steps

1. Ask the AI: *"Summarise what we built or decided today in bullet points"*
2. Ask: *"What rules or patterns should I always apply based on today?"*
3. Ask: *"What should I watch out for next time?"*
4. Copy the output into a new note in `07-memory/` using the tpl-session template
5. If any rules are new, add them to `01-rules/WORKFLOW_RULES.md`
6. If any patterns are new, add them to `07-memory/CROSS_SESSION_MEMORY.md`
7. Update `CONTEXT_PRIMER.md` if priorities or blockers have changed

---

## Rules — never break these

- Do this before closing the chat — you cannot recover context after
- Be specific — "fixed bug" is useless; "Supabase RLS delete returns success with 0 rows — always verify with count check" is gold
- If something took 30+ minutes to figure out, it must be documented

---

## Example output

```
## Session — 2026-04-22

### What we did
- Fixed webhook silent failure on chat.update
- Added respond() fallback using response_url

### New rules
- Always check resp.get("ok") explicitly
- Return bool from update functions so callers can branch

### Watch out for next time
- response_url expires 30min after button click
```

---

## See also

- [[SKILLS_INDEX|Skills Index]]
- [[../07-memory/CROSS_SESSION_MEMORY|What I've Learned]]
