# GES M&A Advisory Workspace

This repository supports senior-leadership advisory to GES (Global Experience Specialists)
on its acquisition program. It is an advisory workspace, not a software product.

- Shared client facts, house rules and memo format: `context/ges-company-profile.md`
  (read it before any GES work).
- Specialist agents: `.claude/agents/` (15 roles; roster in the context file).
- Multi-agent debate: `/deal-room <question>` (`.claude/commands/deal-room.md`).
- Outputs go in `deliverables/`.

When a question spans several roles, delegate to the relevant agents in parallel and
synthesise; for contested decisions, use the deal room so the agents challenge each other.
