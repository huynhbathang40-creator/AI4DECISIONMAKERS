# AI4DECISIONMAKERS — GES M&A Advisory Agents

A team of 15 Claude Code subagents that advise GES (Global Experience Specialists)
leadership on acquisitions. The agents are scoped to this project: they live in
`.claude/agents/` and load automatically when Claude Code runs in this repository.

## The agents

| Group | Agents |
|---|---|
| Deal leadership | `corp-dev-lead`, `pe-sponsor-partner`, `chief-strategy-officer`, `cfo-finance-partner` |
| Industry experts | `exhibitions-gsc-expert`, `show-organizer-relations-expert`, `experiential-agency-expert`, `association-marketing-expert`, `event-tech-registration-expert`, `event-housing-expert`, `av-power-rigging-expert`, `venue-relations-expert`, `event-logistics-freight-expert`, `exhibit-fabrication-expert` |
| Financial analysis | `valuation-analyst` |

All agents share `context/ges-company-profile.md` (client facts, house rules, memo
format). Update facts there once, not in each agent.

## How to use them

**One agent:** name it in your request.

```
Use the valuation-analyst to build a bid range for a regional exhibit house with $40M revenue and $6M EBITDA.
```

**Agents talking to each other:** run the deal room.

```
/deal-room Should GES buy a mid-sized event registration software company?
```

The panel debates in three rounds through a shared transcript, addressing each other by
name, and `corp-dev-lead` writes a decision memo. Output goes to
`deliverables/deal-room/<topic>/`.

Type `/agents` in Claude Code to see or edit the agents.

## Using them outside Claude Code

The Claude Agent SDK loads the same files when project settings are enabled
(`setting_sources=["project"]` in Python, `settingSources: ["project"]` in TypeScript).
See https://code.claude.com/docs/en/agent-sdk.
