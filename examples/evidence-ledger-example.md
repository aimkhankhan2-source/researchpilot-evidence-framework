# Evidence Ledger Example

This is a sanitized example showing how ResearchPilot V2.1 records evidence.

| # | Claim | Source Category | Provenance | Verification |
|---|---|---|---|---|
| 1 | The review included 13 studies | `ACTIVE_SOURCE` | `DIRECTLY_REPORTED` | `SOURCE_CHECKED` |
| 2 | A cited study reported a 20% improvement | `CITED_SOURCE_WITHIN_ACTIVE_PAPER` | `CITED_SOURCE_REPORTED` | `NOT_CHECKED` |
| 3 | 50% of 128 records equals 64 | `ACTIVE_SOURCE` | `CALCULATED` | `SOURCE_CHECKED` |
| 4 | A possible methodological concern is identified by analysis | `ACTIVE_SOURCE` | `INFERRED` | `SOURCE_CHECKED` |

## Important Distinction

A claim can be present in the active paper while still being classified as:

`CITED_SOURCE_WITHIN_ACTIVE_PAPER`

when the paper attributes that claim to another study.

`SOURCE_CHECKED` does not mean `HUMAN_VERIFIED`.

## Purpose

The ledger makes each claim traceable by recording:

- what the claim says
- where it came from
- its provenance
- its verification status
