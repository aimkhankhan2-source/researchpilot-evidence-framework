# ResearchPilot V2.1

## Evidence-Grounded AI Framework with Source-Boundary Control

ResearchPilot V2.1 extends V2 with explicit source categorization, active-paper boundaries, contamination detection, and separate evidence and exclusion logs.

The goal is to make academic literature analysis more traceable and resistant to cross-document contamination.

---

# 1. Source Boundary Rule

Only the **active paper** is an admissible source unless the researcher explicitly requests external context.

Before using any claim, ask:

> Where does this claim come from?

The system must route every claim through the following gates.

---

## Gate 1: ACTIVE_SOURCE

A claim is `ACTIVE_SOURCE` only when:

1. The claim appears in the active paper.
2. The active paper reports it as its own methodology, observation, analysis, result, interpretation, or conclusion.
3. The paper does not attribute the claim to another source.

Example:

> "The review included 13 studies."

Classification:

`ACTIVE_SOURCE`

---

## Gate 2: CITED_SOURCE_WITHIN_ACTIVE_PAPER

Use this category when the active paper attributes the claim to another study, author, dataset, or external source.

Indicators include:

- "Study [n] found..."
- "Research has shown..."
- "According to [Author]..."
- "[Citation] reports..."
- findings presented from included studies

Example:

> "LIFEisGAME produced a 20% improvement."

If the active paper attributes this result to another study:

```text
Source Category:
CITED_SOURCE_WITHIN_ACTIVE_PAPER

Provenance:
CITED_SOURCE_REPORTED

Verification:
NOT_CHECKED
