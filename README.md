# grill-me-research

An AI skill that stress-tests your investment research plan by grilling you with relentless questions along a decision tree — until your thesis is airtight.

## What it does

When you invoke `/grill-me [topic]`, the AI becomes a demanding research director who:

1. **Asks one focused question at a time** about your research plan or investment thesis
2. **Provides its own recommended answer** for each question
3. **Walks the decision tree** — covering research objectives, time horizons, analysis layers, risks, and blind spots
4. **Resolves dependencies** between branches before moving on
5. **Produces a structured Research Brief** once all key branches are resolved

## Example

```
/grill-me Tesla
```

The AI will then ask questions like:
> "What's your research objective here — are you evaluating Tesla for a new position, tracking an existing holding, or doing a sector deep-dive? **My recommendation:** Given Tesla's current inflection point around autonomous driving and energy storage, I'd frame this as a position initiation analysis with a 12-month horizon."

## Install

### Claude Code (CLI)

```bash
claude install-skill https://github.com/Bill306/grill-me-research
```

### Manual

Copy the `SKILL.md` file into your Claude skills directory:

```
~/.claude/skills/grill-me-research/SKILL.md
```

## Usage

```
/grill-me <topic>
```

**topic** can be anything — a company name, a sector, a trade idea, or even a vague hunch:

- `/grill-me NVIDIA`
- `/grill-me China consumer recovery thesis`
- `/grill-me long copper short gold`
- `/grill-me 腾讯`

## Decision Tree Dimensions

The skill covers these angles (in whatever order makes sense):

| Dimension | Examples |
|---|---|
| Research objective | Position initiation, tracking, sector learning, valuation check, risk audit |
| Time horizon | 1–3 months, 6–12 months, 2+ years |
| Analysis boundary | Competitors, historical, industry averages, geographic scope |
| Analysis layers | Macro, industry cycle, supply chain, company fundamentals |
| Existing knowledge | Your current hypothesis, data you already have, gut feelings |
| Output perspective | Buy-side / sell-side, valuation method, deliverable format |
| Risks & blind spots | Biggest traps, views to validate or refute |

## License

MIT
