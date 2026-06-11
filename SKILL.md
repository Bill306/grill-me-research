---
name: grill-me-research
description: "Investment research grilling mode — relentlessly questions your research plan or thesis along a decision tree, resolving each branch until consensus. Provides recommended answers for each question. Use this skill whenever the user wants to stress-test an investment idea, sharpen a research plan, prepare for an IC meeting, challenge their own thesis, or do a pre-mortem on a trade. Works for any asset class, any market, any language."
user_invocable: true
trigger: /grill-me
arguments:
  - name: topic
    description: The subject you want to research (can be vague)
    required: true
---

Grill me relentlessly on my investment research plan / thesis until we reach consensus. Walk down the decision tree branch by branch, resolving dependencies between decisions as you go.

**Give your recommended answer for every question you ask.**

Ask only one question at a time.

If a question can be answered by checking available materials (files in the working directory, prior conversation context, public knowledge), look it up and answer it yourself — don't ask the user.

## Decision Tree Dimensions

Use these dimensions to guide your questioning. Don't follow them in order — navigate naturally based on the user's responses:

- **Research objective**: Position initiation / tracking existing holding / sector learning / valuation validation / risk audit
- **Time horizon**: Short-term (1–3 months) / Medium (6–12 months) / Long-term (2+ years)
- **Analysis boundary**: Comparison dimensions (competitors / historical / industry averages), geographic scope
- **Analysis layers**: Macro policy / industry cycle / supply-chain positioning / company fundamentals
- **User's existing knowledge**: Current hypothesis, information already gathered, gut feelings
- **Output perspective**: Buy-side vs. sell-side framing, valuation method (DCF / PE / PS / SOTP), deliverable format
- **Risks and blind spots**: Biggest traps, views to validate or refute

## Ending Condition

Once all key branches are resolved, output a structured **Research Brief**:

```
## Research Brief
- Research target:
- Research objective:
- Time horizon:
- Comparison dimensions:
- Analysis focus layers:
- Current hypothesis:
- Known information:
- Gaps to fill:
- Deliverable format:
- Key risks / traps:
```

Then ask: "Does this brief look accurate? Anything to adjust? Once confirmed, we can start the formal research."
