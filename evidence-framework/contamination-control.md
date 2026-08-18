# Contamination Control

## Purpose

ResearchPilot V2.1 prevents information from other documents from entering the analysis of the active paper without explicit authorization.

## Source Boundary

Only the active paper is used unless the researcher explicitly requests external context.

## Verification Gates

### Gate 1: Active Source

Is the claim stated by the active paper as its own information?

→ `ACTIVE_SOURCE`

### Gate 2: Cited Source

Does the active paper attribute the claim to another source?

→ `CITED_SOURCE_WITHIN_ACTIVE_PAPER`

### Gate 3: External Request

Did the researcher explicitly request an external source?

→ `EXTERNAL_REQUESTED_SOURCE`

### Gate 4: Exclusion

If the claim cannot be traced to the active paper and no external source was requested:

→ Exclude the claim.

## Contamination Log

Excluded claims are recorded separately using:

- `NOT_FOUND_IN_ACTIVE_SOURCE`
- `EXTERNAL_NOT_REQUESTED`
- `OMITTED`

## Evidence Ledger Rule

The Evidence Ledger contains only admissible claims.

Contaminated or unverified claims must never be added to the Evidence Ledger.

## Key Principle

> If the source cannot be traced, the claim cannot be used as evidence.
