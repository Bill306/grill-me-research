# Grill Me: Investment Research

**Your thesis isn't ready until it's survived the interrogation.**

Most investment mistakes don't come from bad analysis — they come from questions you never thought to ask. This skill turns Claude into a relentless research director who walks your investment idea through a structured decision tree, one sharp question at a time, until every blind spot is exposed and every assumption is explicit.

No hand-waving. No "sounds good." Just focused questions, each with a recommended answer to keep things moving.

## Why this exists

Before committing capital or publishing research, the best investors pressure-test their thinking against a framework. But it's hard to grill yourself — you already believe your thesis. This skill gives you a sparring partner that:

- **Won't let you skip the hard questions** — objective, horizon, competitive framing, risk factors, all get examined
- **Suggests answers** so you're not staring at a blank page — agree, disagree, or refine
- **Adapts to your responses** — follows the natural flow of the conversation, not a rigid checklist
- **Does its own homework** — checks your files and context before asking you for information it can find itself
- **Produces a clean Research Brief** at the end — a structured output ready to hand off or feed into deeper analysis

Works for any asset class, any market, any language.

## Install

### Claude Code

```bash
claude install-skill https://github.com/Bill306/grill-me-research
```

### Claude.ai

Download and upload `SKILL.md` via **Settings → Skills**. See [Using skills in Claude](https://support.claude.com/en/articles/12512180-using-skills-in-claude) for details.

### Manual

Copy the `SKILL.md` file into your Claude Code skills directory:

```
~/.claude/skills/grill-me-research/SKILL.md
```

## Usage

Just tell Claude what you want to research:

```
I want to research NVIDIA's data center business
```

Or be as vague as you want:

```
Is copper a good trade right now?
```

The skill activates whenever Claude detects you're trying to sharpen an investment idea, prepare for an IC meeting, or stress-test a thesis.

### Example session

```
You:  I want to research Tesla's energy business

AI:   What's your research objective — are you initiating a position,
      tracking an existing holding, or doing a sector deep-dive?

      My recommendation: Given Tesla Energy's inflection point around
      Megapack and utility-scale storage, I'd frame this as a position
      initiation analysis with a 12-month horizon.

You:  Initiating. More interested in energy than cars.

AI:   What's your current hypothesis on Tesla Energy's revenue
      trajectory? Are you underwriting the Megapack backlog at face
      value, or discounting for execution risk?

      My recommendation: I'd apply a 15-20% haircut to the stated
      backlog given Tesla's history of production timeline slips,
      and model revenue recognition against deployed GWh rather than
      bookings.

      ...
```

This continues through all relevant branches — time horizon, competitive comparisons, valuation method, risk factors — until consensus is reached. Then:

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

## What gets covered

The skill navigates seven dimensions of investment analysis, in whatever order the conversation demands:

| Dimension | What gets challenged |
|---|---|
| **Research objective** | Are you initiating, tracking, learning, validating, or auditing? |
| **Time horizon** | 1–3 months? 6–12 months? Multi-year? Does your analysis match? |
| **Analysis boundary** | Who are you comparing against? What geography matters? |
| **Analysis layers** | Macro → industry → supply chain → company. Where's the edge? |
| **Existing knowledge** | What do you already believe? What's data vs. gut? |
| **Output framing** | Buy-side or sell-side? DCF or multiples? Memo or model? |
| **Risks & blind spots** | What's the bear case? What would make you wrong? |

## Who this is for

- **Analysts** sharpening a thesis before writing it up
- **Portfolio managers** pressure-testing ideas before sizing a position
- **Students** learning how to structure investment research
- **Solo investors** who want a second opinion before committing capital
- **Anyone** preparing for an IC meeting, stock pitch, or research presentation

## Skill format

This skill follows the [Agent Skills specification](https://agentskills.io/specification). It consists of a single `SKILL.md` file with no additional dependencies — just install and go.

## License

[MIT](LICENSE)
