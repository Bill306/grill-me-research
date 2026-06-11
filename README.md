# Grill Me: Investment Research

**Your thesis isn't ready until it's survived the interrogation.**

Most investment mistakes don't come from bad analysis — they come from questions you never thought to ask. `/grill-me` is a Claude Code skill that plays the role of a relentless research director, walking your investment idea through a structured decision tree until every blind spot is exposed and every assumption is explicit.

No hand-waving. No "sounds good." Just sharp questions, one at a time, each with a recommended answer to keep things moving.

---

## Why this exists

Before committing capital or publishing research, the best investors pressure-test their thinking against a framework. But it's hard to grill yourself — you already believe your thesis. This skill gives you a sparring partner that:

- **Won't let you skip the hard questions** — research objective, time horizon, competitive framing, risk factors
- **Suggests answers** so you're not staring at a blank page — agree, disagree, or refine
- **Adapts to your responses** — follows the natural flow of the conversation, not a rigid checklist
- **Produces a clean Research Brief** at the end — ready to hand off to a team or feed into deeper analysis

It works for any asset class, any market, any language.

---

## Quick Start

### Install

```bash
claude install-skill https://github.com/Bill306/grill-me-research
```

Or manually copy `SKILL.md` to `~/.claude/skills/grill-me-research/SKILL.md`.

### Use

```
/grill-me <topic>
```

That's it. Topic can be anything:

```
/grill-me NVIDIA
/grill-me China consumer recovery
/grill-me long copper short gold
/grill-me 腾讯
/grill-me "is ASML a buy at 40x earnings"
```

---

## How it works

The skill asks one question at a time, navigating seven dimensions of investment analysis:

| Dimension | What gets challenged |
|---|---|
| **Research objective** | Are you initiating, tracking, learning, validating, or auditing? |
| **Time horizon** | 1–3 months? 6–12 months? Multi-year? Does your analysis match? |
| **Analysis boundary** | Who are you comparing against? What geography matters? |
| **Analysis layers** | Macro → industry → supply chain → company. Where's the edge? |
| **Your priors** | What do you already believe? What data do you have? What's gut? |
| **Output framing** | Buy-side or sell-side? DCF or multiples? Memo or model? |
| **Risks & blind spots** | What's the bear case? What could you be wrong about? |

The order is fluid — the skill follows your answers, not a script. It resolves dependencies between branches (e.g., time horizon affects which valuation method makes sense) before moving on.

---

## Example session

```
> /grill-me Tesla

AI: What's your research objective — initiating a position, tracking
    an existing one, or doing a sector deep-dive?

    My recommendation: Given Tesla's current inflection point around
    autonomous driving and energy storage, I'd frame this as a
    position initiation analysis with a 12-month horizon.

You: Initiating. But I'm more interested in the energy business
     than the cars.

AI: Got it — energy focus. What's your current hypothesis on Tesla
    Energy's revenue trajectory? Specifically, are you underwriting
    the Megapack backlog numbers at face value, or do you have a
    discount for execution risk?

    My recommendation: ...
```

This continues until all key branches are resolved, then produces:

```
## Research Brief
- Research target: Tesla — Energy segment focus
- Research objective: Position initiation
- Time horizon: 12 months
- Comparison dimensions: Fluence, BYD Energy Storage, historical Tesla Energy margins
- Analysis focus layers: Industry cycle (utility-scale storage), company fundamentals
- Current hypothesis: Megapack backlog understates demand; margin expansion as manufacturing scales
- Known information: Q1 earnings, deployed GWh figures, IRA subsidy structure
- Gaps to fill: Utility procurement cycle timing, cell supply constraints, margin by geography
- Deliverable format: Buy-side memo with SOTP valuation
- Key risks / traps: Cell cost assumptions, regulatory changes to IRA, Megapack pricing pressure
```

---

## Who this is for

- **Analysts** sharpening a thesis before writing it up
- **PMs** pressure-testing ideas before sizing a position
- **Students** learning how to structure investment research
- **Solo investors** who want a second opinion before committing capital
- **Anyone** preparing for an IC meeting, stock pitch, or research presentation

---

## License

MIT — use it however you want.
