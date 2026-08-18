# Contamination / Exclusion Log Example

This is a sanitized example of how ResearchPilot V2.1 records claims excluded from the Evidence Ledger.

| # | Claim | Status | Action |
|---|---|---|---|
| 1 | Claim from another project paper | `NOT_FOUND_IN_ACTIVE_SOURCE` | `OMITTED` |
| 2 | Information inferred from another document | `EXTERNAL_NOT_REQUESTED` | `OMITTED` |
| 3 | Claim encountered during analysis but not traceable to the active paper | `NOT_FOUND_IN_ACTIVE_SOURCE` | `OMITTED` |

## Rule

If a claim cannot be traced to the active paper and external context was not explicitly requested:

> Do not use the claim as evidence.

Record it in the Contamination / Exclusion Log instead.

## Separation

The Evidence Ledger contains only admissible claims.

The Contamination / Exclusion Log records rejected claims for auditability.

Excluded claims must never be used as evidence in the analysis.
