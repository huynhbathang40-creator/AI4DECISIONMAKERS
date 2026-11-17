---
description: Convene the GES advisory agents in a deal room — they debate a question in rounds, talking to each other, and the corp-dev lead writes the decision memo
argument-hint: <question, target or scenario>
---

You are the **chair** of a GES M&A deal room. The question is:

> $ARGUMENTS

The agents in `.claude/agents/` are the participants. They cannot message each other
directly, so a shared transcript file carries the conversation: each round, every
participant reads the transcript and responds to the others by name. Follow these steps.

## 1. Set up
- Read `context/ges-company-profile.md`.
- Make a short kebab-case slug from the question and create
  `deliverables/deal-room/<slug>/transcript.md` with a title, the question, today's date
  and an empty "Panel" section.
- Choose a **panel of 4–7 agents** most relevant to the question. Always include
  `corp-dev-lead` (it closes the session). Include `pe-sponsor-partner`, `cfo-finance-partner`
  or `valuation-analyst` whenever price, returns or financing are in play. Write the panel
  and a one-line reason for each into the transcript and tell the user who is in the room.

## 2. Round 1 — Opening positions
Run every panelist **in parallel** (one Agent call each, same message). Tell each one:
the transcript path, the question, "Round 1: give your opening position from your role in
150–300 words: your view, your top risk, and one question for a named colleague in the panel."
Append each answer to the transcript under `## Round 1` as `### <agent-name>`.

## 3. Round 2 — Cross-examination
Run every panelist in parallel again. Tell each one: "Read the full transcript. Round 2:
respond directly to at least two other panelists by name — challenge, agree, or answer the
question they asked you. Change your position if the evidence warrants." Append under
`## Round 2`.

## 4. Round 3 — Rebuttal and final position
Run only the panelists who were challenged or asked a question in Round 2 (in parallel).
Tell each: "Read the transcript. Round 3: answer the challenges aimed at you, then state
your final position in one line: proceed / proceed with conditions / pause / pass."
Append under `## Round 3`.

## 5. Decision memo
Run `corp-dev-lead` alone: "Read the full transcript. As chair-of-record, write the decision
memo in the house format, with an extra section 'Where the panel agreed' and 'Unresolved
disagreements (who vs. who, and what data would settle it)'." Save it as
`deliverables/deal-room/<slug>/decision-memo.md`.

## 6. Show the user
In your reply, replay the conversation as a readable exchange, not a file dump:
- For each round, show each turn as **`agent-name → other-agent:`** followed by the key
  point (1–3 sentences), keeping the most important challenges and changes of mind.
- Then the decision memo's bottom line and the unresolved disagreements.
- End with the paths to the full transcript and memo.

Rules: never invent data for the agents — if they lack information they must say so; keep
all target names and prices out of web searches combined with GES's interest.
