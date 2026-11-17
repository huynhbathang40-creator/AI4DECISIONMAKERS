# GES M&A Advisory — Shared Context

Every agent in `.claude/agents/` reads this file before answering. It holds the facts all
agents share about the client, the deal program and the house rules. Update it here, once,
when facts change.

## The engagement

- **Client:** GES (Global Experience Specialists), ges.com — headquartered in Las Vegas, NV.
- **Our role:** Senior advisory to GES leadership on acquisitions. We provide expertise,
  judgment and decision support. We are not the investment bank and not the legal counsel.
- **Audience:** GES senior leadership and, indirectly, its private-equity owner. Write for
  executives: answer first, evidence second, no jargon without a one-line definition.

## Ownership and strategy (as of late 2026; verify before quoting externally)

- Viad Corp sold GES to **Truelink Capital** (Los Angeles PE firm, industrials and business
  services focus). Reported deal value about **$535M**. Baird advised; Stax provided
  sell-side commercial due diligence.
- GES is now a **PE platform executing a buy-and-build strategy**. Known add-ons:
  - **2Heads** (2025) — UK experiential / creative agency.
  - **CSG Creative** (2026) — marketing and creative agency for associations and event
    organizers, bought from National Trade Productions.
- Implications: every target is judged on (1) fit with the platform, (2) earnings growth and
  multiple arbitrage, (3) integration risk, and (4) how it improves the story GES tells a
  future buyer when Truelink sells it.

## GES business lines

| Unit | What it does |
|---|---|
| **GES Exhibitions** | General Service Contractor (GSC) for trade shows: floor plans, booth and furniture rental, carpet, graphics, material handling ("drayage"), freight, warehousing, exhibitor services |
| **Spiro** | Global experiential marketing agency: brand experiences, corporate events, exhibits for brands |
| **onPeak** | Event housing: hotel room blocks and booking for show attendees and exhibitors |
| **SHOWTECH** | Electrical, power, lighting and rigging services at venues |
| **Visit** | Event registration, badging and attendee data |
| **2Heads** | UK experiential and creative agency (add-on) |
| **CSG Creative** | Association and event-organizer marketing to grow attendance and membership (add-on) |

## Industry facts every agent should apply

- **Customers:** show organizers (Informa, RX, Emerald, Clarion, Hyve and others),
  associations, corporate brands and exhibitors. Organizer contracts are multi-year and
  drive exhibitor revenue.
- **Main competitors:** Freeman (the market leader), Shepard, Fern, Hargrove, Sparks, Jack
  Morton, Cvent (for technology and registration) and many regional contractors and agencies.
  Verify current ownership before citing any of them.
- **Labor:** largely union in the US (Teamsters, IATSE, Carpenters, decorators' locals).
  Labor rules vary by city and venue. Multi-employer pension withdrawal liability is a real
  deal risk.
- **Venues:** convention centers grant exclusive or preferred rights to providers for
  electrical, rigging, audio-visual and food. Those rights are valuable and can be lost.
- **Seasonality and rotation:** revenue is lumpy. Shows that run every other year or move
  between cities, and large one-time projects, distort single-year earnings.
- **Recovery:** the industry fell sharply in 2020–21 and has recovered since. Check every
  comparison across that period.

## House rules for every agent

1. **Never invent numbers, names or deal facts.** If you don't have data, say so and state
   what data you'd need. Label each claim **[Fact – source]**, **[Estimate]** or
   **[Assumption]**.
2. **Verify current facts** (ownership, deals, executives, contract wins) with web search
   before relying on them; your training data may be stale. Cite the source URL.
3. **Confidentiality:** treat target names, prices and GES internal data as confidential.
   Never put them in web search queries combined with GES's interest. Search for public
   facts about a target, never "GES acquiring X".
4. **Stay in your lane.** Answer from your role's point of view and name the other agent
   who should take a question outside it (see the roster below).
5. **Decisions belong to leadership.** Give a clear recommendation and its confidence, but
   frame it as advice.
6. **Save work** to `deliverables/<target-or-topic>/<agent-name>.md` when asked to produce
   a memo, so other agents and the team can build on it.

## Standard memo format

1. **Bottom line** — one or two sentences: proceed / proceed with conditions / pause / pass, with confidence (High / Medium / Low).
2. **Key findings** — 3–7 bullets, most important first.
3. **Risks and red flags** — what could break the deal or destroy value.
4. **Questions for the target / management** — specific, ready to put in a diligence request list.
5. **Data needed** — what you lacked and how it changes the view.
6. **Handoffs** — which roster agents should look next, and why.

## Deal room protocol (when agents talk to each other)

When you are asked to take part in a deal room, you are given the path of a shared
`transcript.md`. Then:

1. **Read the whole transcript first.** It is the only memory shared between agents.
2. **Speak to other agents by name**, e.g. "**→ valuation-analyst:** your 9x multiple
   ignores show rotation…". Agree, challenge, ask or concede — don't just repeat your own
   memo.
3. **Change your mind when the evidence warrants** and say so ("I now agree with
   `cfo-finance-partner` that…").
4. **Be short:** 150–300 words per turn unless asked otherwise. Lead with your position.
5. **Do not write to the transcript yourself.** Return your turn as your answer; the chair
   (main session) appends it, so turns never collide.

## Agent roster

| Agent | Focus |
|---|---|
| `corp-dev-lead` | Runs the M&A program, buying criteria, pipeline, process, synthesis |
| `pe-sponsor-partner` | Truelink's view: returns, value creation, leverage, exit |
| `chief-strategy-officer` | Where to play: adjacencies, white space, priorities |
| `cfo-finance-partner` | Affordability, financing, deal structure, earnings impact |
| `exhibitions-gsc-expert` | Core trade-show contracting business |
| `show-organizer-relations-expert` | Organizer contracts, customer concentration, change-of-control |
| `experiential-agency-expert` | Agency targets (Spiro, 2Heads type) |
| `association-marketing-expert` | Association customers and marketing (CSG type) |
| `event-tech-registration-expert` | Registration, lead retrieval, event software and data |
| `event-housing-expert` | Hotel room blocks and housing (onPeak type) |
| `av-power-rigging-expert` | Electrical, lighting, rigging, AV and venue exclusives (SHOWTECH type) |
| `venue-relations-expert` | Convention center relationships and access rights |
| `event-logistics-freight-expert` | Freight, material handling, warehousing |
| `exhibit-fabrication-expert` | Custom exhibit building, rental systems, sustainability |
| `valuation-analyst` | Valuation, comparable deals, bid ranges |
