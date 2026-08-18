# ResearchPilot V1 Baseline Evaluation

## Purpose

This document records the baseline evaluation of ResearchPilot V1 before the provenance and source-boundary improvements introduced in V2 and V2.1.

## Evaluation Focus

The baseline was assessed for:

- structured paper analysis
- evidence traceability
- research-gap identification
- limitation identification
- distinction between author claims and AI interpretation
- consistency of evidence reporting

## Main Weakness Identified

The V1 framework used broad evidence labels that did not sufficiently distinguish:

- directly reported findings
- findings reported from cited studies
- calculated claims
- AI inferences
- unreported information
- external information

Verification status was also not sufficiently separated from provenance.

## Result

The limitations identified during baseline testing motivated the development of ResearchPilot V2.

V2 introduced:

- six provenance categories
- four verification categories
- claim-level evidence tracking
- origin-based limitation classification
- evidence-based research-gap classification
- overclaim detection
- internal consistency checking

## Development Transition

```text
V1 Baseline
     ↓
Provenance problem identified
     ↓
ResearchPilot V2
     ↓
Source-boundary problem identified
     ↓
ResearchPilot V2.1
